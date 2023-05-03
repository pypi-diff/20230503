# Comparing `tmp/pygmtsar-2023.4.20.tar.gz` & `tmp/pygmtsar-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2023.4.20.tar", last modified: Thu Apr 20 09:01:06 2023, max compression
+gzip compressed data, was "pygmtsar-2023.5.3.tar", last modified: Wed May  3 03:13:48 2023, max compression
```

## Comparing `pygmtsar-2023.4.20.tar` & `pygmtsar-2023.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-20 09:01:06.898529 pygmtsar-2023.4.20/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2023.4.20/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-20 09:01:06.898343 pygmtsar-2023.4.20/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     9313 2023-03-12 07:12:55.000000 pygmtsar-2023.4.20/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-20 09:01:06.897275 pygmtsar-2023.4.20/pygmtsar/
--rwxr-xr-x   0 mbg        (501) staff       (20)    25099 2023-04-16 07:24:33.000000 pygmtsar-2023.4.20/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    21884 2023-03-07 05:42:58.000000 pygmtsar-2023.4.20/pygmtsar/PRM_gmtsar.py
--rwxr-xr-x   0 mbg        (501) staff       (20)    11684 2023-03-30 13:07:17.000000 pygmtsar-2023.4.20/pygmtsar/SBAS.py
--rw-r--r--   0 mbg        (501) staff       (20)    17137 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     2161 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)     7320 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_dem_gmt_gdal.py
--rw-r--r--   0 mbg        (501) staff       (20)     8780 2023-04-05 05:10:27.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    12220 2023-04-12 18:26:43.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)     4791 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     2693 2023-04-12 07:30:31.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_intf.py
--rw-r--r--   0 mbg        (501) staff       (20)     1488 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)     1799 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_landmask_gmt.py
--rw-r--r--   0 mbg        (501) staff       (20)     4993 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_merge_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)      821 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)     9743 2023-03-07 05:42:58.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     5518 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    13303 2023-04-09 14:02:35.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     5448 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_sbas_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    10429 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_stack.py
--rw-r--r--   0 mbg        (501) staff       (20)     5630 2023-04-11 17:42:45.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_topo_ra.py
--rw-r--r--   0 mbg        (501) staff       (20)     8644 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)     1824 2023-04-20 05:34:55.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     6045 2023-04-20 05:36:07.000000 pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)      257 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    10812 2023-03-31 15:15:54.000000 pygmtsar-2023.4.20/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     1820 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)      992 2023-02-25 05:08:30.000000 pygmtsar-2023.4.20/pygmtsar/tqdm_joblib.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-04-20 09:01:06.898115 pygmtsar-2023.4.20/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    10038 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)      872 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      259 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2023-04-20 09:01:06.000000 pygmtsar-2023.4.20/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2023-04-20 09:01:06.898573 pygmtsar-2023.4.20/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     1900 2023-04-20 09:00:51.000000 pygmtsar-2023.4.20/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-05-03 03:13:48.005814 pygmtsar-2023.5.3/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2023.5.3/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    10037 2023-05-03 03:13:48.005648 pygmtsar-2023.5.3/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     9313 2023-03-12 07:12:55.000000 pygmtsar-2023.5.3/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-05-03 03:13:48.004391 pygmtsar-2023.5.3/pygmtsar/
+-rwxr-xr-x   0 mbg        (501) staff       (20)    26952 2023-04-26 17:16:46.000000 pygmtsar-2023.5.3/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    21884 2023-03-07 05:42:58.000000 pygmtsar-2023.5.3/pygmtsar/PRM_gmtsar.py
+-rwxr-xr-x   0 mbg        (501) staff       (20)    11684 2023-03-30 13:07:17.000000 pygmtsar-2023.5.3/pygmtsar/SBAS.py
+-rw-r--r--   0 mbg        (501) staff       (20)    18585 2023-05-02 08:49:02.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2161 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7320 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_dem_gmt_gdal.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8937 2023-05-02 07:02:27.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    12199 2023-05-02 07:03:04.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4791 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2752 2023-05-02 07:04:15.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_intf.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1488 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1799 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_landmask_gmt.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5052 2023-05-02 07:04:27.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_merge_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)      821 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9743 2023-03-07 05:42:58.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5518 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15522 2023-05-03 00:10:31.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5448 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_sbas_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10429 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5630 2023-04-11 17:42:45.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_topo_ra.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8644 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1825 2023-05-02 07:03:29.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6462 2023-05-02 09:02:38.000000 pygmtsar-2023.5.3/pygmtsar/SBAS_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)      257 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10812 2023-03-31 15:15:54.000000 pygmtsar-2023.5.3/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1820 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)      992 2023-02-25 05:08:30.000000 pygmtsar-2023.5.3/pygmtsar/tqdm_joblib.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2023-05-03 03:13:48.005429 pygmtsar-2023.5.3/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    10037 2023-05-03 03:13:47.000000 pygmtsar-2023.5.3/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)      872 2023-05-03 03:13:47.000000 pygmtsar-2023.5.3/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2023-05-03 03:13:47.000000 pygmtsar-2023.5.3/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      259 2023-05-03 03:13:47.000000 pygmtsar-2023.5.3/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2023-05-03 03:13:47.000000 pygmtsar-2023.5.3/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2023-05-03 03:13:48.005858 pygmtsar-2023.5.3/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     1899 2023-05-03 03:12:48.000000 pygmtsar-2023.5.3/setup.py
```

### Comparing `pygmtsar-2023.4.20/LICENSE.txt` & `pygmtsar-2023.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/PKG-INFO` & `pygmtsar-2023.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2023.4.20
+Version: 2023.5.3
 Summary: PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone
 Home-page: https://github.com/mobigroup/gmtsar
 Author: Alexey Pechnikov
 Author-email: pechnikov@mobigroup.ru
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2023.4.20/README.md` & `pygmtsar-2023.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/PRM.py` & `pygmtsar-2023.5.3/pygmtsar/PRM.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # Alexey Pechnikov, Sep, 2021, https://github.com/mobigroup/gmtsar
 from .datagrid import datagrid
 from .PRM_gmtsar import PRM_gmtsar
 
 class PRM(datagrid, PRM_gmtsar):
 
-    # replacement function for GMT based robust 2D trend coefficient calculations:
+    # my replacement function for GMT based robust 2D trend coefficient calculations:
     # gmt trend2d r.xyz -Fxyzmw -N1r -V
     # gmt trend2d r.xyz -Fxyzmw -N2r -V
     # gmt trend2d r.xyz -Fxyzmw -N3r -V
     # https://github.com/GenericMappingTools/gmt/blob/master/src/trend2d.c#L719-L744
     # 3 model parameters
     # rank = 3 => nu = size-3
     @staticmethod
-    def GMT_trend2d(data, rank):
+    def robust_trend2d(data, rank):
         import numpy as np
         from sklearn.linear_model import LinearRegression
         # scale factor for normally distributed data is 1.4826
         # https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.median_abs_deviation.html
         MAD_NORMALIZE = 1.4826
         # significance value
         sig_threshold = 0.51
@@ -73,14 +73,63 @@
             #print ('chisq', chisq, 'significant', sig)
             if sig < sig_threshold:
                 break
 
         # get the slope and intercept of the line best fit
         return (coeffs[:rank])
 
+#     # standalone function is compatible but it is too slow while it should not be a problem
+#     @staticmethod
+#     def robust_trend2d(data, rank):
+#         import numpy as np
+#         import statsmodels.api as sm
+# 
+#         if rank not in [1, 2, 3]:
+#             raise Exception('Number of model parameters "rank" should be 1, 2, or 3')
+# 
+#         if rank in [2, 3]:
+#             x = data[:, 0]
+#             x = np.interp(x, (x.min(), x.max()), (-1, +1))
+#         if rank == 3:
+#             y = data[:, 1]
+#             y = np.interp(y, (y.min(), y.max()), (-1, +1))
+#         z = data[:, 2]
+# 
+#         if rank == 1:
+#             X = sm.add_constant(np.ones(z.shape))
+#         elif rank == 2:
+#             X = sm.add_constant(x)
+#         elif rank == 3:
+#             X = sm.add_constant(np.column_stack((x, y)))
+# 
+#         # Hampel weighting function looks the most accurate for noisy data
+#         rlm_model = sm.RLM(z, X, M=sm.robust.norms.Hampel())
+#         rlm_results = rlm_model.fit()
+# 
+#         return rlm_results.params[:rank]
+
+#     # calculate MSE (optional)
+#     @staticmethod
+#     def robust_trend2d_mse(data, coeffs, rank):
+#         import numpy as np
+# 
+#         x = data[:, 0]
+#         y = data[:, 1]
+#         z_actual = data[:, 2]
+# 
+#         if rank == 1:
+#             z_predicted = coeffs[0]
+#         elif rank == 2:
+#             z_predicted = coeffs[0] + coeffs[1] * x
+#         elif rank == 3:
+#             z_predicted = coeffs[0] + coeffs[1] * x + coeffs[2] * y
+# 
+#         mse = np.mean((z_actual - z_predicted) ** 2)
+#         return mse
+
     @staticmethod
     def from_list(prm_list):
         from io import StringIO
         prm = StringIO('\n'.join(prm_list))
         return PRM._from_io(prm)
 
     @staticmethod
@@ -300,44 +349,47 @@
         rng = matrix[np.where(matrix[:,4]>SNR)][:,[0,2,1]]
         azi = matrix[np.where(matrix[:,4]>SNR)][:,[0,2,3]]
 
         # make sure there are enough points remaining
         if rng.shape[0] < 8:
             raise Exception(f'FAILED - not enough points to estimate parameters, try lower SNR ({rng.shape[0]} < 8)')
 
-        rng_coef = PRM.GMT_trend2d(rng, rank_rng)
-        azi_coef = PRM.GMT_trend2d(azi, rank_azi)
+        rng_coef = PRM.robust_trend2d(rng, rank_rng)
+        azi_coef = PRM.robust_trend2d(azi, rank_azi)
+
+        # print MSE (optional)
+        #rng_mse = PRM.robust_trend2d_mse(rng, rng_coef, rank_rng)
+        #azi_mse = PRM.robust_trend2d_mse(azi, azi_coef, rank_azi)
+        #print ('rng_mse_norm', rng_mse/len(rng), 'azi_mse_norm', azi_mse/len(azi))
 
         # range and azimuth data ranges
         scale_coef = [np.min(rng[:,0]), np.max(rng[:,0]), np.min(rng[:,1]), np.max(rng[:,1])]
 
-        rng_coef += scale_coef
-        azi_coef += scale_coef
-        #print ('rng_coef, rng_coef)
-        #print ('azi_coef, azi_coef)
+        #print ('rng_coef', rng_coef)
+        #print ('azi_coef', azi_coef)
 
         # now convert to range coefficients
-        rshift = rng_coef[0] - rng_coef[1]*(rng_coef[4]+rng_coef[3])/(rng_coef[4]-rng_coef[3]) \
-            - rng_coef[2]*(rng_coef[6]+rng_coef[5])/(rng_coef[6]-rng_coef[5])
+        rshift = rng_coef[0] - rng_coef[1]*(scale_coef[1]+scale_coef[0])/(scale_coef[1]-scale_coef[0]) \
+            - rng_coef[2]*(scale_coef[3]+scale_coef[2])/(scale_coef[3]-scale_coef[2])
         # now convert to azimuth coefficients
-        ashift = azi_coef[0] - azi_coef[1]*(azi_coef[4]+azi_coef[3])/(azi_coef[4]-azi_coef[3]) \
-            - azi_coef[2]*(azi_coef[6]+azi_coef[5])/(azi_coef[6]-azi_coef[5])
+        ashift = azi_coef[0] - azi_coef[1]*(scale_coef[1]+scale_coef[0])/(scale_coef[1]-scale_coef[0]) \
+            - azi_coef[2]*(scale_coef[3]+scale_coef[2])/(scale_coef[3]-scale_coef[2])
         #print ('rshift', rshift, 'ashift', ashift)
 
         # note: Python x % y expression and nympy results are different to C, use math function
         # use 'g' format for float values as in original GMTSAR codes to easy compare results
         prm = PRM().set(gformat=True,
                         rshift     =int(rshift) if rshift>=0 else int(rshift)-1,
                         sub_int_r  =math.fmod(rshift, 1)  if rshift>=0 else math.fmod(rshift, 1) + 1,
-                        stretch_r  =rng_coef[1]*2/(rng_coef[4]-rng_coef[3]),
-                        a_stretch_r=rng_coef[2]*2/(rng_coef[6]-rng_coef[5]),
+                        stretch_r  =rng_coef[1]*2/(scale_coef[1]-scale_coef[0]),
+                        a_stretch_r=rng_coef[2]*2/(scale_coef[3]-scale_coef[2]),
                         ashift     =int(ashift) if ashift>=0 else int(ashift)-1,
                         sub_int_a  =math.fmod(ashift, 1)  if ashift>=0 else math.fmod(ashift, 1) + 1,
-                        stretch_a  =azi_coef[1]*2/(azi_coef[4]-azi_coef[3]),
-                        a_stretch_a=azi_coef[2]*2/(azi_coef[6]-azi_coef[5]),
+                        stretch_a  =azi_coef[1]*2/(scale_coef[1]-scale_coef[0]),
+                        a_stretch_a=azi_coef[2]*2/(scale_coef[3]-scale_coef[2]),
                        )
 
         return prm
 
     def diff(self, other, gformat=True):
         """
         Compare to other dataframe and return difference
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2023.5.3/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_base.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,15 +165,16 @@
         # define subswath when subswath=None and check otherwise
         subswath = self.get_subswath(subswath)
     
         if pairs is None:
             # special case to open a single grid {name}.grd or a set of subswath grids Fn_{name}.grd
             pass
         elif isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
+            # convert to standalone DataFrame first
+            pairs = self.pairs(pairs)[['ref', 'rep']].astype(str).values
         else:
             pairs = np.asarray(pairs)
 
         if add_subswath == True:
             prefix = f'F{subswath}_'
         else:
             prefix = ''
@@ -274,15 +275,16 @@
             assert len(subswaths) == 1, 'ERROR: mask can be applied to a single subswath only'
             nanmask = xr.where((mask == 0)|(np.isnan(mask)), np.nan, 1)
 
         if pairs is None:
             # special case to open a single grid {name}.grd or a set of subswath grids Fn_{name}.grd
             pass
         elif isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
+            # convert to standalone DataFrame first
+            pairs = self.pairs(pairs)[['ref', 'rep']].astype(str).values
         else:
             pairs = np.asarray(pairs)
 
         def postprocess(da, subswath):
             masked = False
             if mask is not None and self.is_same(mask, da):
                 # apply mask when the mask defined in the same coordinates only
@@ -386,27 +388,53 @@
             # crop NaNs
             if crop_valid:
                 das = self.cropna(das)
             dass.append(das)
 
         return dass[0] if len(dass) == 1 else dass
 
+    # function is obsolete
     def find_pairs(self, name='phasefilt'):
+        print ('NOTE: use SBAS.pairs() wrapper function to get pairs as DataFrame and optionally dates array')        
+        pairs = self.pairs(name=name)
+        return pairs
+
+    # function is obsolete
+    def find_dates(self, pairs=None):
+        print ('NOTE: use SBAS.pairs() wrapper function to get pairs as DataFrame and optionally dates array')
+        dates = self.pairs(pairs, dates=True)[1]
+        return dates
+
+    def pairs(self, pairs=None, dates=False, name='phasefilt'):
+        import pandas as pd
         import numpy as np
         from glob import glob
 
-        # find all the intf grids
-        pattern = self.get_filenames(None, None, f'????????_????????_{name}')
-        filenames = glob(pattern, recursive=False)
-        pairs = [filename.split('_')[-3:-1] for filename in sorted(filenames)]
-        # return as numpy array for compatibility reasons
-        pairs = np.asarray(pairs)
-        # check that all the pairs produced from the SBAS scenes
-        dates = list(map(lambda x: x.replace('-',''), self.df.index))
-        invalid = [pair for pair in pairs.flatten() if pair not in dates]
-        assert len(invalid) == 0, 'ERROR: found grids for pairs not in the SBAS scenes. Define valid pairs manually.'
-        return pairs
+        if pairs is None:
+            # find all the named grids
+            pattern = self.get_filenames(None, None, f'????????_????????_{name}')
+            filenames = glob(pattern, recursive=False)
+            pairs = [filename.split('_')[-3:-1] for filename in sorted(filenames)]
+            # return as numpy array for compatibility reasons
+            pairs = np.asarray(pairs)
+            # check that all the pairs produced from the SBAS scenes
+            #dates = list(map(lambda x: x.replace('-',''), self.df.index))
+            #invalid = [pair for pair in pairs.flatten() if pair not in dates]
+            #assert len(invalid) == 0, 'ERROR: found grids for pairs not in the SBAS scenes. Define valid pairs manually.'
+
+        if not isinstance(pairs, pd.DataFrame):
+            # Convert numpy array to DataFrame
+            pairs = pd.DataFrame(pairs, columns=['ref', 'rep'])
+            # Convert ref and rep columns to datetime format
+            pairs['ref'] = pd.to_datetime(pairs['ref'])
+            pairs['rep'] = pd.to_datetime(pairs['rep'])
+            # Calculate the duration in days and add it as a new column
+            pairs['duration'] = (pairs['rep'] - pairs['ref']).dt.days
+        else:
+            # workaround for baseline_pairs() output
+            pairs = pairs.rename(columns={'ref_date': 'ref', 'rep_date': 'rep'})
 
-    def find_dates(self):
-        import numpy as np
-        pairs = self.find_pairs()
-        return np.unique(np.asarray(pairs).flatten())
+        if dates:
+            # pairs is DataFrame
+            dates = np.unique(pairs[['ref', 'rep']].astype(str).values.flatten())
+            return (pairs, dates)
+        return pairs
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_dem.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_dem_gmt_gdal.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_dem_gmt_gdal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_detrend.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_detrend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 #!/usr/bin/env python3
 # Alexey Pechnikov, Sep, 2021, https://github.com/mobigroup/gmtsar
 from .SBAS_unwrap import SBAS_unwrap
 
 class SBAS_detrend(SBAS_unwrap):
 
+    def detrend(self, dataarray, fit_intercept=True, fit_dem=True, fit_coords=True,
+            resolution_meters=90, wavelength=None, truncate=3.0, debug=False):
+
+        out1 = self._degaussian(dataarray, wavelength=wavelength, truncate=truncate,
+                                         resolution_meters=resolution_meters, debug=debug)
+        out2 = self._detrend(out1, fit_intercept=fit_intercept, fit_dem=fit_dem, fit_coords=fit_coords,
+                resolution_meters=resolution_meters, debug=debug)
+
+        return out2
+
     def detrend_parallel(self, pairs=None, n_jobs=-1, interactive=False, **kwargs):
         import dask
         import pandas as pd
         from tqdm.auto import tqdm
         import joblib
 
-        if pairs is None:
-            pairs = self.find_pairs()
-        elif isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
+        # convert pairs (list, array, dataframe) to 2D numpy array
+        pairs = self.pairs(pairs)[['ref', 'rep']].astype(str).values
 
         def func(pair, **kwargs):
             #print (f'**kwargs {kwargs}')
-            grid = self.open_grids([pair], 'unwrap', interactive=False)
-
-            # without any processing options return the input as is
-            out = grid[0]
-
-            if 'wavelength' in kwargs:
-                kwargs1 = {k:v for k,v in kwargs.items() if k in ['wavelength', 'truncate', 'resolution_meters', 'debug']}
-                #print (f'kwargs1 {kwargs1}')
-                out = self.degaussian(out, **kwargs1)
-
-            kwargs2 = {k:v for k,v in kwargs.items() if k in ['fit_intercept', 'fit_dem', 'fit_coords',
-                                                              'resolution_meters', 'debug']}
-            #print (f'kwargs2 {kwargs2}')
+            grid = self.open_grids([pair], 'unwrap', interactive=False)[0]
             # ignore detrending when all the fits are disabled
-            out = self.detrend(out, **kwargs2)
-
+            out = self.detrend(grid, **kwargs)
             if interactive:
                 return out
-
             # prepare pipeline for processing and saving
             delayed = self.save_grids([out], 'detrend', interactive=False)
-
             # perform the pipeline
             dask.persist(delayed)
 
         label = 'Detrending and Saving' if not interactive else 'Detrending'
         with self.tqdm_joblib(tqdm(desc=label, total=len(pairs))) as progress_bar:
             results = joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(func)(pair, **kwargs) for pair in pairs)
         
         if interactive:
             return results
 
-    def detrend(self, dataarray, fit_intercept=True, fit_dem=True, fit_coords=True,
+    def _detrend(self, dataarray, fit_intercept=True, fit_dem=True, fit_coords=True,
                 resolution_meters=90, debug=False):
         """
         Detrend unwrapped interferogram in radar coordinates, see for details
             https://github.com/gmtsar/gmtsar/issues/98
             https://github.com/gmtsar/gmtsar/issues/411
         """
         import xarray as xr
@@ -100,83 +93,83 @@
             if debug:
                 print ('DEBUG: Decimated topography array', topo_dec.shape)
         else:
             topo = topo_dec = None
 
         # lazy calculations are useless below
         def data2fit(data, elev, yy, xx):
-            y = data.reshape(-1)
+            y = data.values.reshape(-1) if isinstance(data, xr.DataArray) else data.reshape(-1)
             nanmask = np.isnan(y)
             # prepare regression variable
             Y = y[~nanmask]
 
             if fit_coords or fit_dem:
                 # prepare coordinates for X regression variable
-                ys = yy.reshape(-1)[~nanmask]
-                xs = xx.reshape(-1)[~nanmask]
+                ys = (yy.values.reshape(-1) if isinstance(yy, xr.DataArray) else yy.reshape(-1))[~nanmask]
+                xs = (xx.values.reshape(-1) if isinstance(xx, xr.DataArray) else xx.reshape(-1))[~nanmask]
 
             if fit_dem:
                 # prepare topography for X regression variable
-                zs = elev.reshape(-1)[~nanmask]
+                zs = (elev.values.reshape(-1) if isinstance(elev, xr.DataArray) else elev.reshape(-1))[~nanmask]
                 zys = zs*ys
                 zxs = zs*xs
 
             if fit_dem and fit_coords:
                 X = np.column_stack([zys, zxs, ys, xs, zs])
             elif fit_dem:
                 X = np.column_stack([zys, zxs, zs])
             elif fit_coords:
                 X = np.column_stack([ys, xs])
             return Y, X, nanmask
 
         if debug:
             print ('DEBUG: linear regression calculation')
-    
+
         def regr_fit():
             # build prediction model with or without plane removal (fit_intercept)
             regr = make_pipeline(StandardScaler(), LinearRegression(fit_intercept=fit_intercept))
             yy, xx = xr.broadcast(dataarray_dec.y, dataarray_dec.x)
-            Y, X, _ = data2fit(dataarray_dec.values, topo_dec.values, yy.values, xx.values)
-        
+            Y, X, _ = data2fit(dataarray_dec, topo_dec, yy, xx)
+
             return regr.fit(X, Y)
-    
+
         # calculate for chunks
         def predict(data, elev, yy, xx, regr):
             Y, X, nanmask = data2fit(data, elev, yy, xx)
             # the chunk is NaN-filled, prediction impossible
             if nanmask.all():
                 return data
             # predict when some values are not NaNs
             model = np.nan * np.zeros(data.shape)
             model.reshape(-1)[~nanmask] = regr.predict(X)
             # return data without the trend
             return data - model
-    
+
         def regr_predict(regr):
             yy = xr.DataArray(dataarray.y).chunk(-1)
             xx = xr.DataArray(dataarray.x).chunk(-1)
             yy, xx = xr.broadcast(yy, xx)
 
             # xarray wrapper
             return xr.apply_ufunc(
                 predict,
                 dataarray,
-                topo.chunk(dataarray.chunks),
+                topo.chunk(dataarray.chunks) if topo is not None else None,
                 yy.chunk(dataarray.chunks),
                 xx.chunk(dataarray.chunks),
                 dask='parallelized',
                 vectorize=False,
                 output_dtypes=[np.float32],
                 dask_gufunc_kwargs={'regr': regr},
             )
-    
+
         # build the model and return the input data without the detected trend
         return postprocessing(regr_predict(regr_fit()))
 
-    def degaussian(self, dataarray, wavelength, truncate=3.0, resolution_meters=90, debug=False):
+    def _degaussian(self, dataarray, wavelength, truncate=3.0, resolution_meters=90, debug=False):
         """
         Lazy Gaussian filter for arrays with NaN values.
             dataarray - input dataarray with NaNs allowed,
             wavelength - cut-off wavelength [m],
             truncate - filter window size [sigma],
             resolution_meters - Gaussian filter processing resolution [m],
             debug - print debug information.
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_geocode.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_geocode.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from .SBAS_sbas import SBAS_sbas
 from .tqdm_dask import tqdm_dask
 
 class SBAS_geocode(SBAS_sbas):
 
     def geocode_parallel(self, pairs=None):
         # find any one interferogram to build the geocoding matrices
-        if pairs is None:
-            pairs = self.find_pairs()
+        pairs = self.pairs(pairs)
+        
         # build trans_dat and topo_ra grids
         self.topo_ra_parallel()
         # define the target interferogram grid
         intf_grid = self.open_grids(pairs, 'phasefilt').min('pair').astype(bool)
         # build geographic coordinates transformation matrix for landmask and other grids
         self.intf_ll2ra_matrix_parallel(intf_grid)
         # build radar coordinates transformation matrix for the interferograms grid stack
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_incidence.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_intf.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_intf.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def intf_parallel(self, pairs, n_jobs=-1, **kwargs):
         import pandas as pd
         import numpy as np
         from tqdm.auto import tqdm
         import joblib
         import os
 
-        if isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
+        # convert pairs (list, array, dataframe) to 2D numpy array
+        pairs = self.pairs(pairs)[['ref', 'rep']].astype(str).values
 
         subswaths = self.get_subswaths()
 
         # for now (Python 3.10.10 on MacOS) joblib loads the code from disk instead of copying it
         kwargs['chunksize'] = self.chunksize
         
         # this way does not work properly for long interferogram series on MacOS
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_landmask.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_landmask_gmt.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_landmask_gmt.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_merge.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 
         # merging is not applicable to a single subswath
         # for this case coordinate transformation matrices already built in SBAS.intf_parallel()
         subswaths = self.get_subswaths()
         if len(subswaths) == 1:
             return
         
-        if isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
+        # convert pairs (list, array, dataframe) to 2D numpy array
+        pairs = self.pairs(pairs)[['ref', 'rep']].astype(str).values
 
         with self.tqdm_joblib(tqdm(desc=f'Merging Subswaths', total=len(pairs)*len(grids))) as progress_bar:
             joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(self.merge)(pair, grid, **kwargs) \
                                            for pair in pairs for grid in grids)
 
         df = self.df.groupby(self.df.index).agg({'datetime': min, 'orbit': min, 'mission': min, 'polarization':min,
                                             'subswath': lambda s: int(''.join(map(str,list(s)))),
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_merge_gmtsar.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_merge_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_orbits.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_reframe.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_reframe_gmtsar.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_sbas.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_sbas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,240 +1,282 @@
 #!/usr/bin/env python3
 # Alexey Pechnikov, Sep, 2021, https://github.com/mobigroup/gmtsar
 from .SBAS_sbas_gmtsar import SBAS_sbas_gmtsar
 from .PRM import PRM
+from .tqdm_dask import tqdm_dask
 
 class SBAS_sbas(SBAS_sbas_gmtsar):
 
-    def baseline_table(self, n_jobs=-1, debug=False):
-        import pandas as pd
+    # single-pixel processing function
+    # compute least squares when w = None and weighted least squares otherwise
+    @staticmethod
+    def lstsq(x, w, matrix):
         import numpy as np
-        from tqdm.auto import tqdm
-        import joblib
-        import os
 
-        # use any subswath (the 1st one here) to produce the table
-        subswath = self.get_subswaths()[0]
-        datetimes = self.df[self.df.subswath==subswath].datetime
-
-        def get_filename(dt):
-            _, stem = self.multistem_stem(subswath, dt)
-            filename = os.path.join(self.basedir, f'{stem}.PRM')
-            return filename
-    
-        def ondemand(date, dt):
-            if not os.path.exists(get_filename(dt)):
-                self.make_s1a_tops(subswath, date, debug=debug)
+        if w is None:
+            # allow not weighted Least Squares
+            w = 0.5 * np.ones_like(x)
+        elif np.any(np.isnan(w)):
+            # ignore pixels where correlation is not defined
+            return np.nan * np.zeros(matrix.shape[1])
 
-        # generate PRM, LED if needed
-        #for (date, dt) in datetimes.iteritems():
-        #    #print (dt, date)
-        #    ondemand(dt)
-        with self.tqdm_joblib(tqdm(desc='PRM generation', total=len(datetimes))) as progress_bar:
-            joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(ondemand)(date, dt) for (date, dt) in datetimes.items())
-    
-        # after merging use unmerged subswath PRM files
-        # calc_dop_orb() required for SAT_baseline
-        master_dt = datetimes[self.master]
-        prm_ref = PRM().from_file(get_filename(master_dt)).calc_dop_orb(inplace=True)
-        data = []
-        for (date, dt) in datetimes.items():
-            # after merging use unmerged subswath PRM files
-            prm_rep = PRM().from_file(get_filename(dt))
-            ST0 = prm_rep.get('SC_clock_start')
-            DAY = int(ST0 % 1000)
-            YR = int(ST0/1000) - 2014
-            YDAY = YR * 365 + DAY
-            #print (f'YR={YR}, DAY={DAY}')
-            BPL, BPR = prm_ref.SAT_baseline(prm_rep).get('B_parallel', 'B_perpendicular')
-            data.append({'date':date, 'ST0':ST0, 'YDAY':YDAY, 'BPL':BPL, 'BPR':BPR})
-            #print (date, ST0, YDAY, BPL, BPR)
-        return pd.DataFrame(data).set_index('date')
+        # fill nans as zeroes and set corresponding weight to 0
+        nanmask = np.where(np.isnan(x))
+        if nanmask[0].size > 0:
+            # function arguments are read-only
+            x = x.copy()
+            w = w.copy()
+            x[nanmask] = 0
+            w[nanmask] = 0
+            # check if x has enough valid values
+            if x.size - nanmask[0].size < matrix.shape[1]:
+                return np.nan * np.zeros(matrix.shape[1])
+        try:
+            if np.all(w == 1):
+                # least squares solution
+                model = np.linalg.lstsq(matrix, x, rcond=None)
+            else:
+                # weighted least squares solution
+                W = (w/np.sqrt(1-w**2))
+                model = np.linalg.lstsq(matrix * W[:,np.newaxis], x * W, rcond=None)
+        except Exception as e:
+            # typically, this error handled:
+            # LinAlgError: SVD did not converge in Linear Least Squares
+            print ('SBAS.lstsq notice:', str(e))
+            return np.nan * np.zeros(matrix.shape[1])
+        #print ('model', model)
+        return model[0]
 
-    # returns sorted baseline pairs
-    def baseline_pairs(self, days=100, meters=150, invert=False, n_jobs=-1, debug=False):
+    def lstsq_matrix(self, pairs):
         import numpy as np
         import pandas as pd
-     
-        tbl = self.baseline_table(n_jobs=n_jobs, debug=debug)
-        data = []
-        for line1 in tbl.itertuples():
-            for line2 in tbl.itertuples():
-                #print (line1, line2)
-                if not (line1.YDAY < line2.YDAY and line2.YDAY - line1.YDAY < days):
-                    continue
-                if not (abs(line1.BPR - line2.BPR)< meters):
-                    continue
 
-                if not invert:
-                    data.append({'ref_date':line1.Index, 'rep_date': line2.Index,
-                                 'ref_timeline': np.round(line1.YDAY/365.25+2014, 2), 'ref_baseline': np.round(line1.BPR, 2),
-                                 'rep_timeline': np.round(line2.YDAY/365.25+2014, 2), 'rep_baseline': np.round(line2.BPR, 2)})
-                else:
-                    data.append({'ref_date':line2.Index, 'rep_date': line1.Index,
-                                 'ref_timeline': np.round(line2.YDAY/365.25+2014, 2), 'ref_baseline': np.round(line2.BPR, 2),
-                                 'rep_timeline': np.round(line1.YDAY/365.25+2014, 2), 'rep_baseline': np.round(line1.BPR, 2)})
+        # also define image capture dates from interferogram date pairs 
+        pairs, dates = self.pairs(pairs, dates=True)
+        pairs = pairs[['ref', 'rep']].astype(str).values
+        
+        # here are one row for every interferogram and one column for every date
+        matrix = []
+        for pair in pairs:
+            mrow = [date>pair[0] and date<=pair[1] for date in dates]
+            matrix.append(mrow)
+        matrix = np.stack(matrix).astype(int)
+        return matrix
 
-        return pd.DataFrame(data).sort_values(['ref_date', 'rep_date'])
+    def sbas_parallel(self, pairs=None, mask=None, data='detrend', corr='corr', weight='corr',
+                      chunks=None, chunksize=None, n_jobs=-1, interactive=False):
 
-    def sbas_parallel(self, pairs=None, mask=None, data='detrend', corr='corr', chunks=None, chunksize=None, n_jobs=-1):
+        print ('NOTE: sbas_parallel() is alias for [Weighted] Least Squares lstsq_parallel() function')
+
+        if corr != 'corr':
+            print ('NOTE: use "weight" argument instead of "corr"')
+
+        if mask is not None:
+            print ('NOTE: "mask" argument support is removed. Use "data" and "weight" arguments to call with custom data arrays')
+
+        if chunks is not None:
+            print ('NOTE: use "chunksize" argument instead of "chunks"')
+            
+        return self.lstsq_parallel(pairs=pairs, data=data, weight=weight,
+                                   chunksize=chunksize, n_jobs=n_jobs, interactive=interactive)
+                   
+    def lstsq_parallel(self, pairs=None, data='detrend', weight='corr',
+                       chunksize=None, n_jobs=-1, interactive=False):
         import xarray as xr
         import numpy as np
         import pandas as pd
+        import dask
         from tqdm.auto import tqdm
         import joblib
         import os
-        
-        if chunks is not None:
-            print ('NOTE: use "chunksize" argument instead of "chunks"')
-            chunksize = chunks
+
         if chunksize is None:
+            # smaller chunks are better for large 3D grids processing
             chunksize = self.chunksize
+        #print ('chunksize', chunksize)
+
+        # also define image capture dates from interferogram date pairs 
+        # convert pairs (list, array, dataframe) to 2D numpy array
+        pairs, dates = self.pairs(pairs, dates=True)
+        pairs = pairs[['ref', 'rep']].astype(str).values
+        
+        # split large stacks to chunks about chunksize ^ 3
+        minichunksize = chunksize**2 / len(pairs)
+        # round to 2**deg (32,  64, 128,..., 2048)
+        chunkdegrees = np.array([2**deg for deg in range(5,12) if 2**deg <= chunksize])
+        minichunksize = int(chunkdegrees[np.abs(chunkdegrees-minichunksize).argmin()])
+        #print ('minichunksize', minichunksize)
 
-        # compress 3d output following the processing blocks
-        netcdf_compression = self.compression()
-        netcdf_compression['chunksizes'] = (1, chunksize, chunksize)
-
-        if pairs is None:
-            pairs = self.find_pairs()
-        elif isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
-        else:
-            pairs = np.asarray(pairs)
-        # define all the dates as unique reference and repeat dates
-        dates = np.unique(pairs.flatten())
-    
         # source grids lazy loading
-        if isinstance(corr, str):
-            corr = self.open_grids(pairs, corr, chunksize=chunksize, interactive=False)
         if isinstance(data, str):
-            data = self.open_grids(pairs, data, chunksize=chunksize, interactive=False)
-
-        # crop correlation grid like to unwrap grid which may be defined smaller
-        corr = corr.reindex_like(data)
-        
-        # mask can be sparse and limit work area
-        if mask is not None:
-            data = xr.where(mask>0, data.reindex_like(mask), np.nan)
-            corr   = xr.where(mask>0, corr.reindex_like(mask),   np.nan)
-    
-        # here are one row for every interferogram and one column for every date
-        matrix = []
-        for pair in pairs:
-            mrow = [date>pair[0] and date<=pair[1] for date in dates]
-            matrix.append(mrow)
-        matrix = np.stack(matrix).astype(int)
+            data = self.open_grids(pairs, data, chunksize=minichunksize, interactive=True)
 
-        # single-pixel processing function
-        def fit(x, w, matrix):
-            #return np.zeros(5)
-            # ignore pixels where correlation is not defined
-            if np.any(np.isnan(w)):
-                return np.nan * np.zeros(matrix.shape[1])
-            # fill nans as zeroes and set corresponding weight to 0
-            nanmask = np.where(np.isnan(x))
-            if nanmask[0].size > 0:
-                # function arguments are read-only
-                x = x.copy()
-                w = w.copy()
-                x[nanmask] = 0
-                w[nanmask] = 0
-                # check if x has enough valid values
-                if x.size - nanmask[0].size < matrix.shape[1]:
-                    return np.nan * np.zeros(matrix.shape[1])
-            # least squares solution
-            W = (w/np.sqrt(1-w**2))
-            model = np.linalg.lstsq(matrix * W[:,np.newaxis], x * W, rcond=None)
-            #print ('model', model)
-            return model[0]
+        if isinstance(weight, str):
+            weight = self.open_grids(pairs, weight, chunksize=minichunksize, interactive=True)
+        elif isinstance(weight, (pd.Series, np.ndarray)):
+            # vector weight like to average correlation
+            weight = xr.DataArray(weight, dims=['pair'], coords={'pair': data.pair})
 
         # xarray wrapper
-        models = xr.apply_ufunc(
-            fit,
+        model = xr.apply_ufunc(
+            self.lstsq,
             data.chunk(dict(pair=-1)),
-            corr.chunk(dict(pair=-1)),
-            input_core_dims=[['pair'],['pair']],
+            weight.chunk(dict(pair=-1)) if weight is not None else None,
+            input_core_dims=[['pair'], ['pair'] if weight is not None else []],
             exclude_dims=set(('pair',)),
             dask='parallelized',
             vectorize=True,
             output_dtypes=[np.float32],
             output_core_dims=[['date']],
             dask_gufunc_kwargs={'output_sizes': {'date': len(dates)}},
-            kwargs={'matrix': matrix}
-        )
+            kwargs={'matrix': self.lstsq_matrix(pairs)}
+        ).rename('displacement')
         # define dates axis
-        models['date'] = dates
+        model['date'] = dates
         # set the stack index to be first
-        models = models.transpose('date',...)
-        # define the output grid filename
-        model_filename = self.get_filenames(None, None, 'disp')
-        # cleanup
-        if os.path.exists(model_filename):
-            os.remove(model_filename)
-    
-        ts, ys, xs = models.data.blocks.shape
+        model = model.transpose('date',...)
+
+        if interactive:
+            return model
+
+        # use this trick to save large model using limited RAM and all CPU cores
+        ts, ys, xs = model.data.blocks.shape
         assert ts == 1, 'Date chunks count should be equal to 1'
-        tchunks, ychunks, xchunks = models.chunks
-        coordt = models.date
-        coordy = np.array_split(models.y, np.cumsum(ychunks))
-        coordx = np.array_split(models.x, np.cumsum(xchunks))
-    
+        tchunks, ychunks, xchunks = model.chunks
+        coordt = model.date
+        coordy = np.array_split(model.y, np.cumsum(ychunks))
+        coordx = np.array_split(model.x, np.cumsum(xchunks))
+
         def func(iy, ix):
             chunk_filename = self.get_filenames(None, None, f'disp_chunk_{iy}_{ix}')
             if os.path.exists(chunk_filename):
                 os.remove(chunk_filename)
             # lazy dask array
-            data = models.data.blocks[0,iy,ix]
+            data = model.data.blocks[0,iy,ix]
             # wrap the array
             da = xr.DataArray(data,
                               dims=['date','y','x'],
                               coords={'date': coordt, 'y':coordy[iy], 'x':coordx[ix]})\
                  .rename('displacement')
+            # compress 3d output following the processing blocks
+            netcdf_compression = self.compression()
+            # use model chunks as is for better performance
+            netcdf_compression['chunksizes'] = (1, minichunksize, minichunksize)
             # compute and save to NetCDF using chunks of original coordinates
             da.to_netcdf(chunk_filename,
                          unlimited_dims=['y','x'],
                          encoding={'displacement': netcdf_compression},
                          engine=self.engine,
                          compute=True)
             return chunk_filename
-    
-        # process all the chunks
-        with self.tqdm_joblib(tqdm(desc='Computing', total=ys*xs)) as progress_bar:
+
+        # process the chunks as separate tasks on all available CPU cores
+        with self.tqdm_joblib(tqdm(desc='[Correlation-Weighted] Least Squares Computing', total=ys*xs)) as progress_bar:
             filenames = joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(func)(iy, ix) \
                                                      for iy in range(ys) for ix in range(xs))
-    
+
         # rebuild the datasets to user-friendly format
         das = [xr.open_dataarray(f, engine=self.engine, chunks=chunksize) for f in filenames]
-        if xr.__version__ == '0.19.0':
-            # for Google Colab
-            das = xr.merge(das)
-        else:
-            # for modern xarray versions
-            das = xr.combine_by_coords(das)
-
-        # add subswath prefix
-        subswath = self.get_subswath()
+        das = xr.combine_by_coords(das)
 
         def output(dt):
-            filename = os.path.join(self.basedir, f'F{subswath}_disp_{dt}.grd'.replace('-',''))
+            filename = self.get_filenames(None, None, f'disp_{dt}'.replace('-',''))
             if os.path.exists(filename):
                 os.remove(filename)
+            # compress 3d output following the processing blocks
+            netcdf_compression = self.compression()
+            netcdf_compression['chunksizes'] = (chunksize, chunksize)
             das.sel(date=dt).to_netcdf(filename,
-                        encoding={'displacement': self.compression()},
+                        encoding={'displacement': netcdf_compression},
                         engine=self.engine)
 
         # saving all the grids
         with self.tqdm_joblib(tqdm(desc='Saving', total=len(das.date))) as progress_bar:
             joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(output)(dt) for dt in das.date.values)
 
         # cleanup
         for filename in filenames:
             if os.path.exists(filename):
                 os.remove(filename)
 
+    def baseline_table(self, n_jobs=-1, debug=False):
+        import pandas as pd
+        import numpy as np
+        from tqdm.auto import tqdm
+        import joblib
+        import os
+
+        # use any subswath (the 1st one here) to produce the table
+        subswath = self.get_subswaths()[0]
+        datetimes = self.df[self.df.subswath==subswath].datetime
+
+        def get_filename(dt):
+            _, stem = self.multistem_stem(subswath, dt)
+            filename = os.path.join(self.basedir, f'{stem}.PRM')
+            return filename
+    
+        def ondemand(date, dt):
+            if not os.path.exists(get_filename(dt)):
+                self.make_s1a_tops(subswath, date, debug=debug)
+
+        # generate PRM, LED if needed
+        #for (date, dt) in datetimes.iteritems():
+        #    #print (dt, date)
+        #    ondemand(dt)
+        with self.tqdm_joblib(tqdm(desc='PRM generation', total=len(datetimes))) as progress_bar:
+            joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(ondemand)(date, dt) for (date, dt) in datetimes.items())
+    
+        # after merging use unmerged subswath PRM files
+        # calc_dop_orb() required for SAT_baseline
+        master_dt = datetimes[self.master]
+        prm_ref = PRM().from_file(get_filename(master_dt)).calc_dop_orb(inplace=True)
+        data = []
+        for (date, dt) in datetimes.items():
+            # after merging use unmerged subswath PRM files
+            prm_rep = PRM().from_file(get_filename(dt))
+            ST0 = prm_rep.get('SC_clock_start')
+            DAY = int(ST0 % 1000)
+            YR = int(ST0/1000) - 2014
+            YDAY = YR * 365 + DAY
+            #print (f'YR={YR}, DAY={DAY}')
+            BPL, BPR = prm_ref.SAT_baseline(prm_rep).get('B_parallel', 'B_perpendicular')
+            data.append({'date':date, 'ST0':ST0, 'YDAY':YDAY, 'BPL':BPL, 'BPR':BPR})
+            #print (date, ST0, YDAY, BPL, BPR)
+        return pd.DataFrame(data).set_index('date')
+
+    # returns sorted baseline pairs
+    def baseline_pairs(self, days=100, meters=150, limit=None, invert=False, n_jobs=-1, debug=False):
+        import numpy as np
+        import pandas as pd
+
+        tbl = self.baseline_table(n_jobs=n_jobs, debug=debug)
+        data = []
+        for line1 in tbl.itertuples():
+            counter = 0
+            for line2 in tbl.itertuples():
+                #print (line1, line2)
+                if limit is not None and counter >= limit:
+                    continue
+                if not (line1.YDAY < line2.YDAY and line2.YDAY - line1.YDAY < days):
+                    continue
+                if not (abs(line1.BPR - line2.BPR)< meters):
+                    continue
+
+                counter += 1
+                if not invert:
+                    data.append({'ref_date':line1.Index, 'rep_date': line2.Index,
+                                 'ref_timeline': np.round(line1.YDAY/365.25+2014, 2), 'ref_baseline': np.round(line1.BPR, 2),
+                                 'rep_timeline': np.round(line2.YDAY/365.25+2014, 2), 'rep_baseline': np.round(line2.BPR, 2)})
+                else:
+                    data.append({'ref_date':line2.Index, 'rep_date': line1.Index,
+                                 'ref_timeline': np.round(line2.YDAY/365.25+2014, 2), 'ref_baseline': np.round(line2.BPR, 2),
+                                 'rep_timeline': np.round(line1.YDAY/365.25+2014, 2), 'rep_baseline': np.round(line1.BPR, 2)})
+
+        return pd.DataFrame(data).sort_values(['ref_date', 'rep_date'])
+
     #intf.tab format:   unwrap.grd  corr.grd  ref_id  rep_id  B_perp 
     def intftab(self, baseline_pairs):
         import numpy as np
         import datetime
 
         # return a single subswath for None
         subswath = self.get_subswath()
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_sbas_gmtsar.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_sbas_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_stack.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_topo_ra.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_topo_ra.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_trans.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_unwrap.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,17 @@
         def unwrap_tiledir(pair, **kwargs):
             # define unique tiledir name for parallel processing
             if 'conf' in kwargs:
                 dirpath = self.get_filenames(None, [pair], 'snaphu_tiledir')[0][:-4]
                 kwargs['conf'] += f'    TILEDIR {dirpath}'
             return self.unwrap(pair, **kwargs)
 
-        if pairs is None:
-            pairs = self.find_pairs()
-        elif isinstance(pairs, pd.DataFrame):
-            pairs = pairs.values
-
+        # convert pairs (list, array, dataframe) to 2D numpy array
+        pairs = self.pairs(pairs)[['ref', 'rep']].astype(str).values
+        
         # materialize lazy mask
         if mask is not None and isinstance(mask, xr.DataArray):
             mask_filename = self.get_filenames(None, None, 'unwrapmask')
             if os.path.exists(mask_filename):
                 os.remove(mask_filename)
             # workaround to save NetCDF file correct
             mask.rename('mask').rename({'y':'a','x':'r'}).\
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/SBAS_unwrap_snaphu.py` & `pygmtsar-2023.5.3/pygmtsar/SBAS_unwrap_snaphu.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,49 +7,58 @@
     # -s for SMOOTH mode and -d for DEFO mode when DEFOMAX_CYCLE should be defined in the configuration
     # DEFO mode (-d) and DEFOMAX_CYCLE=0 is equal to SMOOTH mode (-s)
     # https://web.stanford.edu/group/radar/softwareandlinks/sw/snaphu/snaphu_man1.html
     def unwrap(self, pair, threshold=1e-3, conf=None, func=None, mask=None, conncomp=False,
                phase='phasefilt', corr='corr', interactive=True, chunksize=None, debug=False):
         import xarray as xr
         import numpy as np
+        import pandas as pd
         import os
         import subprocess
 
+        # convert to 2D single-element array
+        if isinstance(pair, pd.DataFrame):
+            # DataFrame can 
+            assert len(pair) == 1, 'Only single-record DataFrame or 1 D or 2D pair of dates allowed'
+            pair = self.pairs(pair)[['ref','rep']].astype(str).values
+        else:
+            pair = [pair] if np.asarray(pair).ndim == 1 else pair
+
         # define lost class variables due to joblib
         if chunksize is None:
             chunksize = self.chunksize
 
         if conf is None:
             conf = self.PRM().snaphu_config()
-    
+
         # open input data grids if needed
         if isinstance(phase, str):
-            phase = self.open_grids([pair], phase, chunksize=chunksize, interactive=False)[0]
+            phase = self.open_grids(pair, phase, chunksize=chunksize, interactive=False)[0]
         if isinstance(corr, str):
-            corr = self.open_grids([pair], corr, chunksize=chunksize, interactive=False)[0]
+            corr = self.open_grids(pair, corr, chunksize=chunksize, interactive=False)[0]
         if mask is not None and isinstance(mask, str):
             mask = self.open_grids(None, mask, chunksize=chunksize, interactive=False)
-        
+
         # convert user-defined mask to boolean mask (NaN values converted to 0)
         if mask is not None:
             assert self.is_ra(mask), 'ERROR: mask should be defined in radar coordinates'
             # define mask on the same grid as phase and convert to boolean
             binmask = xr.where(mask>0, 1, 0).astype(bool)
             # unify grids to maybe smallest mask
             phase = phase.reindex_like(mask)
             corr = corr.reindex_like(mask)
         else:
             binmask = 1
         # add threshold mask
         binmask = binmask & (corr>=threshold)
 
         # extract dates from pair
-        date1, date2 = pair
+        date1, date2 = pair[0]
 
-        basename = self.get_filenames(None, [pair], '')[0][:-4]
+        basename = self.get_filenames(None, pair, '')[0][:-4]
         #print ('basename', basename)
 
         # output data grids
         unwrap_filename = basename + 'unwrap.grd'
         conncomp_filename = basename + 'conncomp.grd'
         # SNAPHU input files
         phase_in = basename + 'unwrap.phase'
@@ -98,21 +107,23 @@
             values = np.fromfile(conncomp_out, dtype=np.ubyte).reshape(phase.shape)
             conn = xr.DataArray(values, phase.coords, name='conncomp').chunk(chunksize)
 
         # convert to grid unwrapped phase from SNAPHU output applying postprocessing
         values = np.fromfile(unwrap_out, dtype=np.float32).reshape(phase.shape)
         #values = np.frombuffer(stdout_data, dtype=np.float32).reshape(phase.shape)
         unwrap = xr.DataArray(values, phase.coords).chunk(chunksize)
+        # NaN values allowed in the output grid, assign userfriendly name for the output grid
+        unwrap = unwrap.where(binmask)
         # apply user-defined function for post-processing
         if func is not None:
             # the both grids should have the right chunksize
-            unwrap = func(corr.where(binmask), unwrap)
-        # apply binary mask after the post-processing to completely exclude masked regions
-        # NaN values allowed in the output grid, assign userfriendly name for the output grid
-        unwrap = unwrap.where(binmask).rename('phase')
+            # mask invalid area on correlation grid
+            unwrap = func(corr, unwrap).where(~np.isnan(corr))
+        # rename after all the processing
+        unwrap = unwrap.rename('phase')
 
         # the output files required for interactive output
         for tmp_file in [phase_in, corr_in] + [unwrap_out, conncomp_out] if not interactive else []:
             if os.path.exists(tmp_file):
                 if debug:
                     print ('DEBUG: remove', tmp_file)
                 os.remove(tmp_file)
```

### Comparing `pygmtsar-2023.4.20/pygmtsar/datagrid.py` & `pygmtsar-2023.5.3/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/tqdm_dask.py` & `pygmtsar-2023.5.3/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar/tqdm_joblib.py` & `pygmtsar-2023.5.3/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2023.5.3/pygmtsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2023.4.20
+Version: 2023.5.3
 Summary: PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone
 Home-page: https://github.com/mobigroup/gmtsar
 Author: Alexey Pechnikov
 Author-email: pechnikov@mobigroup.ru
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2023.4.20/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2023.5.3/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2023.4.20/setup.py` & `pygmtsar-2023.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pygmtsar',
-    version='2023.4.20',
+    version='2023.5.3',
     description='PyGMTSAR (Python GMTSAR) - Easy and Fast Satellite Interferometry For Everyone',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mobigroup/gmtsar',
     author='Alexey Pechnikov',
     author_email='pechnikov@mobigroup.ru',
     license='BSD-3-Clause',
```

