# Comparing `tmp/plot-antenna-1.0.tar.gz` & `tmp/plot-antenna-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-antenna-1.0.tar", last modified: Sun Oct 30 13:03:24 2022, max compression
+gzip compressed data, was "plot-antenna-1.1.tar", last modified: Wed May  3 13:44:27 2023, max compression
```

## Comparing `plot-antenna-1.0.tar` & `plot-antenna-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-10-30 13:03:24.373878 plot-antenna-1.0/
--rw-r--r--   0 ralf      (1000) priv      (1011)     8739 2022-10-30 13:03:24.373878 plot-antenna-1.0/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     6947 2022-09-13 08:09:10.000000 plot-antenna-1.0/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-10-30 13:03:24.341878 plot-antenna-1.0/plot_antenna/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2022-10-30 13:02:26.000000 plot-antenna-1.0/plot_antenna/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.0/plot_antenna/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    46054 2022-10-30 10:51:48.000000 plot-antenna-1.0/plot_antenna/plot_antenna.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-10-30 13:03:24.365878 plot-antenna-1.0/plot_antenna.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)     8739 2022-10-30 13:03:24.000000 plot-antenna-1.0/plot_antenna.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      333 2022-10-30 13:03:24.000000 plot-antenna-1.0/plot_antenna.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2022-10-30 13:03:24.000000 plot-antenna-1.0/plot_antenna.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       65 2022-10-30 13:03:24.000000 plot-antenna-1.0/plot_antenna.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       17 2022-10-30 13:03:24.000000 plot-antenna-1.0/plot_antenna.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       13 2022-10-30 13:03:24.000000 plot-antenna-1.0/plot_antenna.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2022-10-30 13:03:24.373878 plot-antenna-1.0/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.0/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2022-10-30 13:03:24.369878 plot-antenna-1.0/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.0/test/test_plot.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.677311 plot-antenna-1.1/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9309 2023-05-03 13:44:27.677311 plot-antenna-1.1/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7405 2023-05-03 13:41:51.000000 plot-antenna-1.1/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.649310 plot-antenna-1.1/plot_antenna/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-03 13:44:00.000000 plot-antenna-1.1/plot_antenna/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.1/plot_antenna/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    47920 2023-05-03 13:32:42.000000 plot-antenna-1.1/plot_antenna/plot_antenna.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.669310 plot-antenna-1.1/plot_antenna.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     9309 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-03 13:44:27.000000 plot-antenna-1.1/plot_antenna.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-03 13:44:27.677311 plot-antenna-1.1/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.1/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-03 13:44:27.673311 plot-antenna-1.1/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.1/test/test_plot.py
```

### Comparing `plot-antenna-1.0/PKG-INFO` & `plot-antenna-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.0
+Version: 1.1
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -125,15 +125,15 @@
         to the right of the plot. With mouse-over you can see the current angle
         (Elevation or Azimuth with the 2D plots and both for the 3D plot) and
         the gain at that point. For the 2D variants, more than one frequency can
         be selected for plotting. This allows comparison of pattern between
         different frequencies. For the 3D plot, the frequencies in the legend
         act like radio-buttons, only one at a time can be selected.
         
-        With the --geo option you get a display of the antenna geometry.
+        With the ``--geo`` option you get a display of the antenna geometry.
         Unfortunately plotly_ seems to have limitations on the zoom depths, so
         for large antennas it is not possible to see the plot in deep detail. As
         of this writing not all geometry details are displayed. In particular 2D
         patches in NEC, transmission lines in NEC, and visualization of loaded
         segments (e.g. with a capacity) are not shown.
         
         .. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
@@ -148,14 +148,28 @@
         .. _`Antenna modelling notes episode 48`:
             http://on5au.be/content/amod/amod48.html
         .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
         .. _pymininec: https://github.com/schlatterbeck/pymininec
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         
+        Release Notes
+        -------------
+        
+        v1.1: Specification of azimuth / elevation angle
+        
+        - Now we can specify an azimuth angle for elevation plot and an
+          elevation angle for azimuth plots
+        - Bug-fix in computation of maximum gain azimuth direction: If the
+          maximum gain in theta direction goes up or down, the azimuth angle
+          would be computed incorrectly because all gain values at that theta
+          angle are the same for all azimuth angles.
+        
+        v1.0: Initial Release
+        
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
```

### Comparing `plot-antenna-1.0/README.rst` & `plot-antenna-1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 to the right of the plot. With mouse-over you can see the current angle
 (Elevation or Azimuth with the 2D plots and both for the 3D plot) and
 the gain at that point. For the 2D variants, more than one frequency can
 be selected for plotting. This allows comparison of pattern between
 different frequencies. For the 3D plot, the frequencies in the legend
 act like radio-buttons, only one at a time can be selected.
 
-With the --geo option you get a display of the antenna geometry.
+With the ``--geo`` option you get a display of the antenna geometry.
 Unfortunately plotly_ seems to have limitations on the zoom depths, so
 for large antennas it is not possible to see the plot in deep detail. As
 of this writing not all geometry details are displayed. In particular 2D
 patches in NEC, transmission lines in NEC, and visualization of loaded
 segments (e.g. with a capacity) are not shown.
 
 .. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
@@ -139,7 +139,21 @@
     http://on5au.be/Books/allmodnotes.zip
 .. _`Antenna modelling notes episode 48`:
     http://on5au.be/content/amod/amod48.html
 .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
 .. _pymininec: https://github.com/schlatterbeck/pymininec
 .. _matplotlib: https://matplotlib.org/
 .. _plotly: https://github.com/plotly/plotly.py
+
+Release Notes
+-------------
+
+v1.1: Specification of azimuth / elevation angle
+
+- Now we can specify an azimuth angle for elevation plot and an
+  elevation angle for azimuth plots
+- Bug-fix in computation of maximum gain azimuth direction: If the
+  maximum gain in theta direction goes up or down, the azimuth angle
+  would be computed incorrectly because all gain values at that theta
+  angle are the same for all azimuth angles.
+
+v1.0: Initial Release
```

### Comparing `plot-antenna-1.0/plot_antenna/plot_antenna.py` & `plot-antenna-1.1/plot_antenna/plot_antenna.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 
 import sys
 import os
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import numpy as np
+from bisect import bisect
 from mpl_toolkits.mplot3d import Axes3D
 from argparse import ArgumentParser
 from matplotlib import cm, __version__ as matplotlib_version, rcParams
 from matplotlib.widgets import Slider
 try:
     import plotly.express as px
     import plotly.graph_objects as go
@@ -169,63 +170,69 @@
         self.thetas   = self.thetas_d * np.pi / 180
         self.phis     = self.phis_d   * np.pi / 180
         self.maxg     = max (gains)
         self.gains    = np.reshape \
             (np.array (gains), (self.thetas.shape [0], -1))
         idx = np.unravel_index (self.gains.argmax (), self.gains.shape)
         self.theta_maxidx, self.phi_maxidx = idx
+        # Special case: If theta is 0° or 180° recompute phi_maxidx
+        # since in that case all values are the same at that theta angle
+        if self.thetas_d [self.theta_maxidx] == 0:
+            self.phi_maxidx = self.gains [1].argmax ()
+        elif self.thetas_d [self.theta_maxidx] == 180:
+            self.phi_maxidx = self.gains [-1].argmax ()
         self.theta_max = self.thetas_d [self.theta_maxidx]
         self.phi_max   = self.phis_d   [self.phi_maxidx]
         self.desc      = ['Title: %s' % self.parent.title]
         self.desc.append ('Frequency: %.2f MHz' % self.f)
         self.lbl_deg   = 0
         self.labels    = None
     # end def compute
 
     def azimuth_gains (self, scaler):
-        g = self.gains [self.parent.theta_maxidx]
+        g = self.gains [self.parent.theta_angle_idx]
         gains = scaler.scale (self.parent.maxg, g)
         return gains, g
     # end def azimuth_gains
 
     def azimuth_text (self, scaler):
         desc = self.desc.copy ()
         desc.insert (0, 'Azimuth Pattern')
         desc.append ('Outer ring: %.2f dBi' % self.parent.maxg)
         desc.append ('Scaling: %s' % scaler.title)
         desc.append \
             ( 'Elevation: %.2f°'
-            % (90 - self.thetas_d [self.parent.theta_maxidx])
+            % (90 - self.thetas_d [self.parent.theta_angle_idx])
             )
         return desc
     # end def azimuth_text
 
     def elevation_gains (self, scaler):
-        gains1 = self.gains.T [self.parent.phi_maxidx].T
+        gains1 = self.gains.T [self.parent.phi_angle_idx].T
         # Find index of the other side of the azimuth
         pmx = self.phis.shape [0] - self.phis.shape [0] % 2
-        idx = (self.parent.phi_maxidx + pmx // 2) % pmx
-        assert idx != self.parent.phi_maxidx
+        idx = (self.parent.phi_angle_idx + pmx // 2) % pmx
+        assert idx != self.parent.phi_angle_idx
         eps = 1e-9
         phis = self.phis
-        assert abs (phis [idx] - phis [self.parent.phi_maxidx]) - np.pi < eps
+        assert abs (phis [idx] - phis [self.parent.phi_angle_idx]) - np.pi < eps
         gains2 = self.gains.T [idx].T
         g = np.append (gains1, np.flip (gains2))
         gains = scaler.scale (self.parent.maxg, g)
         return gains, g
     # end def elevation_gains
 
     def elevation_text (self, scaler):
         desc = self.desc.copy ()
         desc.insert (0, 'Elevation Pattern')
         desc.append ('Outer ring: %.2f dBi' % self.parent.maxg)
         desc.append ('Scaling: %s' % scaler.title)
         desc.append \
-            ( 'Azimuth: %.2f° (X: 0°)'
-            % self.phis_d [self.parent.phi_maxidx]
+            ( 'Azimuth: %.2f° (X=0°)'
+            % self.phis_d [self.parent.phi_angle_idx]
             )
         return desc
     # end def elevation_text
 
     def plot3d_gains (self, scaler):
         gains  = scaler.scale (self.parent.maxg, self.gains)
         P, T   = np.meshgrid (self.phis, self.thetas)
@@ -243,14 +250,30 @@
         # https://github.com/plotly/plotly.js/issues/5003
         t = np.moveaxis (t, (0, 1, 2), (1, 0, 2))
         return t, gains, X, Y, Z
     # end def plot3d_gains
 
 # end class Gain_Data
 
+def nearest_angle_idx (angles, dst_angle):
+    """ Compute index of angle nearest to dst_angle in angles.
+        The sequence angles is sorted.
+    """
+    idx  = bisect (angles, dst_angle)
+    if idx >= len (angles):
+        idx = len (angles) - 1
+    if idx < 0:
+        idx = 0
+    if idx == 0:
+        return idx
+    if (abs (angles [idx] - dst_angle) < abs (angles [idx - 1] - dst_angle)):
+        return idx
+    return idx - 1
+# end def nearest_angle_idx
+
 class Gain_Plot:
     fig_x = 512
     fig_y = 384
     plot_names   = ('azimuth', 'elevation', 'plot_vswr', 'plot3d', 'plot_geo')
     update_names = set (('azimuth', 'elevation', 'plot3d'))
 
 
@@ -277,14 +300,15 @@
             self.with_slider = False
         # Default title from filename
         self.title       = os.path.splitext \
             (os.path.basename (args.filename)) [0]
         # This might override title
         self.gdata = {}
         self.geo = []
+        # This populates gdata:
         self.read_file ()
         self.frequencies = []
         self.maxg = None
         theta_idx = {}
         phi_idx   = {}
         for f in sorted (self.gdata):
             gdata = self.gdata [f]
@@ -300,14 +324,26 @@
             self.frequencies.append (f)
         # Compute the theta index that occurs most often over all
         # frequencies
         self.theta_maxidx = list \
             (sorted (theta_idx, key = lambda a: theta_idx [a])) [-1]
         self.phi_maxidx = list \
             (sorted (phi_idx, key = lambda a: phi_idx [a])) [-1]
+        if self.args.azimuth_angle is not None:
+            phis = next (iter (self.gdata.values ())).phis_d
+            self.phi_angle_idx = nearest_angle_idx \
+                (phis, self.args.azimuth_angle)
+        else:
+            self.phi_angle_idx = self.phi_maxidx
+        if self.args.elevation_angle is not None:
+            thetas = next (iter (self.gdata.values ())).thetas_d
+            self.theta_angle_idx = nearest_angle_idx \
+                (thetas, 90 - self.args.elevation_angle)
+        else:
+            self.theta_angle_idx = self.theta_maxidx
         if self.outfile or len (self.gdata) == 1 or not self.with_slider:
             self.with_slider = False
         # Borrow colormap from matplotlib to use in plotly
         self.colormap = []
         for cn in mcolors.TABLEAU_COLORS:
             self.colormap.append (mcolors.TABLEAU_COLORS [cn])
     # end def __init__
@@ -701,16 +737,15 @@
             fig.savefig (self.outfile)
         else:
             plt.show ()
     # end def plot_matplotlib
 
     def azimuth (self, name):
         self.desc = self.data.azimuth_text (self.scaler)
-        pm = self.data.phis_d [self.phi_maxidx]
-        self.lbl_deg = pm
+        self.lbl_deg = self.data.phis_d [self.phi_angle_idx]
         self.labels  = 'XY'
         self.polargains, self.unscaled = self.data.azimuth_gains (self.scaler)
         self.angles = self.data.phis
         self.polarplot (name)
     # end def azimuth
 
     def elevation (self, name):
@@ -721,15 +756,15 @@
             self.polargains = gains1
             OK for both 90° and 180° plots:
             self.angles = p2 + self.thetas
             self.polargains = gains2
             But second half must (both) be flipped to avoid crossover
         """
         self.desc = self.data.elevation_text (self.scaler)
-        self.lbl_deg  = 90 - self.data.thetas_d [self.theta_maxidx]
+        self.lbl_deg  = 90 - self.data.thetas_d [self.theta_angle_idx]
         self.labels   = None
         self.polargains, self.unscaled = self.data.elevation_gains (self.scaler)
         thetas = self.data.thetas
         p2 = np.pi / 2
         self.angles = np.append (p2 - thetas, np.flip (p2 + thetas))
         self.polarplot (name)
     # end def elevation
@@ -1137,24 +1172,36 @@
         )
     cmd.add_argument \
         ( '--azimuth'
         , help    = 'Do an azimuth plot'
         , action  = 'store_true'
         )
     cmd.add_argument \
+        ( '--azimuth-angle'
+        , help    = 'Azimuth angle to use for elevation plot, default is '
+                    'maximum gain angle'
+        , type    = float
+        )
+    cmd.add_argument \
         ( '--dpi'
         , help    = 'Resolution for matplotlib, default = %(default)s'
         , type    = int
         , default = 80
         )
     cmd.add_argument \
         ( '--elevation'
         , help    = 'Do an elevation plot'
         , action  = 'store_true'
         )
+    cmd.add_argument \
+        ( '--elevation-angle'
+        , help    = 'Elevation angle to use for azimuth plot, default is '
+                    'maximum gain angle'
+        , type    = float
+        )
     # For versions below 3.5 slider will be always off
     if matplotlib_version_float >= 3.5:
         cmd.add_argument \
             ( '--with-frequency-slider', '--with-slider'
             , dest    = 'with_slider'
             , help    = 'Turn on frequency slider, frequency can be stepped'
                         ' with +/- keys and slider is very slow.'
```

### Comparing `plot-antenna-1.0/plot_antenna.egg-info/PKG-INFO` & `plot-antenna-1.1/plot_antenna.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.0
+Version: 1.1
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -125,15 +125,15 @@
         to the right of the plot. With mouse-over you can see the current angle
         (Elevation or Azimuth with the 2D plots and both for the 3D plot) and
         the gain at that point. For the 2D variants, more than one frequency can
         be selected for plotting. This allows comparison of pattern between
         different frequencies. For the 3D plot, the frequencies in the legend
         act like radio-buttons, only one at a time can be selected.
         
-        With the --geo option you get a display of the antenna geometry.
+        With the ``--geo`` option you get a display of the antenna geometry.
         Unfortunately plotly_ seems to have limitations on the zoom depths, so
         for large antennas it is not possible to see the plot in deep detail. As
         of this writing not all geometry details are displayed. In particular 2D
         patches in NEC, transmission lines in NEC, and visualization of loaded
         segments (e.g. with a capacity) are not shown.
         
         .. [1] L. B. Cebik. Radiation plots: Polar or rectangular; log or linear.
@@ -148,14 +148,28 @@
         .. _`Antenna modelling notes episode 48`:
             http://on5au.be/content/amod/amod48.html
         .. _nec2c: https://packages.debian.org/stable/hamradio/nec2c
         .. _pymininec: https://github.com/schlatterbeck/pymininec
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         
+        Release Notes
+        -------------
+        
+        v1.1: Specification of azimuth / elevation angle
+        
+        - Now we can specify an azimuth angle for elevation plot and an
+          elevation angle for azimuth plots
+        - Bug-fix in computation of maximum gain azimuth direction: If the
+          maximum gain in theta direction goes up or down, the azimuth angle
+          would be computed incorrectly because all gain values at that theta
+          angle are the same for all azimuth angles.
+        
+        v1.0: Initial Release
+        
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
```

### Comparing `plot-antenna-1.0/setup.py` & `plot-antenna-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `plot-antenna-1.0/test/test_plot.py` & `plot-antenna-1.1/test/test_plot.py`

 * *Files identical despite different names*

