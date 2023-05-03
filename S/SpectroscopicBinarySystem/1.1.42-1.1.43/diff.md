# Comparing `tmp/SpectroscopicBinarySystem-1.1.42.tar.gz` & `tmp/SpectroscopicBinarySystem-1.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.1.42.tar", last modified: Mon May  1 09:14:58 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.1.43.tar", last modified: Wed May  3 12:42:38 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.1.42.tar` & `SpectroscopicBinarySystem-1.1.43.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 09:14:58.923858 SpectroscopicBinarySystem-1.1.42/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.42/LICENSE
--rw-rw-rw-   0        0        0     4732 2023-05-01 09:14:58.923858 SpectroscopicBinarySystem-1.1.42/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2023-05-01 08:09:46.000000 SpectroscopicBinarySystem-1.1.42/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 09:14:58.919834 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-01 09:14:58.000000 SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.42/pyproject.toml
--rw-rw-rw-   0        0        0      725 2023-05-01 09:14:58.927845 SpectroscopicBinarySystem-1.1.42/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 09:14:58.923858 SpectroscopicBinarySystem-1.1.42/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    29374 2023-05-01 09:13:08.000000 SpectroscopicBinarySystem-1.1.42/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:42:38.660517 SpectroscopicBinarySystem-1.1.43/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.43/LICENSE
+-rw-rw-rw-   0        0        0     4732 2023-05-03 12:42:38.660517 SpectroscopicBinarySystem-1.1.43/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2023-05-03 12:42:11.000000 SpectroscopicBinarySystem-1.1.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 12:42:38.658010 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.43/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-05-03 12:42:38.664540 SpectroscopicBinarySystem-1.1.43/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 12:42:38.660517 SpectroscopicBinarySystem-1.1.43/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    30330 2023-05-03 12:40:47.000000 SpectroscopicBinarySystem-1.1.43/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.1.42/LICENSE` & `SpectroscopicBinarySystem-1.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.42/PKG-INFO` & `SpectroscopicBinarySystem-1.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.42
+Version: 1.1.43
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.41)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.43)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.42/README.md` & `SpectroscopicBinarySystem-1.1.43/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.41)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.43)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.42
+Version: 1.1.43
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.41)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.43)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.42/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.42/setup.cfg` & `SpectroscopicBinarySystem-1.1.43/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 3432 0d0a  rsion = 1.1.42..
+00000030: 7273 696f 6e20 3d20 312e 312e 3433 0d0a  rsion = 1.1.43..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.1.42/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.1.43/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,22 +364,27 @@
         # write result file for BinaryStarSolver
         with open(f'{self._spectra_path}/sbs_results.txt', 'w') as f:
             for s in self._sb_spectra:
                 output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)}"
                 f.write(output + '\n')
 
         # [γ, K, ω, e, T0, P, a, f(M)]
-        params, err, cov = StarSolve(
-            data_file=f"{self._spectra_path}/sbs_results.txt",
-            star="primary",
-            Period=self._period,
-            Pguess=self._period_guess,
-            covariance=True,
-            graphs=False,
-        )
+        try:
+            params, err, cov = StarSolve(
+                data_file=f"{self._spectra_path}/sbs_results.txt",
+                star="primary",
+                Period=self._period,
+                Pguess=self._period_guess,
+                covariance=True,
+                graphs=False,
+            )
+        except:
+            print(
+                'An exception occurred : the calculation of the orbital solution failed')
+            exit()
 
         self._orbital_solution = (params, err, cov)
 
         # If self._t0 compute phase delta between T0 of the model and the fixed value
         if self._t0:
             t0 = self._t0
             phase1 = self.__getPhase(
@@ -422,15 +427,15 @@
         :param array: array for search
         :param value: value to find
         :return: index of the nearest value
         """
         array = np.asarray(array)
         return (np.abs(array - value)).argmin()
 
-    def __plotRadialVelocityDots(self, axs, t0):
+    def __plotRadialVelocityDots(self, axs, t0, group_by_instruments=False):
         """
         Plot the radial velocity dots from the data
         :param axs: axes to plot
         :model t0: Periastron epoch T0 (julian date)
         :return: None
         """
         observers = {}
@@ -452,35 +457,42 @@
         for s in self._sb_spectra:
 
             # get the observer
             obs = s.getObserver()
             if (obs not in observers.keys()):
                 observers[obs] = colors[color_number]
                 color_number += 1
+                if not group_by_instruments:
+                    axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
+                                    fmt='o', ecolor='k', label=obs, capsize=0, color=observers[obs], lw=.7, markersize=5)
+            elif not group_by_instruments:
+                axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
+                                fmt='o', ecolor='k', capsize=0, color=observers[obs], lw=.7, markersize=5)
             color = observers[obs]
 
             # get the instrument
-
-            label = f"{obs} - {s.getInstrument()[:30]}…"
-            if label not in instruments.keys():
-                if obs not in marker_index:
-                    marker_index[obs] = 0
-                instruments[label] = markers_style[marker_index[obs]]
-                marker_index[obs] += 1
-                axs[0].errorbar(s.getPhase(), s.getRV(
-                ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
-            else:
-                axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
-                                fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
+            if (group_by_instruments):
+                label = f"{obs} - {s.getInstrument()[:30]}…"
+                if label not in instruments.keys():
+                    if obs not in marker_index:
+                        marker_index[obs] = 0
+                    instruments[label] = markers_style[marker_index[obs]]
+                    marker_index[obs] += 1
+                    axs[0].errorbar(s.getPhase(), s.getRV(
+                    ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
+                else:
+                    axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
+                                    fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
             xindex = self.__findNearest(self._model_x, s.getPhase())
+            fmt = instruments[label] if group_by_instruments else 'o'
             axs[1].errorbar(s.getPhase(), s.getRV() - self._model_y[xindex],
-                            yerr=0, fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
+                            yerr=0, fmt=fmt, ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
-    def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=0.5, savefig=False, dpi=150, font_family='monospace', font_size=9):
+    def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=None, savefig=False, dpi=150, font_family='monospace', font_size=9, group_by_instruments=False):
         if not self._orbital_solution:
             self.__solveSystem()
 
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
         fig, axs = plt.subplots(2, 1, figsize=(11, 7), gridspec_kw={
                                 'height_ratios': [4, 1]}, sharex=True)
@@ -499,27 +511,30 @@
         self._model_x = np.arange(0, 1.011, 0.001)
         self._model_y = list(map(lambda x: self.__computeRadialVelocityCurve(
             x, self._v0, self._orbital_solution[0][1], self._orbital_solution[0][3], self._orbital_solution[0][2], self._orbital_solution[0][0]), self._model_x))
         axs[0].plot(self._model_x, self._model_y, 'k',
                     alpha=0.7, lw=0.7, label='Orbital solution')
 
         # plot dots
-        self.__plotRadialVelocityDots(axs, self._t0)
+        self.__plotRadialVelocityDots(axs, self._t0, group_by_instruments)
 
         split_oname = title.split(' ')
         t = ''.join(r"$\bf{%s}$ " % (w) for w in split_oname)
         p = f'{self._orbital_solution[0][5]} ± {round(self._orbital_solution[1][5],4)} days'
         subtitle = f'{subtitle}\nT0={self._t0} P={p}' if subtitle else f'T0={self._t0} P={p}'
         axs[0].set_title("%s\n%s" % (t, subtitle), fontsize=9,
                          fontweight="0", color='black')
 
-        axs[0].yaxis.set_major_locator(MultipleLocator(rv_y_multiple))
+        if rv_y_multiple:
+            axs[0].yaxis.set_major_locator(MultipleLocator(rv_y_multiple))
         axs[0].axhline(0, color='black', linewidth=0.7, linestyle="--")
 
-        axs[1].yaxis.set_major_locator(MultipleLocator(residual_y_multiple))
+        if residual_y_multiple:
+            axs[1].yaxis.set_major_locator(
+                MultipleLocator(residual_y_multiple))
         axs[1].axhline(0, color='black', linewidth=0.7, linestyle="--")
 
         axs[0].legend(bbox_to_anchor=(1, 1), loc="upper left",
                       frameon=False, prop={'size': 8})
         plt.tight_layout(pad=1, w_pad=0, h_pad=1)
         plt.xticks(np.arange(0, 1.01, 0.1))
         if savefig:
@@ -712,15 +727,15 @@
             ss = copy.copy(s)
             # apply heliocentric/barycentric correction
             ss.shift_spectrum_to(
                 radial_velocity=s.getRVCorrection())
             fluxc_resample = LinearInterpolatedResampler()
             output_spectrum1D = fluxc_resample(ss, sc)
             phase = s.getPhase()
-            indice = int(round(phase, 2) * len(y_phase))-1
+            indice = int(round(phase, 2) * (len(y_phase))-1)
 
             spec2d[:, indice] = output_spectrum1D.flux
 
         # prepare imshow
         plt.rcParams["figure.figsize"] = (8, 7)
         fig, ax = plt.subplots()
         ax.imshow(np.rot90(spec2d), extent=[wv_to_kms.min().value,
```

