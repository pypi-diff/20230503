# Comparing `tmp/csst-ifs-gehong-0.0.1.4.tar.gz` & `tmp/csst-ifs-gehong-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csst-ifs-gehong-0.0.1.4.tar", last modified: Wed May  3 06:40:52 2023, max compression
+gzip compressed data, was "csst-ifs-gehong-0.0.1.5.tar", last modified: Wed May  3 12:15:02 2023, max compression
```

## Comparing `csst-ifs-gehong-0.0.1.4.tar` & `csst-ifs-gehong-0.0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 06:40:52.659228 csst-ifs-gehong-0.0.1.4/
--rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.4/LICENSE
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-03 06:40:52.659303 csst-ifs-gehong-0.0.1.4/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.4/README.md
--rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-03 06:40:52.659593 csst-ifs-gehong-0.0.1.4/setup.cfg
--rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-03 06:40:48.000000 csst-ifs-gehong-0.0.1.4/setup.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 06:40:52.656468 csst-ifs-gehong-0.0.1.4/src/
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 06:40:52.657896 csst-ifs-gehong-0.0.1.4/src/csst_ifs_gehong.egg-info/
--rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-03 06:40:52.000000 csst-ifs-gehong-0.0.1.4/src/csst_ifs_gehong.egg-info/PKG-INFO
--rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-03 06:40:52.000000 csst-ifs-gehong-0.0.1.4/src/csst_ifs_gehong.egg-info/SOURCES.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-03 06:40:52.000000 csst-ifs-gehong-0.0.1.4/src/csst_ifs_gehong.egg-info/dependency_links.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-03 06:40:52.000000 csst-ifs-gehong-0.0.1.4/src/csst_ifs_gehong.egg-info/requires.txt
--rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-03 06:40:52.000000 csst-ifs-gehong-0.0.1.4/src/csst_ifs_gehong.egg-info/top_level.txt
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 06:40:52.658603 csst-ifs-gehong-0.0.1.4/src/gehong/
--rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.4/src/gehong/__init__.py
--rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.4/src/gehong/config.py
--rw-r--r--   0 sfeng      (501) staff       (20)     3591 2023-05-03 04:54:26.000000 csst-ifs-gehong-0.0.1.4/src/gehong/cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-03 04:45:44.000000 csst-ifs-gehong-0.0.1.4/src/gehong/map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    37322 2023-05-03 01:19:30.000000 csst-ifs-gehong-0.0.1.4/src/gehong/spec1d.py
-drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 06:40:52.659089 csst-ifs-gehong-0.0.1.4/test/
--rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.4/test/test_cube3d.py
--rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.4/test/test_map2d.py
--rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.4/test/test_spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.489448 csst-ifs-gehong-0.0.1.5/
+-rw-r--r--   0 sfeng      (501) staff       (20)     1073 2023-04-25 01:31:05.000000 csst-ifs-gehong-0.0.1.5/LICENSE
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-03 12:15:02.489538 csst-ifs-gehong-0.0.1.5/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      244 2023-04-26 13:40:59.000000 csst-ifs-gehong-0.0.1.5/README.md
+-rw-r--r--   0 sfeng      (501) staff       (20)      103 2023-05-03 12:15:02.489897 csst-ifs-gehong-0.0.1.5/setup.cfg
+-rw-r--r--   0 sfeng      (501) staff       (20)      392 2023-05-03 11:43:38.000000 csst-ifs-gehong-0.0.1.5/setup.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.484777 csst-ifs-gehong-0.0.1.5/src/
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.486724 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/
+-rw-r--r--   0 sfeng      (501) staff       (20)      228 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/PKG-INFO
+-rw-r--r--   0 sfeng      (501) staff       (20)      415 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/SOURCES.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        1 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/dependency_links.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        8 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/requires.txt
+-rw-r--r--   0 sfeng      (501) staff       (20)        7 2023-05-03 12:15:02.000000 csst-ifs-gehong-0.0.1.5/src/csst_ifs_gehong.egg-info/top_level.txt
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.488025 csst-ifs-gehong-0.0.1.5/src/gehong/
+-rw-r--r--   0 sfeng      (501) staff       (20)        0 2023-04-12 01:06:24.000000 csst-ifs-gehong-0.0.1.5/src/gehong/__init__.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     1236 2023-05-02 10:42:18.000000 csst-ifs-gehong-0.0.1.5/src/gehong/config.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     3591 2023-05-03 04:54:26.000000 csst-ifs-gehong-0.0.1.5/src/gehong/cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    11669 2023-05-03 04:45:44.000000 csst-ifs-gehong-0.0.1.5/src/gehong/map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    37295 2023-05-03 12:14:02.000000 csst-ifs-gehong-0.0.1.5/src/gehong/spec1d.py
+drwxr-xr-x   0 sfeng      (501) staff       (20)        0 2023-05-03 12:15:02.488764 csst-ifs-gehong-0.0.1.5/test/
+-rw-r--r--   0 sfeng      (501) staff       (20)     2710 2023-05-03 04:52:05.000000 csst-ifs-gehong-0.0.1.5/test/test_cube3d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)     8115 2023-05-03 04:46:37.000000 csst-ifs-gehong-0.0.1.5/test/test_map2d.py
+-rw-r--r--   0 sfeng      (501) staff       (20)    17388 2023-05-03 01:16:32.000000 csst-ifs-gehong-0.0.1.5/test/test_spec1d.py
```

### Comparing `csst-ifs-gehong-0.0.1.4/LICENSE` & `csst-ifs-gehong-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.4/src/gehong/config.py` & `csst-ifs-gehong-0.0.1.5/src/gehong/config.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.4/src/gehong/cube3d.py` & `csst-ifs-gehong-0.0.1.5/src/gehong/cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.4/src/gehong/map2d.py` & `csst-ifs-gehong-0.0.1.5/src/gehong/map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.4/src/gehong/spec1d.py` & `csst-ifs-gehong-0.0.1.5/src/gehong/spec1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,19 +209,19 @@
     -------
     float
         Extinction value corresponding to the input wavelength
     """
     wave_number = 1./(wave * 1e-4)
     reddening_curve = np.zeros(len(wave))
     
-    idx = np.logical_and(wave >= 1200, wave <= 6300)
+    idx = (wave >= 1200) & (wave < 6300)
     reddening_curve[idx] = 2.659 * ( -2.156 + 1.509 * wave_number[idx] - 0.198 * \
                     (wave_number[idx] ** 2)) + 0.011 * (wave_number[idx] **3 ) + Rv
                                     
-    idx = np.logical_and(wave >= 6300, wave <= 22000)
+    idx = (wave >= 6300) & (wave <= 22000)
     reddening_curve[idx] = 2.659 * ( -1.857 + 1.040 * wave_number[idx]) + Rv
     return reddening_curve
 
 def reddening(wave, flux, ebv = 0.0, law = 'calzetti', Rv = 4.05):
     """
     Reddening an input spectra through a given reddening curve.
 
@@ -611,15 +611,15 @@
     The class of power-law spectrum of AGN
 
     Parameters
     ----------
     config : class
         Class of configuration
     M5100 : float, optional
-        Median flux of power law spectrum between 5050A and 5150A, by default 1000.0 * 1e-17 erg/s/cm^2
+        Magnitude of power law spectrum between 5050A and 5150A, by default 1000.0 * 1e-17 erg/s/cm^2
     alpha : float, optional
         Index of power law, by default -1.5
     vel : float, optional
         Line of sight velocity, by default 100.0km/s
     Ebv : float, optional
         Dust extinction, by default 0.1
     """
@@ -697,29 +697,29 @@
         self.flux = NLR.flux + PL.flux + Fe.flux
         
         if halpha_broad > 0:
             self.flux = self.flux + BLR.flux
     
 def BHmass_to_M5100(bhmass, edd_ratio = 0.05, dist = 21.0):
     """
-    Caculate luminosity at 5100A according to the black hole mass
+    Caculate magnitude at 5100A according to the black hole mass
 
     Parameters
     ----------
     bhmass : float
         Black hole mass, unit: solar mass
     edd_ratio : float, optional
         Eddtington ratio, by default 0.05
     dist : float, optional
         Distance to the black hole, by default 21.0Mpc
 
     Returns
     -------
     float
-        Luminosity at 5100A
+        Magnitude at 5100A
     """
     
     # Calculate bolometric luminosity
     Ledd = 3e4 * bhmass
     Lbol = Ledd * edd_ratio
 
     # Convert bolometric luminosity to 5100A luminosity (Marconi et al. 2004)
```

### Comparing `csst-ifs-gehong-0.0.1.4/test/test_cube3d.py` & `csst-ifs-gehong-0.0.1.5/test/test_cube3d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.4/test/test_map2d.py` & `csst-ifs-gehong-0.0.1.5/test/test_map2d.py`

 * *Files identical despite different names*

### Comparing `csst-ifs-gehong-0.0.1.4/test/test_spec1d.py` & `csst-ifs-gehong-0.0.1.5/test/test_spec1d.py`

 * *Files identical despite different names*

