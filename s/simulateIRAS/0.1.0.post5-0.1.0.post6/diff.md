# Comparing `tmp/simulateIRAS-0.1.0.post5.tar.gz` & `tmp/simulateIRAS-0.1.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulateIRAS-0.1.0.post5.tar", last modified: Tue May  2 19:13:36 2023, max compression
+gzip compressed data, was "simulateIRAS-0.1.0.post6.tar", last modified: Tue May  2 22:21:05 2023, max compression
```

## Comparing `simulateIRAS-0.1.0.post5.tar` & `simulateIRAS-0.1.0.post6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.753524 simulateIRAS-0.1.0.post5/
--rw-rw-rw-   0        0        0    35184 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/LICENSE
--rw-rw-rw-   0        0        0       27 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/MANIFEST.in
--rw-rw-rw-   0        0        0     4099 2023-05-02 19:13:36.753524 simulateIRAS-0.1.0.post5/PKG-INFO
--rw-rw-rw-   0        0        0     3289 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.731524 simulateIRAS-0.1.0.post5/examples/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.738524 simulateIRAS-0.1.0.post5/examples/dataRegression/
--rw-rw-rw-   0        0        0     8080 2023-05-02 18:56:34.000000 simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression.py
--rw-rw-rw-   0        0        0     8096 2023-05-02 18:58:36.000000 simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression2.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.740523 simulateIRAS-0.1.0.post5/examples/simpleSimulation/
--rw-rw-rw-   0        0        0    52782 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/IRASTestK.txt
--rw-rw-rw-   0        0        0   193070 2023-05-02 17:24:17.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/SimulatedIRAS.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.740523 simulateIRAS-0.1.0.post5/examples/simpleSimulation/Solutions/
--rw-rw-rw-   0        0        0   193070 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
--rw-rw-rw-   0        0        0     2862 2023-05-02 18:48:22.000000 simulateIRAS-0.1.0.post5/examples/simpleSimulation/simpleSimulation.py
--rw-rw-rw-   0        0        0       99 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/pyproject.toml
--rw-rw-rw-   0        0        0      375 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 19:13:36.753524 simulateIRAS-0.1.0.post5/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-02 19:13:19.000000 simulateIRAS-0.1.0.post5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.742523 simulateIRAS-0.1.0.post5/src/
--rw-rw-rw-   0        0        0        2 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.752524 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/
--rw-rw-rw-   0        0        0     4099 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 19:13:36.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10024 2023-05-02 19:13:05.000000 simulateIRAS-0.1.0.post5/src/simulateIRAS.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:13:36.752524 simulateIRAS-0.1.0.post5/tests/
--rw-rw-rw-   0        0        0      146 2023-05-02 17:12:29.000000 simulateIRAS-0.1.0.post5/tests/test_code.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.156472 simulateIRAS-0.1.0.post6/
+-rw-rw-rw-   0        0        0    35184 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5503 2023-05-02 22:21:05.156472 simulateIRAS-0.1.0.post6/PKG-INFO
+-rw-rw-rw-   0        0        0     4688 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.096754 simulateIRAS-0.1.0.post6/examples/
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.109848 simulateIRAS-0.1.0.post6/examples/dataRegression/
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.118848 simulateIRAS-0.1.0.post6/examples/dataRegression/Solutions/
+-rw-rw-rw-   0        0        0   201826 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/examples/dataRegression/Solutions/SimulatedIRAS.txt
+-rw-rw-rw-   0        0        0   157340 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/examples/dataRegression/Solutions/SimulatedK.txt
+-rw-rw-rw-   0        0        0    10004 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/examples/dataRegression/dataRegression.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.129469 simulateIRAS-0.1.0.post6/examples/simpleSimulation/
+-rw-rw-rw-   0        0        0    52782 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/examples/simpleSimulation/IRASTestK.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.132474 simulateIRAS-0.1.0.post6/examples/simpleSimulation/Solutions/
+-rw-rw-rw-   0        0        0   193070 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/examples/simpleSimulation/Solutions/SimulatedIRAS.txt
+-rw-rw-rw-   0        0        0     2402 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/examples/simpleSimulation/simpleSimulation.py
+-rw-rw-rw-   0        0        0       99 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/pyproject.toml
+-rw-rw-rw-   0        0        0      375 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 22:21:05.156472 simulateIRAS-0.1.0.post6/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-02 22:20:44.000000 simulateIRAS-0.1.0.post6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.138474 simulateIRAS-0.1.0.post6/src/
+-rw-rw-rw-   0        0        0        2 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.154472 simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/
+-rw-rw-rw-   0        0        0     5503 2023-05-02 22:21:05.000000 simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-05-02 22:21:05.000000 simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 22:21:05.000000 simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 22:21:05.000000 simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 22:21:05.000000 simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10024 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/src/simulateIRAS.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:21:05.155471 simulateIRAS-0.1.0.post6/tests/
+-rw-rw-rw-   0        0        0      146 2023-05-02 22:20:29.000000 simulateIRAS-0.1.0.post6/tests/test_code.py
```

### Comparing `simulateIRAS-0.1.0.post5/LICENSE` & `simulateIRAS-0.1.0.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post5/PKG-INFO` & `simulateIRAS-0.1.0.post6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0.post5
+Version: 0.1.0.post6
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
@@ -53,16 +53,25 @@
 We recommend importing in python as iras. 
 <br><br>
 `import simulateIRAS as iras`
 <br>
 
 ## Examples
 ### Example 1: Simulating polarization- and azimuth-resolved IRAS spectra
+This example simulates the 4 polarization- and azimuth-resolved IRAS spectra with given k parameters k(x), k(y), k(z) for an isotropic, dielectric substrate. The python code, input files and output files are provided in "simulateIRAS/examples/simpleSimulation". The simulation requires the following inputs: 
+1) incident angle of light relative to the surface normal
+2) complex index of refraction of the subtrate layer which here is wavelength independent for an isotropic substrate modelling anatase TiO<sub>2</sub>(101) as $n = 2.3 + 0.0i$.
+3) k parameters of the adsorbate layer (imaginary part of the complex index of refraction) which here is for a water film.
+4) real index of refraction of the adsorbate layer in the infinite wavenumber simulation limit which here is taken as $Real(n) = 1.37$ for a water film.
+5) adsobate film thickness
+The Kramersâ€“Kronig relations aure use on the adsorbate k parameters (imaginary part of the complex index of refraction) to get the real part of the complex index of refraction for the adsorbate layer. The simulation then applies the three-layer (substrate-adsorbate-vacuum) model to simulate the 4 polarization- and azimuth-resolved IRAS spectra.
+<br>
+The input adsorbate k parameters and 4 polarization- and azimuth-resolved simulated IRAS spectra are plotted below:
 <p align="center">
-<img src='./examples/simpleSimulation/Solutions/Figure1.png' width='50%'>
+<img src='./examples/simpleSimulation/Solutions/Figure0.png' width='40%'><img src='./examples/simpleSimulation/Solutions/Figure1.png' width='40%'>
 </p>
 
 ### Example 2: Determining extinction coefficients from polarization- and azimuth-resolved IRAS spectra
 <p align="center">
 <img src='./examples/simpleSimulation/Solutions/Figure1.png' width='50%'>
 </p>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `simulateIRAS-0.1.0.post5/examples/dataRegression/dataRegression.py` & `simulateIRAS-0.1.0.post6/examples/dataRegression/dataRegression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Aug 12 13:19:18 2021
 
-@author: ocon360
-"""
 
 import numpy as np 
 from matplotlib import pyplot as plt
 import scipy.fftpack as ft
 import random
 import simulateIRAS as iras
 
-# IRAS Simulation parameters (Change these values for different simulations)
+
+# IRAS physical parameters (Change these values for different model systems)
 nVacuumComplexExpression = 1.0 + 0.0j
 nSubstrateComplexExpression = 2.3 + 0.0j
 nAdsorbateInf = 1.37
 
 filmThickness = 1.6*10**-8
 angle = 86*np.pi/180
 
-fittingXmin = 1900; fittingXmax = 3000; simulationBuffer = 1000; simulationXspacing = 1
-kPosition = 2100; kAmplitude = 0.001; kFWHM = 2
-numSimulations = 10; WeightingS = 5
+dataFile = "IRASTest2ML.csv"
 
-dataFile = "IRASTest.csv"
+# IRAS simulation parameters (Change these values for different regression conditions)
+fittingXmin = 1900; fittingXmax = 3000; simulationBuffer = 10; simulationXspacing = 0.05
+kPosition = 2100; kFWHM = 1; kAmplitude = 0.01; scaleStoP = 5
+
+numSimulationXY = 30000; kAmplitudeXY = 0.05; cutoffXY = 0.05
+numSimulationZ = 50000; cutoffZ = 1
+numSimulationXYZ = 50000; cutoffXYZ = 0; 
 
 # Imports IRAS data
 dataIRAS = iras.ImportSpectra(dataFile)
 simulationWavenumber = dataIRAS[0]
 
 # Generates the complex index of refraction for the vacuum and substrate layers
 nVacuum = \
@@ -47,106 +48,124 @@
 nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
 
 # Simulates and plots polarization- and azimuth-resolved spectra
 simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
                         nVacuum, nSubstrate, nAdsorbate,
                         filmThickness, angle)
 
-# Initial Guess Fitting Routine
-for i in range(fittingXmin, fittingXmax):
-    randomXYZ = list(range(0,3)); random.shuffle(randomXYZ)
-    for j in randomXYZ:
+# Initial Fitting kx and ky
+for i in range(0,numSimulationXY):
         # Randomizer for new peak fitting
-        tryAgain = True
+        randomXY = random.randint(0, 1)
+        randomWavenumber = random.randint(fittingXmin, fittingXmax)
+        randomKAmplitude = random.randint(-25,25) / 100
+        kNew = iras.LorentzianFunction(simulationWavenumber,randomWavenumber,(1+randomKAmplitude)*kAmplitude*scaleStoP,kFWHM)
         
         # Evaluate initial fit quality
-        fitQualityInitial = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, WeightingS)
+        fitQualityInitial = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, 1,0)
+        # print(np.sum(np.absolute(dataIRAS[1]-simulatedSpectra[1])))
+        # print(np.sum(np.absolute(dataIRAS[3]-simulatedSpectra[3])))
+            
+        if randomXY == 0:
+                kAdsorbateX = kAdsorbateX + kNew
+        if randomXY == 1:
+            kAdsorbateY = kAdsorbateY + kNew
 
-        while tryAgain:
-            randomKAmplitude = random.randint(-25,25) / 100
-            kNew = iras.LorentzianFunction(simulationWavenumber,i,(1+randomKAmplitude)*kAmplitude,kFWHM)
-            tryAgain = True
+        kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
             
-            # Evaluate initial fit quality
-            fitQualityInitial = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, WeightingS)
+        # Generates the k parameters for the adsorbate layer (imaginary index of refraction)
+        simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
         
-            if j == 0:
-                kAdsorbateX = kAdsorbateX + kNew
-            if j == 1:
-                kAdsorbateY = kAdsorbateY + kNew
-            if j == 2:
-                kAdsorbateZ = kAdsorbateZ + kNew
+        # Calculates the complex index of refraction for the adsorbate layer
+        nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
+        
+        # Simulates and plots polarization- and azimuth-resolved spectra
+        simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
+                                nVacuum, nSubstrate, nAdsorbate,
+                                filmThickness, angle)
+        
+        # Evaulate new fit quality
+        fitQualityFinal = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, 1,0)
+        
+        if fitQualityInitial < fitQualityFinal+(kAmplitudeXY*cutoffXY):
+            if randomXY == 0:
+                kAdsorbateX = kAdsorbateX - kNew
+            if randomXY == 1:
+                kAdsorbateY = kAdsorbateY - kNew
             kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
-                
-            # Generates the k parameters for the adsorbate layer (imaginary index of refraction)
             simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
-            
-            # Calculates the complex index of refraction for the adsorbate layer
             nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
-            
-            # Simulates and plots polarization- and azimuth-resolved spectra
-            simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
-                                    nVacuum, nSubstrate, nAdsorbate,
-                                    filmThickness, angle)
-            
-            # Evaulate new fit quality
-            fitQualityFinal = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, WeightingS)
-            
-            if fitQualityInitial < fitQualityFinal:
-                if j == 0:
-                    kAdsorbateX = kAdsorbateX - kNew
-                if j == 1:
-                    kAdsorbateY = kAdsorbateY - kNew
-                if j == 2:
-                    kAdsorbateZ = kAdsorbateZ - kNew
-                kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
-                simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
-                nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
-                tryAgain = False
                 
-# Fitting Routine
-for i in range(0,numSimulations):
+# Initial fitting routine kz
+for i in range(0,numSimulationZ):
         # Randomizer for new peak fitting
-        randomXYZ = random.randint(0, 2)
         randomWavenumber = random.randint(fittingXmin, fittingXmax)
         randomKAmplitude = random.randint(-25,25) / 100
         kNew = iras.LorentzianFunction(simulationWavenumber,randomWavenumber,(1+randomKAmplitude)*kAmplitude,kFWHM)
         
         # Evaluate initial fit quality
-        fitQualityInitial = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, WeightingS)
+        fitQualityInitial = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, 0,1)
+
+        kAdsorbateZ = kAdsorbateZ + kNew
+        kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
+            
+        # Generates the k parameters for the adsorbate layer (imaginary index of refraction)
+        simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
+        
+        # Calculates the complex index of refraction for the adsorbate layer
+        nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
+        
+        # Simulates and plots polarization- and azimuth-resolved spectra
+        simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
+                                nVacuum, nSubstrate, nAdsorbate,
+                                filmThickness, angle)
+        
+        # Evaulate new fit quality
+        fitQualityFinal = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, 0,1)
+        
+        if fitQualityInitial < fitQualityFinal+(kAmplitude*cutoffZ):
+            kAdsorbateZ = kAdsorbateZ - kNew
+            kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
+            simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
+            nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
+
+# Combined kx, ky, kz fitting routine
+for i in range(0,numSimulationXYZ):
+        # Randomizer for new peak fitting
+        randomWavenumber = random.randint(fittingXmin, fittingXmax)
+        randomKAmplitude = random.randint(-25,25) / 100
+        randomKXYSign = random.choice([-1,1])
+        kNew = iras.LorentzianFunction(simulationWavenumber,randomWavenumber,(randomKXYSign+randomKAmplitude)*kAmplitude,kFWHM)
+        
+        # Evaluate initial fit quality
+        fitQualityInitial = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, scaleStoP,1)
             
-        if randomXYZ == 0:
-                kAdsorbateX = kAdsorbateX + kNew
-        if randomXYZ == 1:
-            kAdsorbateY = kAdsorbateY + kNew
-        if randomXYZ == 2:
-            kAdsorbateZ = kAdsorbateZ + kNew
+        kAdsorbateX = kAdsorbateX + kNew*scaleStoP
+        kAdsorbateY = kAdsorbateY + kNew*scaleStoP
+        kAdsorbateZ = kAdsorbateZ - kNew
         kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
             
         # Generates the k parameters for the adsorbate layer (imaginary index of refraction)
         simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
         
         # Calculates the complex index of refraction for the adsorbate layer
         nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
         
         # Simulates and plots polarization- and azimuth-resolved spectra
         simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
                                 nVacuum, nSubstrate, nAdsorbate,
                                 filmThickness, angle)
         
         # Evaulate new fit quality
-        fitQualityFinal = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, WeightingS)
+        fitQualityFinal = iras.CalculateResidualAbsoluteDifference(dataIRAS, simulatedSpectra, scaleStoP,1)
         
-        if fitQualityInitial < fitQualityFinal:
-            if randomXYZ == 0:
-                kAdsorbateX = kAdsorbateX - kNew
-            if randomXYZ == 1:
-                kAdsorbateY = kAdsorbateY - kNew
-            if randomXYZ == 2:
-                kAdsorbateZ = kAdsorbateZ - kNew
+        if fitQualityInitial < fitQualityFinal+(kAmplitude*cutoffXYZ):
+            kAdsorbateX = kAdsorbateX - kNew*scaleStoP
+            kAdsorbateY = kAdsorbateY - kNew*scaleStoP
+            kAdsorbateZ = kAdsorbateZ + kNew
             kAdsorbate = np.array([kAdsorbateX, kAdsorbateY, kAdsorbateZ])
             simulatedKSpectra = np.array([simulationWavenumber,kAdsorbateX, kAdsorbateY, kAdsorbateZ])
             nAdsorbate = nAdsorbateInf + iras.CalcIndexRefractFromK(kAdsorbate)
     
 # Plots the adsorbate k(w) parameters
 plt.figure(0); plt.clf()
 plt.xlabel("$\mathregular{Wavenumber\ (cm^{-1})}$")
@@ -154,29 +173,37 @@
 plt.plot(simulatedKSpectra[0], simulatedKSpectra[1])
 plt.plot(simulatedKSpectra[0], simulatedKSpectra[2])
 plt.plot(simulatedKSpectra[0], simulatedKSpectra[3])
 plt.xlim(1900, 3000)
 plt.tight_layout()
 plt.ion()
 plt.show()
+plt.savefig("Figure0.png", dpi=300, format='png')
 
 plt.figure(1); plt.clf() 
 plt.xlabel("$\mathregular{Wavenumber\ (cm^{-1})}$")
 plt.ylabel("$\mathregular{\Delta R / R}$")
-plt.scatter(dataIRAS[0], dataIRAS[1], s=1)
+plt.scatter(dataIRAS[0], dataIRAS[1]*scaleStoP, s=1)
 plt.scatter(dataIRAS[0], dataIRAS[2], s=1)
-plt.scatter(dataIRAS[0], dataIRAS[3], s=1)
+plt.scatter(dataIRAS[0], dataIRAS[3]*scaleStoP, s=1)
 plt.scatter(dataIRAS[0], dataIRAS[4], s=1)
-plt.plot(simulatedSpectra[0], simulatedSpectra[1])
+plt.plot(simulatedSpectra[0], simulatedSpectra[1]*scaleStoP)
 plt.plot(simulatedSpectra[0], simulatedSpectra[2])
-plt.plot(simulatedSpectra[0], simulatedSpectra[3])
+plt.plot(simulatedSpectra[0], simulatedSpectra[3]*scaleStoP)
 plt.plot(simulatedSpectra[0], simulatedSpectra[4])
 plt.xlim(1900, 3000)
 plt.tight_layout() 
 plt.ion()
 plt.show()
+plt.savefig("Figure1.png", dpi=300, format='png')
 
-# Exports the 4 polarization- and azimuth-resolved IRAS spectra
-# np.savetxt("SimulatedIRAS.txt", np.transpose(simulatedSpectra.real), 
-#            delimiter = ",", 
-#            header="wavenumber(cm^-1),spol(y),ppol(zx),spol(x),ppol(zy)",comments=''
-#            )
+#Exports the 4 polarization- and azimuth-resolved IRAS spectra
+np.savetxt("SimulatedIRAS.txt", np.transpose(simulatedSpectra.real), 
+            delimiter = ",", 
+            header="wavenumber(cm^-1),spol(y),ppol(zx),spol(x),ppol(zy)",comments=''
+            )
+
+#Exports the 4 polarization- and azimuth-resolved IRAS spectra
+np.savetxt("SimulatedK.txt", np.transpose(simulatedKSpectra), 
+            delimiter = ",", 
+            header="wavenumber(cm^-1),k(x),k(y),k(z)",comments=''
+            )
```

### Comparing `simulateIRAS-0.1.0.post5/examples/simpleSimulation/IRASTestK.txt` & `simulateIRAS-0.1.0.post6/examples/simpleSimulation/IRASTestK.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post5/examples/simpleSimulation/SimulatedIRAS.txt` & `simulateIRAS-0.1.0.post6/examples/simpleSimulation/Solutions/SimulatedIRAS.txt`

 * *Files identical despite different names*

### Comparing `simulateIRAS-0.1.0.post5/examples/simpleSimulation/Solutions/SimulatedIRAS.txt` & `simulateIRAS-0.1.0.post6/examples/dataRegression/Solutions/SimulatedIRAS.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,1501 +1,1557 @@
 wavenumber(cm^-1),spol(y),ppol(zx),spol(x),ppol(zy)
-1.500000000000000000e+03,-4.540424606060542079e-10,1.973697558470914251e-09,-8.010787953238236292e-10,3.709712536854469166e-10
-1.501000000000000000e+03,-4.554098669672962141e-10,1.979460529178253747e-09,-8.035253722765181621e-10,3.717502647285096813e-10
-1.502000000000000000e+03,-4.567568712490491331e-10,1.985156274588768244e-09,-8.059821161943849609e-10,3.723208727158509936e-10
-1.503000000000000000e+03,-4.581148264886488972e-10,1.990960271852509117e-09,-8.084567042921028871e-10,3.729678974223842443e-10
-1.504000000000000000e+03,-4.595058904567836009e-10,1.996632804001991645e-09,-8.109186444888489000e-10,3.736947759642670852e-10
-1.505000000000000000e+03,-4.608641960537059590e-10,2.002579167133739096e-09,-8.134360754295739433e-10,3.742879224636222060e-10
-1.506000000000000000e+03,-4.622581205528917758e-10,2.008228588751838561e-09,-8.159032544202993865e-10,3.749807068848738891e-10
-1.507000000000000000e+03,-4.636595593603457134e-10,2.014105825352949798e-09,-8.184243930138192919e-10,3.756868068611985203e-10
-1.508000000000000000e+03,-4.650149655281919105e-10,2.019767396927733687e-09,-8.208968179253171085e-10,3.761896237342748567e-10
-1.509000000000000000e+03,-4.664186803127486571e-10,2.025615497762615920e-09,-8.234223669025936034e-10,3.768567305624578887e-10
-1.510000000000000000e+03,-4.678183667397787898e-10,2.031409927171910449e-09,-8.259415115035359547e-10,3.774811391902232001e-10
-1.511000000000000000e+03,-4.692245994304310137e-10,2.037458152030315582e-09,-8.285133178360186616e-10,3.781463670853702712e-10
-1.512000000000000000e+03,-4.706271849697639940e-10,2.043229704775232295e-09,-8.310378305160116107e-10,3.787364965598648114e-10
-1.513000000000000000e+03,-4.720360512427065605e-10,2.049217016582170404e-09,-8.336146562034325382e-10,3.793297931319755814e-10
-1.514000000000000000e+03,-4.734831223407609134e-10,2.054965554376041676e-09,-8.361445397069200130e-10,3.800775521839107134e-10
-1.515000000000000000e+03,-4.748947203561055304e-10,2.060963470563933107e-09,-8.387264894074026762e-10,3.806704048554821218e-10
-1.516000000000000000e+03,-4.763447798692413824e-10,2.066845672005623573e-09,-8.413033884168355393e-10,3.813484961758068909e-10
-1.517000000000000000e+03,-4.777591550836793195e-10,2.072783612607892543e-09,-8.438905585622248320e-10,3.818700895604747726e-10
-1.518000000000000000e+03,-4.792122044014783121e-10,2.078871066193472283e-09,-8.465146191648835306e-10,3.825494333843733715e-10
-1.519000000000000000e+03,-4.806711165294880333e-10,2.084784873356980470e-09,-8.491070850260990150e-10,3.832281219036793859e-10
-1.520000000000000000e+03,-4.820854277828026985e-10,2.090849749956858390e-09,-8.517366953565815959e-10,3.836803533586550223e-10
-1.521000000000000000e+03,-4.835472288523736673e-10,2.096932508716621762e-09,-8.543762779011054759e-10,3.843237354239544285e-10
-1.522000000000000000e+03,-4.850062889444194962e-10,2.102939134955894060e-09,-8.570114674219409231e-10,3.848986146535471542e-10
-1.523000000000000000e+03,-4.865128674350795694e-10,2.108998277552912971e-09,-8.596564918324518511e-10,3.857000449023627704e-10
-1.524000000000000000e+03,-4.879749767114148240e-10,2.115175527003370181e-09,-8.623391356629500182e-10,3.862404700777844221e-10
-1.525000000000000000e+03,-4.894426878015074842e-10,2.121211182673716824e-09,-8.649896494490483089e-10,3.868135594269392688e-10
-1.526000000000000000e+03,-4.909078193664660099e-10,2.127365946621946804e-09,-8.676779623641143031e-10,3.873192753383554781e-10
-1.527000000000000000e+03,-4.924204460069620721e-10,2.133536081215293723e-09,-8.703759409949474772e-10,3.880150701427926015e-10
-1.528000000000000000e+03,-4.939306151253376314e-10,2.139668340447619238e-09,-8.730699522778975703e-10,3.886799624510723023e-10
-1.529000000000000000e+03,-4.954043064969655181e-10,2.145815244359245377e-09,-8.757735349200874210e-10,3.891468297378341915e-10
-1.530000000000000000e+03,-4.969175854355886286e-10,2.152119059572788261e-09,-8.785152927412673371e-10,3.897771311922242133e-10
-1.531000000000000000e+03,-4.984363504397394107e-10,2.158437114171415573e-09,-8.812665926580633244e-10,3.904029399697633252e-10
-1.532000000000000000e+03,-4.999527678710318519e-10,2.164488350949780494e-09,-8.839720622868113969e-10,3.909627482031182024e-10
-1.533000000000000000e+03,-5.014746254554083726e-10,2.170783412911733571e-09,-8.867290717918577620e-10,3.915534781524762822e-10
-1.534000000000000000e+03,-5.029941823743089822e-10,2.177201265211052278e-09,-8.895245955785886867e-10,3.920785017807878637e-10
-1.535000000000000000e+03,-5.045613246372697947e-10,2.183437537350812084e-09,-8.922873777494854053e-10,3.927929211927676379e-10
-1.536000000000000000e+03,-5.060840497676188295e-10,2.189833221756268582e-09,-8.950888065108987515e-10,3.932831376673276548e-10
-1.537000000000000000e+03,-5.076543794206766857e-10,2.196082532147073042e-09,-8.978573678896824578e-10,3.939986254755176070e-10
-1.538000000000000000e+03,-5.091802735871946198e-10,2.202419909470284850e-09,-9.006647031871047927e-10,3.944178922060583594e-10
-1.539000000000000000e+03,-5.107537942184879972e-10,2.208805511768346302e-09,-9.034813550724905978e-10,3.950623113428374385e-10
-1.540000000000000000e+03,-5.123251885354752831e-10,2.215316045368128685e-09,-9.063369604095027910e-10,3.956419421039785545e-10
-1.541000000000000000e+03,-5.139019314479022885e-10,2.221678977549190951e-09,-9.091595162915586732e-10,3.962513060919845709e-10
-1.542000000000000000e+03,-5.154765818629700007e-10,2.228167428257715780e-09,-9.120211453310346341e-10,3.967960722675533494e-10
-1.543000000000000000e+03,-5.170565498612272251e-10,2.234667348539376966e-09,-9.148920304619097281e-10,3.973341187084605218e-10
-1.544000000000000000e+03,-5.186344569983463408e-10,2.241133695506279320e-09,-9.177597123317588607e-10,3.978438678076641478e-10
-1.545000000000000000e+03,-5.202176526018065204e-10,2.247611064162122231e-09,-9.206365961895635457e-10,3.983465646842064568e-10
-1.546000000000000000e+03,-5.218413192377033480e-10,2.254251495692106865e-09,-9.235528398784256631e-10,3.990174563231182158e-10
-1.547000000000000000e+03,-5.234277728157899240e-10,2.260866534652927259e-09,-9.264782896193326428e-10,3.994485768942274330e-10
-1.548000000000000000e+03,-5.250547832335800762e-10,2.267252276807857724e-09,-9.293581387840542920e-10,4.000483035387236951e-10
-1.549000000000000000e+03,-5.266870849336053238e-10,2.274041559800101525e-09,-9.323322739481632611e-10,4.006405645641528568e-10
-1.550000000000000000e+03,-5.283174676638271846e-10,2.280601832590691471e-09,-9.352608584535290171e-10,4.012053206730847125e-10
-1.551000000000000000e+03,-5.299531170752338593e-10,2.287172084480817767e-09,-9.381985514408070547e-10,4.017623132002581012e-10
-1.552000000000000000e+03,-5.315868728372962304e-10,2.293870947470065566e-09,-9.411759891675179604e-10,4.022556172477911148e-10
-1.553000000000000000e+03,-5.332258716650856578e-10,2.300615978863406837e-09,-9.441625442274139689e-10,4.027771970762369798e-10
-1.554000000000000000e+03,-5.349057319791461137e-10,2.307293006515132095e-09,-9.471462703700248870e-10,4.034325496113549875e-10
-1.555000000000000000e+03,-5.365481098621898802e-10,2.313979437898298562e-09,-9.501390680443380114e-10,4.038823045850313893e-10
-1.556000000000000000e+03,-5.382314300043201289e-10,2.320795681536848925e-09,-9.531718793838995711e-10,4.044661603614900834e-10
-1.557000000000000000e+03,-5.398771884005526019e-10,2.327657625126043168e-09,-9.562137734745775312e-10,4.048802966789847094e-10
-1.558000000000000000e+03,-5.415639690765009707e-10,2.334254313114494908e-09,-9.592101380709354463e-10,4.054289015487859672e-10
-1.559000000000000000e+03,-5.432559831996929362e-10,2.341255676780495211e-09,-9.623012471596173501e-10,4.059687910699915013e-10
-1.560000000000000000e+03,-5.449462528783137101e-10,2.347991937382670089e-09,-9.653468706406705088e-10,4.064455883994902779e-10
-1.561000000000000000e+03,-5.466417358872093797e-10,2.354971506131906681e-09,-9.684444294901714723e-10,4.069499163562337618e-10
-1.562000000000000000e+03,-5.483784548211209168e-10,2.361685904929200574e-09,-9.714964896183652145e-10,4.075896430775935922e-10
-1.563000000000000000e+03,-5.500774357957851545e-10,2.368606960251487985e-09,-9.746005008293026195e-10,4.080218132503615506e-10
-1.564000000000000000e+03,-5.517747140659584696e-10,2.375696755652351953e-09,-9.777450491701777174e-10,4.084276462519321277e-10
-1.565000000000000000e+03,-5.535202114796539301e-10,2.382559320434328925e-09,-9.808555703996446371e-10,4.089860885045635959e-10
-1.566000000000000000e+03,-5.552640824133905112e-10,2.389591085076979900e-09,-9.840067307163395566e-10,4.095185345258744313e-10
-1.567000000000000000e+03,-5.570131656657207043e-10,2.396630695353963529e-09,-9.871668756618222974e-10,4.100414044300389700e-10
-1.568000000000000000e+03,-5.587606417120998786e-10,2.403641030979769816e-09,-9.903246770108121589e-10,4.105384005732894325e-10
-1.569000000000000000e+03,-5.605133118142745951e-10,2.410622124731164182e-09,-9.934914222812257491e-10,4.109888367469299996e-10
-1.570000000000000000e+03,-5.622643935399814634e-10,2.417574126888090236e-09,-9.966558665772628579e-10,4.114134723342739399e-10
-1.571000000000000000e+03,-5.640206514708692829e-10,2.424732859448546068e-09,-9.998724405425278017e-10,4.118279920056102931e-10
-1.572000000000000000e+03,-5.658185846438816030e-10,2.431862986517714996e-09,-1.003086812055035678e-09,4.124165476060097966e-10
-1.573000000000000000e+03,-5.676217329311542090e-10,2.438963303293936845e-09,-1.006310104230625007e-09,4.129581794876467561e-10
-1.574000000000000000e+03,-5.693800842034736862e-10,2.446235224635072057e-09,-1.009574548594914886e-09,4.132744746465264824e-10
-1.575000000000000000e+03,-5.711869078110669520e-10,2.453477159087156413e-09,-1.012847929865758465e-09,4.137433703437861672e-10
-1.576000000000000000e+03,-5.729922537598444193e-10,2.460490810507211166e-09,-1.016075879791128748e-09,4.141869753840226434e-10
-1.577000000000000000e+03,-5.748027815340677580e-10,2.467911555143432715e-09,-1.019399468153182934e-09,4.146199156832056342e-10
-1.578000000000000000e+03,-5.766552652483093342e-10,2.475104227504339314e-09,-1.022677664653450479e-09,4.152281841744401989e-10
-1.579000000000000000e+03,-5.784695261096689156e-10,2.482466792939867292e-09,-1.026008176548864361e-09,4.155882107579100236e-10
-1.580000000000000000e+03,-5.803258172962753737e-10,2.489601190702870558e-09,-1.029293279846012471e-09,4.161238909658088614e-10
-1.581000000000000000e+03,-5.821438120692366934e-10,2.496905319264811023e-09,-1.032630717476595257e-09,4.164107397996517379e-10
-1.582000000000000000e+03,-5.840039114083059036e-10,2.504420396785720529e-09,-1.036009814346635600e-09,4.169105942553126355e-10
-1.583000000000000000e+03,-5.858691997976655400e-10,2.511703158268099211e-09,-1.039354234845410159e-09,4.173622441137737529e-10
-1.584000000000000000e+03,-5.877331356606260412e-10,2.519123253218347266e-09,-1.042740414019945189e-09,4.177521259316457018e-10
-1.585000000000000000e+03,-5.896022449299439884e-10,2.526548876768353517e-09,-1.046135448552887084e-09,4.181305319010042698e-10
-1.586000000000000000e+03,-5.914700181487245132e-10,2.534112485312890844e-09,-1.049572396772877744e-09,4.184471815549210751e-10
-1.587000000000000000e+03,-5.933866221613103336e-10,2.541516884507017527e-09,-1.052974531926832710e-09,4.189909163209647968e-10
-1.588000000000000000e+03,-5.953019624746653261e-10,2.549059707440287563e-09,-1.056418679820711157e-09,4.194732101996821544e-10
-1.589000000000000000e+03,-5.971787722509858184e-10,2.556570410412578622e-09,-1.059871661147444404e-09,4.197046419488163771e-10
-1.590000000000000000e+03,-5.990980366298686795e-10,2.564055196671268521e-09,-1.063323038187152729e-09,4.201136352205925987e-10
-1.591000000000000000e+03,-6.010224845225860557e-10,2.571746955411341737e-09,-1.066827011094007410e-09,4.205106353548192420e-10
-1.592000000000000000e+03,-6.029457013298894406e-10,2.579376017778285821e-09,-1.070329476800014085e-09,4.208462143065076900e-10
-1.593000000000000000e+03,-6.049179305471421291e-10,2.587009645225262905e-09,-1.073840755290827644e-09,4.213720132400714466e-10
-1.594000000000000000e+03,-6.068451282615894149e-10,2.594580701706731854e-09,-1.077350567928526605e-09,4.216340409136374024e-10
-1.595000000000000000e+03,-6.088213808118916452e-10,2.602396078101849561e-09,-1.080913069980504562e-09,4.221236028393396865e-10
-1.596000000000000000e+03,-6.107525601425951992e-10,2.609909019054864584e-09,-1.084430258780492862e-09,4.223118378703395954e-10
-1.597000000000000000e+03,-6.127328367295223986e-10,2.617628844818509864e-09,-1.088000156261601947e-09,4.226902789809515063e-10
-1.598000000000000000e+03,-6.147119847802415742e-10,2.625489822769850908e-09,-1.091612728108370990e-09,4.230075762772963946e-10
-1.599000000000000000e+03,-6.166963141005327709e-10,2.633188801634872553e-09,-1.095190077865702342e-09,4.233494702982142835e-10
-1.600000000000000000e+03,-6.187235737883084210e-10,2.640991942677564571e-09,-1.098810202337696075e-09,4.237962453519984864e-10
-1.601000000000000000e+03,-6.207119845171428010e-10,2.649039704255381540e-09,-1.102483183775199585e-09,4.240641132502368920e-10
-1.602000000000000000e+03,-6.227433983729721418e-10,2.656785002550281728e-09,-1.106110917672356752e-09,4.244370880586848546e-10
-1.603000000000000000e+03,-6.247800203101027465e-10,2.664774851253414361e-09,-1.109791527557725400e-09,4.248344674270596970e-10
-1.604000000000000000e+03,-6.268156166405001810e-10,2.672666063450411314e-09,-1.113471048036598314e-09,4.251335049372862780e-10
-1.605000000000000000e+03,-6.288564067705791183e-10,2.680560319182208998e-09,-1.117159315497099406e-09,4.254191762361217614e-10
-1.606000000000000000e+03,-6.308961862980950800e-10,2.688431116428932272e-09,-1.120846535896313146e-09,4.256815574280950324e-10
-1.607000000000000000e+03,-6.329411452781440523e-10,2.696471435494597115e-09,-1.124586724287153048e-09,4.258927574721732769e-10
-1.608000000000000000e+03,-6.350293801542876480e-10,2.704693273301949477e-09,-1.128370253450717701e-09,4.262851766366263133e-10
-1.609000000000000000e+03,-6.371228364711553835e-10,2.712675636210943488e-09,-1.132118244743950330e-09,4.266263606155716528e-10
-1.610000000000000000e+03,-6.392153687550676841e-10,2.720802304814363076e-09,-1.135909677706179028e-09,4.269069550937264481e-10
-1.611000000000000000e+03,-6.412687517748136260e-10,2.728931372236840003e-09,-1.139709849915043113e-09,4.269687837223424511e-10
-1.612000000000000000e+03,-6.434099399675317089e-10,2.737000330965127436e-09,-1.143509216064605056e-09,4.273797390556522589e-10
-1.613000000000000000e+03,-6.455119634883843436e-10,2.745071298541239190e-09,-1.147317281169741753e-09,4.275716534876208976e-10
-1.614000000000000000e+03,-6.476575357514022813e-10,2.753287631552838558e-09,-1.151169045101805514e-09,4.279082402149889885e-10
-1.615000000000000000e+03,-6.497638720062011659e-10,2.761505840445025225e-09,-1.155029523415141535e-09,4.280252523784985581e-10
-1.616000000000000000e+03,-6.519138292724747747e-10,2.769870079170163740e-09,-1.158933858164215400e-09,4.282872071093850961e-10
-1.617000000000000000e+03,-6.540690065417319094e-10,2.778030321814535600e-09,-1.162802374352615664e-09,4.285346951514000000e-10
-1.618000000000000000e+03,-6.562233773295040505e-10,2.786299163907533970e-09,-1.166714849284118288e-09,4.286840423217670611e-10
-1.619000000000000000e+03,-6.584275385297054570e-10,2.794813165580264020e-09,-1.170680616794011526e-09,4.290623749340369962e-10
-1.620000000000000000e+03,-6.605863513368441890e-10,2.803024378902077564e-09,-1.174601288925051926e-09,4.291367506937396571e-10
-1.621000000000000000e+03,-6.627949978511257873e-10,2.811442760815802592e-09,-1.178575270343335685e-09,4.294022436896487243e-10
-1.622000000000000000e+03,-6.650029235111108599e-10,2.819802469923084367e-09,-1.182548834551840675e-09,4.296076615502876319e-10
-1.623000000000000000e+03,-6.672160837271422599e-10,2.828369474394925305e-09,-1.186575780019172878e-09,4.297980176926216340e-10
-1.624000000000000000e+03,-6.694285381083460342e-10,2.836878211901971039e-09,-1.190602409451308338e-09,4.299283066490894796e-10
-1.625000000000000000e+03,-6.716462128451447131e-10,2.845349572882937692e-09,-1.194637713887886249e-09,4.300052643910849994e-10
-1.626000000000000000e+03,-6.739079804614005180e-10,2.853762770637333574e-09,-1.198672747968330477e-09,4.302289427112684591e-10
-1.627000000000000000e+03,-6.761301981252468224e-10,2.862421245074800485e-09,-1.202761249147340856e-09,4.302683148164881660e-10
-1.628000000000000000e+03,-6.783965811648873546e-10,2.870945882881948691e-09,-1.206849582115153574e-09,4.303785971693053654e-10
-1.629000000000000000e+03,-6.806682119475761512e-10,2.879715915290315744e-09,-1.210991452919942826e-09,4.305112548136703314e-10
-1.630000000000000000e+03,-6.829841364765022641e-10,2.888183039215306016e-09,-1.215088336788719671e-09,4.307533311105686404e-10
-1.631000000000000000e+03,-6.852604248462408764e-10,2.897103055919278815e-09,-1.219283723110996070e-09,4.308103312877726715e-10
-1.632000000000000000e+03,-6.875810794216420062e-10,2.905720266114905476e-09,-1.223434167025738051e-09,4.309769810867129589e-10
-1.633000000000000000e+03,-6.899070091905307379e-10,2.914544759924086591e-09,-1.227638234106365359e-09,4.311276278879995278e-10
-1.634000000000000000e+03,-6.922324221890890541e-10,2.923274240190438737e-09,-1.231842384172034944e-09,4.311804912817015888e-10
-1.635000000000000000e+03,-6.945630961042749121e-10,2.932002944940855341e-09,-1.236055161835901021e-09,4.312170307324870855e-10
-1.636000000000000000e+03,-6.968932685597569039e-10,2.940883213143486414e-09,-1.240313164207690599e-09,4.311939553687128383e-10
-1.637000000000000000e+03,-6.992737840997540199e-10,2.949762545935148797e-09,-1.244579804932238313e-09,4.313625505661221874e-10
-1.638000000000000000e+03,-7.016087443789682156e-10,2.958547321936904965e-09,-1.248846681662416290e-09,4.312251100595540585e-10
-1.639000000000000000e+03,-7.039940908315742721e-10,2.967539352897040936e-09,-1.253167331493075298e-09,4.312792825840062838e-10
-1.640000000000000000e+03,-7.064242042843269975e-10,2.976437163858034769e-09,-1.257488321971499097e-09,4.314444104078813752e-10
-1.641000000000000000e+03,-7.088144376582930289e-10,2.985580648422392185e-09,-1.261863154195471849e-09,4.314223740652138680e-10
-1.642000000000000000e+03,-7.112042720825126824e-10,2.994630299131904263e-09,-1.266238432135263146e-09,4.313026029282775307e-10
-1.643000000000000000e+03,-7.136446332663553718e-10,3.003639774454676333e-09,-1.270622324799678175e-09,4.313362197703383136e-10
-1.644000000000000000e+03,-7.160846669084750081e-10,3.012632308678053215e-09,-1.275006712976248732e-09,4.313490943833516034e-10
-1.645000000000000000e+03,-7.185300020407340832e-10,3.021755195688364728e-09,-1.279445021226816492e-09,4.312677854006371829e-10
-1.646000000000000000e+03,-7.210203779382678278e-10,3.030861577732549072e-09,-1.283883931205207785e-09,4.313752053341221911e-10
-1.647000000000000000e+03,-7.234707155182657375e-10,3.040136768082012274e-09,-1.288376828439361847e-09,4.312171929917932438e-10
-1.648000000000000000e+03,-7.259661669403878775e-10,3.049357421906153751e-09,-1.292870434016267058e-09,4.312097231167493361e-10
-1.649000000000000000e+03,-7.284669460049101964e-10,3.058536904346731871e-09,-1.297372626330154037e-09,4.311460303027494495e-10
-1.650000000000000000e+03,-7.309675013454485977e-10,3.067833543593030832e-09,-1.301921074328012035e-09,4.309848373196588956e-10
-1.651000000000000000e+03,-7.334733697187609392e-10,3.077165863054139209e-09,-1.306478116559222840e-09,4.308441709033204669e-10
-1.652000000000000000e+03,-7.360245536490226006e-10,3.086405632021232854e-09,-1.311036027152957603e-09,4.308162255468453841e-10
-1.653000000000000000e+03,-7.385810917310855805e-10,3.095813940064156602e-09,-1.315648065933598085e-09,4.307315649592809104e-10
-1.654000000000000000e+03,-7.411374943529211063e-10,3.105379308554612629e-09,-1.320306691841273544e-09,4.305881847635565114e-10
-1.655000000000000000e+03,-7.436992363861684156e-10,3.114691910724352709e-09,-1.324928287868204939e-09,4.303877133746450058e-10
-1.656000000000000000e+03,-7.463064959764598090e-10,3.124161994210809714e-09,-1.329596582409345416e-09,4.303392692593907038e-10
-1.657000000000000000e+03,-7.488734702943651144e-10,3.133589547159597840e-09,-1.334273436097178448e-09,4.300227152435356486e-10
-1.658000000000000000e+03,-7.514860358248754409e-10,3.143175263043921955e-09,-1.338997155889002511e-09,4.298584363014710451e-10
-1.659000000000000000e+03,-7.541039658440699800e-10,3.152718165781618099e-09,-1.343729440794075871e-09,4.296365626908749428e-10
-1.660000000000000000e+03,-7.567218659476330855e-10,3.162419918507539920e-09,-1.348508760318637817e-09,4.293561797867462169e-10
-1.661000000000000000e+03,-7.593908946765919813e-10,3.172078570339368330e-09,-1.353296649987047011e-09,4.292292448540033174e-10
-1.662000000000000000e+03,-7.620599658932943694e-10,3.181646223379494145e-09,-1.358085902799077188e-09,4.290052119125526391e-10
-1.663000000000000000e+03,-7.647344275000418036e-10,3.191420875199930792e-09,-1.362929543738700430e-09,4.287618903140824108e-10
-1.664000000000000000e+03,-7.674089484182542894e-10,3.201104909780989657e-09,-1.367774659315481366e-09,4.284214150433310824e-10
-1.665000000000000000e+03,-7.701347369687197467e-10,3.210995961946589216e-09,-1.372674225197459054e-09,4.282732587416259599e-10
-1.666000000000000000e+03,-7.728147360507238382e-10,3.220757859081132963e-09,-1.377575377852531812e-09,4.277771485657246698e-10
-1.667000000000000000e+03,-7.755460446817733153e-10,3.230553317431363984e-09,-1.382485057980617792e-09,4.275121811028052032e-10
-1.668000000000000000e+03,-7.783234799176658017e-10,3.240432212838212882e-09,-1.387442395126165244e-09,4.273235827548661995e-10
-1.669000000000000000e+03,-7.810603647494530536e-10,3.250305463007718206e-09,-1.392408262093051351e-09,4.269026707764053170e-10
-1.670000000000000000e+03,-7.838434505303006494e-10,3.260301738290350744e-09,-1.397421958173877578e-09,4.265972645178016505e-10
-1.671000000000000000e+03,-7.865859127900814976e-10,3.270292105996796534e-09,-1.402444186099744378e-09,4.260589352658881986e-10
-1.672000000000000000e+03,-7.894207424175469451e-10,3.280367110269337105e-09,-1.407514415962637594e-09,4.258101365223632404e-10
-1.673000000000000000e+03,-7.922149311785067977e-10,3.290435891933486866e-09,-1.412593178664883631e-09,4.253280150544115959e-10
-1.674000000000000000e+03,-7.950555263883649241e-10,3.300415699547947385e-09,-1.417673931441064699e-09,4.249620487563780282e-10
-1.675000000000000000e+03,-7.979015847052271927e-10,3.310563059151386078e-09,-1.422809375750965409e-09,4.245362816126306221e-10
-1.676000000000000000e+03,-8.007479742470732470e-10,3.320660958729416379e-09,-1.427946926146242857e-09,4.240528575627605813e-10
-1.677000000000000000e+03,-8.035998107938128473e-10,3.330887185566915713e-09,-1.433139225987259331e-09,4.234700661164165320e-10
-1.678000000000000000e+03,-8.064982588405550595e-10,3.341064368765320715e-09,-1.438333749105118058e-09,4.230432302364352937e-10
-1.679000000000000000e+03,-8.094021932030959858e-10,3.351408947161675505e-09,-1.443583078796894298e-09,4.225560126125157512e-10
-1.680000000000000000e+03,-8.123065510101104640e-10,3.361665711094016413e-09,-1.448834749801804542e-09,4.219721231853254821e-10
-1.681000000000000000e+03,-8.152627262911023521e-10,3.372089760587998289e-09,-1.454141283763328735e-09,4.215414542935996401e-10
-1.682000000000000000e+03,-8.181730226328370900e-10,3.382465663193163567e-09,-1.459450277853114104e-09,4.208393930274670196e-10
-1.683000000000000000e+03,-8.211351772290684601e-10,3.392969476758853531e-09,-1.464814190571042360e-09,4.202511089241733969e-10
-1.684000000000000000e+03,-8.241442799439153441e-10,3.403386244677756792e-09,-1.470180682691665890e-09,4.197806882887909887e-10
-1.685000000000000000e+03,-8.271124699337378617e-10,3.413794658759053856e-09,-1.475555646690232695e-09,4.190738397085404557e-10
-1.686000000000000000e+03,-8.301276841641757976e-10,3.424291728307783706e-09,-1.480979785320145741e-09,4.184457153941618773e-10
-1.687000000000000000e+03,-8.331484293341029583e-10,3.434995118788742062e-09,-1.486458950463624941e-09,4.177953254041884198e-10
-1.688000000000000000e+03,-8.361697839085251440e-10,3.445572888233509867e-09,-1.491940937567961581e-09,4.170090960754220549e-10
-1.689000000000000000e+03,-8.392432274595597025e-10,3.456102162283110508e-09,-1.497431388283690450e-09,4.163758474316555183e-10
-1.690000000000000000e+03,-8.423173550546386372e-10,3.466800226881781849e-09,-1.502971372885003249e-09,4.156857849313441428e-10
-1.691000000000000000e+03,-8.453970355052823698e-10,3.477625505912065317e-09,-1.508566489120710080e-09,4.148939659883037469e-10
-1.692000000000000000e+03,-8.485240797416540825e-10,3.488365358480128448e-09,-1.514164673373575882e-09,4.142212928032245200e-10
-1.693000000000000000e+03,-8.516567149048016247e-10,3.499055907215524243e-09,-1.519771309704364676e-09,4.134861020618793367e-10
-1.694000000000000000e+03,-8.547901290276332277e-10,3.509877145895237189e-09,-1.525427842847446080e-09,4.126547590972290116e-10
-1.695000000000000000e+03,-8.579291163403954567e-10,3.520825173117884770e-09,-1.531139609338807517e-09,4.117208579641652615e-10
-1.696000000000000000e+03,-8.611156763310451578e-10,3.531728175270572434e-09,-1.536854693694922044e-09,4.109463148358460968e-10
-1.697000000000000000e+03,-8.643078471196184753e-10,3.542541418764122029e-09,-1.542578215057931668e-09,4.100689606990859880e-10
-1.698000000000000000e+03,-8.675008927843817456e-10,3.553486696593629377e-09,-1.548352000126178700e-09,4.090955472736169318e-10
-1.699000000000000000e+03,-8.707463905191458564e-10,3.564597982727688012e-09,-1.554181116594985381e-09,4.082748444706839219e-10
-1.700000000000000000e+03,-8.739928388551718307e-10,3.575585827567841145e-09,-1.560013805241936646e-09,4.073185930818711357e-10
-1.701000000000000000e+03,-8.772449179217194220e-10,3.586779185426480969e-09,-1.565901873726066499e-09,4.063380972080723678e-10
-1.702000000000000000e+03,-8.805449126903978027e-10,3.597849503314159286e-09,-1.571793642449086258e-09,4.054387627074533474e-10
-1.703000000000000000e+03,-8.838505751860423087e-10,3.609045693443489707e-09,-1.577740838502625446e-09,4.044354944669439708e-10
-1.704000000000000000e+03,-8.871572855251248255e-10,3.620376222366528968e-09,-1.583738911833699417e-09,4.033364365385123220e-10
-1.705000000000000000e+03,-8.904696448215209945e-10,3.631655001590559862e-09,-1.589745437583789683e-09,4.021726816160315512e-10
-1.706000000000000000e+03,-8.938301310699626345e-10,3.642851302371981031e-09,-1.595755924032767186e-09,4.011304223269637519e-10
-1.707000000000000000e+03,-8.971963029863654329e-10,3.654172977124207800e-09,-1.601821928424118023e-09,3.999833954095739048e-10
-1.708000000000000000e+03,-9.006107362607771316e-10,3.665590535014155500e-09,-1.607939187323921249e-09,3.989184282907609140e-10
-1.709000000000000000e+03,-9.040308917529016634e-10,3.676955345995584590e-09,-1.614064872649194482e-09,3.977882253552875988e-10
-1.710000000000000000e+03,-9.074522709638533740e-10,3.688456613413800335e-09,-1.620242003857176901e-09,3.965625366214960935e-10
-1.711000000000000000e+03,-9.108793529567790834e-10,3.700082942603242619e-09,-1.626474795720952039e-09,3.952311880010247499e-10
-1.712000000000000000e+03,-9.143549091078191265e-10,3.711588382644388287e-09,-1.632712002611076933e-09,3.939824295869522077e-10
-1.713000000000000000e+03,-9.178362039933433802e-10,3.723040055168694320e-09,-1.638957606586996748e-09,3.926676265278365754e-10
-1.714000000000000000e+03,-9.213661083274448697e-10,3.734808201448820176e-09,-1.645302375198356698e-09,3.914358169813439267e-10
-1.715000000000000000e+03,-9.249017871134698033e-10,3.746263538609258649e-09,-1.651608215037636983e-09,3.900976522966356440e-10
-1.716000000000000000e+03,-9.284388683391933658e-10,3.758076304610253892e-09,-1.658013472703881054e-09,3.886642496169760235e-10
-1.717000000000000000e+03,-9.320290747492553462e-10,3.769834499089542344e-09,-1.664427146886006755e-09,3.873827545413325168e-10
-1.718000000000000000e+03,-9.356207617216742836e-10,3.781652090551952466e-09,-1.670893097825138231e-09,3.859260631535227451e-10
-1.719000000000000000e+03,-9.392182387330556459e-10,3.793414525244410187e-09,-1.677367446309829810e-09,3.844021726849264581e-10
-1.720000000000000000e+03,-9.428646755896503544e-10,3.805277105501745160e-09,-1.683894268679675254e-09,3.829621988054891748e-10
-1.721000000000000000e+03,-9.465169370396129956e-10,3.817263356606918140e-09,-1.690477004803362971e-09,3.814145677916427985e-10
-1.722000000000000000e+03,-9.501707818661097406e-10,3.829130999422024400e-09,-1.697064903578679916e-09,3.797317982349196115e-10
-1.723000000000000000e+03,-9.538779715886701313e-10,3.841140694999875641e-09,-1.703756347332516225e-09,3.779592411850236826e-10
-1.724000000000000000e+03,-9.575868240755227022e-10,3.853093889445471495e-09,-1.710405527545927623e-09,3.763330489192016473e-10
-1.725000000000000000e+03,-9.613491132427609588e-10,3.865510931397685871e-09,-1.717158346640961585e-09,3.749388541188581741e-10
-1.726000000000000000e+03,-9.651131448322407814e-10,3.877308505301930418e-09,-1.723868986373827564e-09,3.731280363106315090e-10
-1.727000000000000000e+03,-9.688830494133540058e-10,3.889569748240736312e-09,-1.730683358081470312e-09,3.713289430263959692e-10
-1.728000000000000000e+03,-9.727024044243226424e-10,3.902055342915997350e-09,-1.737551112804125985e-09,3.697360395253951419e-10
-1.729000000000000000e+03,-9.765276660105020113e-10,3.914160745207450658e-09,-1.744427267844696522e-09,3.677514267282915637e-10
-1.730000000000000000e+03,-9.804025159844288682e-10,3.926491144537848594e-09,-1.751357010430819607e-09,3.659733415628398099e-10
-1.731000000000000000e+03,-9.842833058261559174e-10,3.938844074610336796e-09,-1.758295126369330208e-09,3.642065485187084437e-10
-1.732000000000000000e+03,-9.881660250566942202e-10,3.951019000203052535e-09,-1.765287035304596788e-09,3.620222280388513042e-10
-1.733000000000000000e+03,-9.921024871909182602e-10,3.963436848154473141e-09,-1.772335172272948284e-09,3.600693527844427925e-10
-1.734000000000000000e+03,-9.960409598651144921e-10,3.976081748440366593e-09,-1.779437364467297502e-09,3.581031706312705786e-10
-1.735000000000000000e+03,-1.000033265621176943e-09,3.988343608192664185e-09,-1.786547930015469394e-09,3.559638957068981704e-10
-1.736000000000000000e+03,-1.004027663646186306e-09,4.001238226064633542e-09,-1.793712759589903801e-09,3.542164328125474783e-10
-1.737000000000000000e+03,-1.008075984629951550e-09,4.013565481951868678e-09,-1.800933929669264484e-09,3.518904429214636370e-10
-1.738000000000000000e+03,-1.012126479713487521e-09,4.026526884125459400e-09,-1.808209629557729801e-09,3.499568036770299560e-10
-1.739000000000000000e+03,-1.016182991047940831e-09,4.039325497797616897e-09,-1.815541752446517830e-09,3.476275812202677397e-10
-1.740000000000000000e+03,-1.020289727825184836e-09,4.052132132038443437e-09,-1.822880588467597827e-09,3.455073332889829491e-10
-1.741000000000000000e+03,-1.024402512461830654e-09,4.064775025455646821e-09,-1.830275873173810138e-09,3.429905771806324513e-10
-1.742000000000000000e+03,-1.028565662750596392e-09,4.077648712181408161e-09,-1.837726166902615083e-09,3.406831697905908667e-10
-1.743000000000000000e+03,-1.032734892455397013e-09,4.090542088745401749e-09,-1.845184817947712372e-09,3.383849321568857141e-10
-1.744000000000000000e+03,-1.036954628376322181e-09,4.103260624736887441e-09,-1.852698693893865237e-09,3.358900615338361747e-10
-1.745000000000000000e+03,-1.041180474954907762e-09,4.116443511770902729e-09,-1.860317346782172111e-09,3.334038690633838883e-10
-1.746000000000000000e+03,-1.045456968719770883e-09,4.129636778155649396e-09,-1.867943295562966675e-09,3.311282662731039596e-10
-1.747000000000000000e+03,-1.049739604013824039e-09,4.142664349900591899e-09,-1.875625871039310327e-09,3.284538119772138017e-10
-1.748000000000000000e+03,-1.054073027903757356e-09,4.155702778687015395e-09,-1.883315902742073541e-09,3.259903376535616680e-10
-1.749000000000000000e+03,-1.058412623773765413e-09,4.168797787116726520e-09,-1.891110923518569135e-09,3.231270735976464809e-10
-1.750000000000000000e+03,-1.062803150134898332e-09,4.181904395719233582e-09,-1.898913617498733221e-09,3.204751858922518293e-10
-1.751000000000000000e+03,-1.067199878258983002e-09,4.195251985854968934e-09,-1.906773031976762807e-09,3.178309678238047061e-10
-1.752000000000000000e+03,-1.071599313401555822e-09,4.208427180785394306e-09,-1.914688713257718881e-09,3.147669981011364021e-10
-1.753000000000000000e+03,-1.076053318627476503e-09,4.221843042599559283e-09,-1.922661186820548699e-09,3.119334324289682590e-10
-1.754000000000000000e+03,-1.080558538839120614e-09,4.235087112349964546e-09,-1.930690207111639140e-09,3.089034509774248414e-10
-1.755000000000000000e+03,-1.085070020355036820e-09,4.248571525692595858e-09,-1.938776090464913920e-09,3.058801177947041746e-10
-1.756000000000000000e+03,-1.089632860479319744e-09,4.262294290193131013e-09,-1.946918801706963464e-09,3.030698768597943016e-10
-1.757000000000000000e+03,-1.094201990643320261e-09,4.275623446977695899e-09,-1.955069871381703875e-09,2.998564756995767325e-10
-1.758000000000000000e+03,-1.098822623312504965e-09,4.289416229730436126e-09,-1.963326599408250534e-09,2.968565912502170167e-10
-1.759000000000000000e+03,-1.103449574310802232e-09,4.302814345880387529e-09,-1.971591694329666909e-09,2.934525792572452358e-10
-1.760000000000000000e+03,-1.108128172267905791e-09,4.316677445260340746e-09,-1.979962791677764724e-09,2.902625193212906513e-10
-1.761000000000000000e+03,-1.112813116320362368e-09,4.330144807161386857e-09,-1.988342262657635271e-09,2.866673580859033695e-10
-1.762000000000000000e+03,-1.117549852661354449e-09,4.343853524381856959e-09,-1.996779364046285331e-09,2.832865898379038980e-10
-1.763000000000000000e+03,-1.122341640986480440e-09,4.357801401964259083e-09,-2.005273536170211765e-09,2.801356587045724278e-10
-1.764000000000000000e+03,-1.127136715904154985e-09,4.371806145801017421e-09,-2.013874403575273081e-09,2.765640189760458311e-10
-1.765000000000000000e+03,-1.131986927264033650e-09,4.385824525167736774e-09,-2.022483654405105431e-09,2.732219353695707010e-10
-1.766000000000000000e+03,-1.136840514011711585e-09,4.399675209947323705e-09,-2.031151118545459955e-09,2.694588978700751448e-10
-1.767000000000000000e+03,-1.141749320862021855e-09,4.413577928266004087e-09,-2.039924636531108617e-09,2.655131272054851041e-10
-1.768000000000000000e+03,-1.146661592514498676e-09,4.427499873990564020e-09,-2.048707825362549727e-09,2.615579224252800246e-10
-1.769000000000000000e+03,-1.151629167667370429e-09,4.441659809695018431e-09,-2.057548266018988720e-09,2.578317096302946187e-10
-1.770000000000000000e+03,-1.156649175398335108e-09,4.455879516202688074e-09,-2.066496457163086272e-09,2.539097915977826919e-10
-1.771000000000000000e+03,-1.161675718787972185e-09,4.470110847724379240e-09,-2.075453033701712193e-09,2.499909558994175164e-10
-1.772000000000000000e+03,-1.166754843435944669e-09,4.484402964236787557e-09,-2.084517719243327365e-09,2.458764600645602386e-10
-1.773000000000000000e+03,-1.171889491409899344e-09,4.498932457655290474e-09,-2.093639820452559037e-09,2.419906016886269688e-10
-1.774000000000000000e+03,-1.177027933610010684e-09,4.513070833186871492e-09,-2.102772317476974396e-09,2.376831371473704931e-10
-1.775000000000000000e+03,-1.182221980971506267e-09,4.527258809107237418e-09,-2.112011320902001701e-09,2.331901945696878120e-10
-1.776000000000000000e+03,-1.187419914744381911e-09,4.541696586119971663e-09,-2.121310086260146647e-09,2.286890018098437592e-10
-1.777000000000000000e+03,-1.192722611835378574e-09,4.556370848403075214e-09,-2.130666372095802916e-09,2.246424770746886329e-10
-1.778000000000000000e+03,-1.198029343313086039e-09,4.571109267818090072e-09,-2.140131906097403808e-09,2.201741981280651694e-10
-1.779000000000000000e+03,-1.203342764536447070e-09,4.585441980476878689e-09,-2.149605855300747388e-09,2.152922437095958509e-10
-1.780000000000000000e+03,-1.208709420461221183e-09,4.600254398901374970e-09,-2.159189421011431131e-09,2.106296055977770869e-10
-1.781000000000000000e+03,-1.214131979176802215e-09,4.614887432464631270e-09,-2.168830655195979319e-09,2.057794281279130307e-10
-1.782000000000000000e+03,-1.219607979711739744e-09,4.629774309144290546e-09,-2.178532635995082742e-09,2.011493578619701054e-10
-1.783000000000000000e+03,-1.225090770806630626e-09,4.644480855707917149e-09,-2.188292329743884551e-09,1.961037813748364859e-10
-1.784000000000000000e+03,-1.230627156366143957e-09,4.659254640077435691e-09,-2.198162436950561758e-09,1.908630341617313945e-10
-1.785000000000000000e+03,-1.236219658531948213e-09,4.674034901011223077e-09,-2.208040971611038195e-09,1.858490074801797272e-10
-1.786000000000000000e+03,-1.241865963673621977e-09,4.688883554157774482e-09,-2.218030296903442484e-09,1.806401855400073946e-10
-1.787000000000000000e+03,-1.247519158123771182e-09,4.704194521169369453e-09,-2.228126908699101245e-09,1.754300106700769401e-10
-1.788000000000000000e+03,-1.253226309784036094e-09,4.719118637630803223e-09,-2.238235863485776821e-09,1.700251732053387000e-10
-1.789000000000000000e+03,-1.258989788974990983e-09,4.734087834614709723e-09,-2.248452201151361694e-09,1.644296261125769276e-10
-1.790000000000000000e+03,-1.264757989009515555e-09,4.749316260490855367e-09,-2.258730672559559033e-09,1.588281565306984574e-10
-1.791000000000000000e+03,-1.270632069241553654e-09,4.764589281635541297e-09,-2.269116675069852810e-09,1.532636578047683933e-10
-1.792000000000000000e+03,-1.276511023625037727e-09,4.779705550625969816e-09,-2.279565193793083946e-09,1.472761971967431278e-10
-1.793000000000000000e+03,-1.282446516032715078e-09,4.795283281427579465e-09,-2.290121389206444006e-09,1.415140234611746596e-10
-1.794000000000000000e+03,-1.288436542015309801e-09,4.810476224141499594e-09,-2.300690843640694703e-09,1.355576809098478798e-10
-1.795000000000000000e+03,-1.294433648330678150e-09,4.825711998051285409e-09,-2.311368063442467726e-09,1.291791734212815294e-10
-1.796000000000000000e+03,-1.300535063345873464e-09,4.841022291648017540e-09,-2.322158215599866606e-09,1.228353587813495412e-10
-1.797000000000000000e+03,-1.306643631550586234e-09,4.856563740051263837e-09,-2.333006600222752442e-09,1.164867982913240449e-10
-1.798000000000000000e+03,-1.312807105497836549e-09,4.872181255769210481e-09,-2.343968368526934121e-09,1.099442350359522219e-10
-1.799000000000000000e+03,-1.319027452821643720e-09,4.888029529096712463e-09,-2.354988447999846957e-09,1.036257891997283948e-10
-1.800000000000000000e+03,-1.325302920394179421e-09,4.903305960987268900e-09,-2.366072549481106567e-09,9.669439071465068285e-11
-1.801000000000000000e+03,-1.331635391090545928e-09,4.919042209278749093e-09,-2.377264828423664166e-09,8.998646894907136997e-11
-1.802000000000000000e+03,-1.338023197423104590e-09,4.934857231439230907e-09,-2.388571400550449598e-09,8.308503598131105411e-11
-1.803000000000000000e+03,-1.344418318949902234e-09,4.950481608949943002e-09,-2.399936435988295365e-09,7.575673977780090589e-11
-1.804000000000000000e+03,-1.350918782578816073e-09,4.966606232508117945e-09,-2.411416226073235379e-09,6.888521943744903233e-11
-1.805000000000000000e+03,-1.357426631639980500e-09,4.982118782175737819e-09,-2.422954550202014045e-09,6.116540433556931597e-11
-1.806000000000000000e+03,-1.364040098121534875e-09,4.998133201936508161e-09,-2.434608094055757640e-09,5.390311277119530574e-11
-1.807000000000000000e+03,-1.370661019740480453e-09,5.014185710905933737e-09,-2.446370258529166600e-09,4.621169541993943186e-11
-1.808000000000000000e+03,-1.377387835202840516e-09,5.030321265812535179e-09,-2.458248166389863048e-09,3.855783561897722113e-11
-1.809000000000000000e+03,-1.384122174237248531e-09,5.046262756668394628e-09,-2.470184798504035719e-09,3.047345042089918407e-11
-1.810000000000000000e+03,-1.390912668761522657e-09,5.062710202076335675e-09,-2.482237646669591746e-09,2.261764062985719093e-11
-1.811000000000000000e+03,-1.397810788622120543e-09,5.078540743641003083e-09,-2.494349281004251726e-09,1.437048210368086000e-11
-1.812000000000000000e+03,-1.404715267076801521e-09,5.095110620806871331e-09,-2.506627771148032650e-09,6.121431005595685670e-12
-1.813000000000000000e+03,-1.411727553414516668e-09,5.111484288681524660e-09,-2.518965160750804531e-09,-2.097954425091490792e-12
-1.814000000000000000e+03,-1.418746362910914134e-09,5.127523007059912719e-09,-2.531419781410105734e-09,-1.116357431640611641e-11
-1.815000000000000000e+03,-1.425873161963116908e-09,5.144018407527429283e-09,-2.543983606443186532e-09,-1.977812254184642456e-11
-1.816000000000000000e+03,-1.433056836806802419e-09,5.160370821424869859e-09,-2.556614924214131106e-09,-2.858468983782320442e-11
-1.817000000000000000e+03,-1.440248306006880495e-09,5.176988722503266095e-09,-2.569405866284871026e-09,-3.782696985556942709e-11
-1.818000000000000000e+03,-1.447597309243223682e-09,5.193274017612216516e-09,-2.582315123057077572e-09,-4.722072823953889708e-11
-1.819000000000000000e+03,-1.454954225750141279e-09,5.209782320320438778e-09,-2.595283550205380727e-09,-5.662820095536643067e-11
-1.820000000000000000e+03,-1.462368470933148234e-09,5.226615636078744832e-09,-2.608421182345746759e-09,-6.622734171919031937e-11
-1.821000000000000000e+03,-1.469840967399500845e-09,5.243247455782876404e-09,-2.621618084307165865e-09,-7.603268247453210630e-11
-1.822000000000000000e+03,-1.477421377825775816e-09,5.259781928912084534e-09,-2.634984806102332457e-09,-8.622127120034211441e-11
-1.823000000000000000e+03,-1.485060214948112888e-09,5.276770820725294399e-09,-2.648461375796972594e-09,-9.619292103053857017e-11
-1.824000000000000000e+03,-1.492756892759598108e-09,5.293430933929056828e-09,-2.662057928884154746e-09,-1.067803446214555953e-10
-1.825000000000000000e+03,-1.500512116710046438e-09,5.310544828096672667e-09,-2.675764482122343592e-09,-1.171516185578021319e-10
-1.826000000000000000e+03,-1.508375883808099002e-09,5.327331296388718919e-09,-2.689591583481859233e-09,-1.279057612304512809e-10
-1.827000000000000000e+03,-1.516298370217567323e-09,5.344145426911760172e-09,-2.703528833118302608e-09,-1.388697573083849423e-10
-1.828000000000000000e+03,-1.524279215336837614e-09,5.360866866536138411e-09,-2.717637828461630369e-09,-1.504501021981909000e-10
-1.829000000000000000e+03,-1.532318896995330324e-09,5.378040525741925932e-09,-2.731857170532366951e-09,-1.618161182555126385e-10
-1.830000000000000000e+03,-1.540467756830302318e-09,5.394889387370973660e-09,-2.746198264968121610e-09,-1.735650035688637578e-10
-1.831000000000000000e+03,-1.548675624393276383e-09,5.412423958053750798e-09,-2.760700560145720068e-09,-1.851001402979361257e-10
-1.832000000000000000e+03,-1.556993018514769529e-09,5.429208898421495964e-09,-2.775325244711439268e-09,-1.974443120593454268e-10
-1.833000000000000000e+03,-1.565369590308630575e-09,5.446678845838268325e-09,-2.790111380445174895e-09,-2.095758089322465852e-10
-1.834000000000000000e+03,-1.573805338183144200e-09,5.463827070827387529e-09,-2.805020548355092278e-09,-2.223239363844468059e-10
-1.835000000000000000e+03,-1.582351106672550804e-09,5.480998047627650753e-09,-2.820040583183154999e-09,-2.350532205283011832e-10
-1.836000000000000000e+03,-1.591007102258910493e-09,5.498510767084463985e-09,-2.835235103985228301e-09,-2.477375303429346819e-10
-1.837000000000000000e+03,-1.599722613053764683e-09,5.515852573079777267e-09,-2.850591561749522665e-09,-2.610657704834648220e-10
-1.838000000000000000e+03,-1.608497890212975317e-09,5.533110586771732937e-09,-2.866123275569667949e-09,-2.750111717650509729e-10
-1.839000000000000000e+03,-1.617383636595295993e-09,5.550816791482257239e-09,-2.881766272551973161e-09,-2.885121410624871710e-10
-1.840000000000000000e+03,-1.626329446337044833e-09,5.568013073521160127e-09,-2.897585247303186326e-09,-3.030583633546012166e-10
-1.841000000000000000e+03,-1.635385948616831000e-09,5.585656434015767014e-09,-2.913515678167904828e-09,-3.171610336300816077e-10
-1.842000000000000000e+03,-1.644553742231534961e-09,5.603026933227633531e-09,-2.929673848505146766e-09,-3.320743604408795180e-10
-1.843000000000000000e+03,-1.653781548035204435e-09,5.620843618636386759e-09,-2.945943698080091675e-09,-3.467801162365985281e-10
-1.844000000000000000e+03,-1.663121005017409848e-09,5.638389411795047756e-09,-2.962442137676932296e-09,-3.622968257732484378e-10
-1.845000000000000000e+03,-1.672571651139185130e-09,5.655950982606057250e-09,-2.979052474931804675e-09,-3.778010298255174330e-10
-1.846000000000000000e+03,-1.682134364949949542e-09,5.674102608402095014e-09,-2.995892260033237170e-09,-3.932572785156990707e-10
-1.847000000000000000e+03,-1.691757470756234012e-09,5.691409251395983155e-09,-3.012844155551615846e-09,-4.097973624455663026e-10
-1.848000000000000000e+03,-1.701493008284412988e-09,5.709308432518210176e-09,-3.030026365102628680e-09,-4.262893269761782983e-10
-1.849000000000000000e+03,-1.711340225361658745e-09,5.727026833988107771e-09,-3.047372129059055346e-09,-4.432016460638387611e-10
-1.850000000000000000e+03,-1.721249138298278054e-09,5.745104300968002806e-09,-3.064897870084934758e-09,-4.603011606170543000e-10
-1.851000000000000000e+03,-1.731321132578275070e-09,5.762805433402289386e-09,-3.082638722826866688e-09,-4.780173028454223498e-10
-1.852000000000000000e+03,-1.741455188350360507e-09,5.780868229117277816e-09,-3.100560429756333628e-09,-4.959204049738956529e-10
-1.853000000000000000e+03,-1.751752653197258717e-09,5.798746717613912662e-09,-3.118646265260558158e-09,-5.140111372047307635e-10
-1.854000000000000000e+03,-1.762112547988387962e-09,5.816364133089354520e-09,-3.136965170583140789e-09,-5.331510127178532929e-10
-1.855000000000000000e+03,-1.772636177877038408e-09,5.834463931572702435e-09,-3.155499919645212068e-09,-5.520491598255763040e-10
-1.856000000000000000e+03,-1.783222608543883171e-09,5.852499439916383405e-09,-3.174217309591791781e-09,-5.715650575367340346e-10
-1.857000000000000000e+03,-1.793973099085439455e-09,5.870822082924156216e-09,-3.193202371385463943e-09,-5.912723342638213794e-10
-1.858000000000000000e+03,-1.804838149415925261e-09,5.888412886722564610e-09,-3.212319535402434146e-09,-6.117924668495402124e-10
-1.859000000000000000e+03,-1.815816223289606675e-09,5.906721445017739896e-09,-3.231704783929622117e-09,-6.323109667558023321e-10
-1.860000000000000000e+03,-1.826909291206092605e-09,5.924776180412362180e-09,-3.251326106453199275e-09,-6.536424760430450691e-10
-1.861000000000000000e+03,-1.838115645886638970e-09,5.943115029343291008e-09,-3.271216027842074479e-09,-6.754071534305274513e-10
-1.862000000000000000e+03,-1.849488931660029873e-09,5.961397392274741583e-09,-3.291291503959273716e-09,-6.973143268040146149e-10
-1.863000000000000000e+03,-1.860975820461937266e-09,5.979290553452208619e-09,-3.311584388282695467e-09,-7.200901078963260700e-10
-1.864000000000000000e+03,-1.872578636662394368e-09,5.997606729718464161e-09,-3.332167113349814127e-09,-7.432460621113944554e-10
-1.865000000000000000e+03,-1.884346901704908429e-09,6.015531382772074711e-09,-3.352967687298818653e-09,-7.670355399114076694e-10
-1.866000000000000000e+03,-1.896231592032489498e-09,6.033882426223619949e-09,-3.374059282067044866e-09,-7.912049660950330772e-10
-1.867000000000000000e+03,-1.908282103089762157e-09,6.052078623670877121e-09,-3.395420921967290485e-09,-8.160105803630162319e-10
-1.868000000000000000e+03,-1.920501212165492203e-09,6.070465747907129153e-09,-3.417023037445558891e-09,-8.409572217151680808e-10
-1.869000000000000000e+03,-1.932783165782637717e-09,6.088695880230931585e-09,-3.438895686100201391e-09,-8.670200284297881684e-10
-1.870000000000000000e+03,-1.945285955405197611e-09,6.106924686734028566e-09,-3.461061804068387954e-09,-8.934196051301707251e-10
-1.871000000000000000e+03,-1.957955354860015622e-09,6.125233661179835129e-09,-3.483550867704206510e-09,-9.204610234605238841e-10
-1.872000000000000000e+03,-1.970742753064917384e-09,6.143304894714490817e-09,-3.506282819952314861e-09,-9.483169645756657685e-10
-1.873000000000000000e+03,-1.983697127238902466e-09,6.161454091079167825e-09,-3.529338305596670535e-09,-9.768179758161852309e-10
-1.874000000000000000e+03,-1.996821855700179260e-09,6.179608443520380602e-09,-3.552689872183611752e-09,-1.005894477435589998e-09
-1.875000000000000000e+03,-2.010113978216621499e-09,6.197838736569138898e-09,-3.576365605929002298e-09,-1.035619067465099616e-09
-1.876000000000000000e+03,-2.023577084931220239e-09,6.216318022732323317e-09,-3.600390802346158075e-09,-1.065918935834997974e-09
-1.877000000000000000e+03,-2.037208001719648960e-09,6.234434840632318780e-09,-3.624740845138567618e-09,-1.097306517020076069e-09
-1.878000000000000000e+03,-2.051010536522483342e-09,6.253000661844447185e-09,-3.649389754906856354e-09,-1.128832771851906072e-09
-1.879000000000000000e+03,-2.064981295354569849e-09,6.271005119692143244e-09,-3.674416241132847853e-09,-1.161887247435947681e-09
-1.880000000000000000e+03,-2.079176325941206547e-09,6.289266200733408694e-09,-3.699795178675472513e-09,-1.195277074600629063e-09
-1.881000000000000000e+03,-2.093540046578826280e-09,6.307400149577407488e-09,-3.725552471360750017e-09,-1.229762335330460372e-09
-1.882000000000000000e+03,-2.108076723199443922e-09,6.325598446470590804e-09,-3.751715991696324997e-09,-1.265260572198640989e-09
-1.883000000000000000e+03,-2.122834600669311143e-09,6.343863668538366546e-09,-3.778206461174713385e-09,-1.301180263796071592e-09
-1.884000000000000000e+03,-2.137818266585405786e-09,6.362000830820221468e-09,-3.805157073960480488e-09,-1.338310341907335357e-09
-1.885000000000000000e+03,-2.152971549617139803e-09,6.380005515746385490e-09,-3.832487676547962173e-09,-1.376544466642547660e-09
-1.886000000000000000e+03,-2.168351388468331634e-09,6.398082998555451918e-09,-3.860227951032592911e-09,-1.415551482908866768e-09
-1.887000000000000000e+03,-2.183953518541881230e-09,6.416508767517723527e-09,-3.888453714476668731e-09,-1.455425745501979287e-09
-1.888000000000000000e+03,-2.199730786926466314e-09,6.434573332206478835e-09,-3.917091009932342743e-09,-1.496752955117920446e-09
-1.889000000000000000e+03,-2.215783134943964283e-09,6.452544736464263366e-09,-3.946214820428543798e-09,-1.539149802425701917e-09
-1.890000000000000000e+03,-2.232063697184280694e-09,6.470400917681771196e-09,-3.975804481870011722e-09,-1.582759356201134640e-09
-1.891000000000000000e+03,-2.248567688500227322e-09,6.488600634762716361e-09,-4.005881728840662819e-09,-1.627245334256589976e-09
-1.892000000000000000e+03,-2.265300733627150765e-09,6.506735196051704738e-09,-4.036531839000715202e-09,-1.673384291278436948e-09
-1.893000000000000000e+03,-2.282310159677531124e-09,6.524771083674255065e-09,-4.067670702769829679e-09,-1.720602727881212011e-09
-1.894000000000000000e+03,-2.299549538964116346e-09,6.542746817332523960e-09,-4.099384712719210737e-09,-1.769475531377370611e-09
-1.895000000000000000e+03,-2.317013528948583806e-09,6.560863627608908569e-09,-4.131641216756602970e-09,-1.819675346810545241e-09
-1.896000000000000000e+03,-2.334813272561945048e-09,6.579168789985688871e-09,-4.164527844042952555e-09,-1.871046304485001122e-09
-1.897000000000000000e+03,-2.352838294620597346e-09,6.596973817020860092e-09,-4.198010923087815209e-09,-1.924631596197927071e-09
-1.898000000000000000e+03,-2.371200156915934148e-09,6.615414019235015231e-09,-4.232126692988014067e-09,-1.978948046805173159e-09
-1.899000000000000000e+03,-2.389787962746498011e-09,6.633152837576459061e-09,-4.266893036538020249e-09,-2.035926960821646901e-09
-1.900000000000000000e+03,-2.408713702972557892e-09,6.651335346091305744e-09,-4.302347456418784397e-09,-2.094079253639666287e-09
-1.901000000000000000e+03,-2.427918666372708890e-09,6.669498072620320059e-09,-4.338506791635217902e-09,-2.154217312857391865e-09
-1.902000000000000000e+03,-2.447462720928449711e-09,6.687959127284741365e-09,-4.375515435541121121e-09,-2.216413393926451632e-09
-1.903000000000000000e+03,-2.467286770663299125e-09,6.706443229255537418e-09,-4.413336481223916718e-09,-2.281045253966798635e-09
-1.904000000000000000e+03,-2.487451077437949480e-09,6.725233284813369030e-09,-4.452010208759580342e-09,-2.347737704337763352e-09
-1.905000000000000000e+03,-2.507948881180957679e-09,6.745020589547214031e-09,-4.491709923132086764e-09,-2.416631048254342108e-09
-1.906000000000000000e+03,-2.528840933083043522e-09,6.765168687343118902e-09,-4.532371773787540456e-09,-2.487786290577289313e-09
-1.907000000000000000e+03,-2.550014625308026956e-09,6.785916217681504340e-09,-4.574168132017334155e-09,-2.562280917829106183e-09
-1.908000000000000000e+03,-2.571636684947596910e-09,6.808256959491660624e-09,-4.617195503468525010e-09,-2.638796845683007927e-09
-1.909000000000000000e+03,-2.593594102245898346e-09,6.831732646559800872e-09,-4.661572518069667044e-09,-2.718862127514223860e-09
-1.910000000000000000e+03,-2.615895613058609627e-09,6.857641393637078513e-09,-4.707556652422165979e-09,-2.802327413978472003e-09
-1.911000000000000000e+03,-2.638692069698083246e-09,6.885958455861896053e-09,-4.755265826499396560e-09,-2.889065357719104305e-09
-1.912000000000000000e+03,-2.661834045604118773e-09,6.918289109505465591e-09,-4.805119210080021912e-09,-2.980096644699791260e-09
-1.913000000000000000e+03,-2.685419214608990830e-09,6.956515235169025522e-09,-4.857552867278007312e-09,-3.075102190348108099e-09
-1.914000000000000000e+03,-2.709510263753851089e-09,7.003045496382972797e-09,-4.913255208473256212e-09,-3.174563124374903756e-09
-1.915000000000000000e+03,-2.733992740118446671e-09,7.061768631891637988e-09,-4.973194703126446705e-09,-3.279591994680282016e-09
-1.916000000000000000e+03,-2.758982782847665105e-09,7.140633384248507307e-09,-5.038969521402022701e-09,-3.389084558441558733e-09
-1.917000000000000000e+03,-2.784418469416851105e-09,7.249531035958723057e-09,-5.113042090031981656e-09,-3.504807796428515914e-09
-1.918000000000000000e+03,-2.810416584400537130e-09,7.406197042867337606e-09,-5.199417888318982188e-09,-3.626985505786461652e-09
-1.919000000000000000e+03,-2.836914782408204079e-09,7.639174691730643205e-09,-5.304407421358852163e-09,-3.756506289417693080e-09
-1.920000000000000000e+03,-2.863977348934094082e-09,7.990399065238130725e-09,-5.437158584486999617e-09,-3.893386119834720233e-09
-1.921000000000000000e+03,-2.891594606436244120e-09,8.486058107686444497e-09,-5.603956810009827121e-09,-4.040509910929347707e-09
-1.922000000000000000e+03,-2.919831467938826770e-09,9.047107003955292387e-09,-5.788043777365044786e-09,-4.199227330936162570e-09
-1.923000000000000000e+03,-2.948677851355597167e-09,9.332611685856186170e-09,-5.916216066335999067e-09,-4.372441882880891349e-09
-1.924000000000000000e+03,-2.978199321267735543e-09,9.063489858816396664e-09,-5.928594910159698230e-09,-4.562393504912063463e-09
-1.925000000000000000e+03,-3.008385367693508649e-09,8.479084225229640381e-09,-5.878401881818119812e-09,-4.775582511891927475e-09
-1.926000000000000000e+03,-3.039302232924055597e-09,7.894502693920246503e-09,-5.835677729367590100e-09,-5.020065948733431765e-09
-1.927000000000000000e+03,-3.070992321082550661e-09,7.394952891691197479e-09,-5.821246238717997989e-09,-5.306611347161151041e-09
-1.928000000000000000e+03,-3.103469267434920873e-09,6.957067256408761912e-09,-5.833608676846028146e-09,-5.651601662231105625e-09
-1.929000000000000000e+03,-3.136828482619493710e-09,6.525915529737016828e-09,-5.865779785327465664e-09,-6.077266326957148736e-09
-1.930000000000000000e+03,-3.171137814906708252e-09,6.054660625813822524e-09,-5.914102766051990406e-09,-6.613240802664537404e-09
-1.931000000000000000e+03,-3.206385488295230076e-09,5.502101990304859718e-09,-5.974784568845752389e-09,-7.283262493649364589e-09
-1.932000000000000000e+03,-3.242747148234662276e-09,4.880470478284157200e-09,-6.045227612228179851e-09,-8.062292883778877733e-09
-1.933000000000000000e+03,-3.280317726522882313e-09,4.313627516041255696e-09,-6.123770235670074769e-09,-8.818358033900346270e-09
-1.934000000000000000e+03,-3.319166995976900075e-09,3.949267288981502930e-09,-6.211031674667369088e-09,-9.406301355398451260e-09
-1.935000000000000000e+03,-3.359496802956372092e-09,3.768250127962770008e-09,-6.305881541655091603e-09,-9.839109829233954053e-09
-1.936000000000000000e+03,-3.401592626077954111e-09,3.721590537274182312e-09,-6.409479989957462893e-09,-1.016980848249151423e-08
-1.937000000000000000e+03,-3.445602955701137523e-09,3.679205753639428892e-09,-6.522307113672580734e-09,-1.053001153202009469e-08
-1.938000000000000000e+03,-3.492083454506395258e-09,3.553858031783826242e-09,-6.647146362718017951e-09,-1.101724536681595314e-08
-1.939000000000000000e+03,-3.541505439061627763e-09,3.314015635643467720e-09,-6.785557862270484084e-09,-1.166807019409616203e-08
-1.940000000000000000e+03,-3.594911335668046571e-09,3.001925654751261800e-09,-6.941418080219122968e-09,-1.245332744719247627e-08
-1.941000000000000000e+03,-3.653527392110157236e-09,2.718515732502147776e-09,-7.119530592380898424e-09,-1.328861074335297338e-08
-1.942000000000000000e+03,-3.719477744648099011e-09,2.683323135212896645e-09,-7.327574500348111047e-09,-1.398003744711466297e-08
-1.943000000000000000e+03,-3.795178600063928744e-09,3.210373703857757678e-09,-7.577935546714296561e-09,-1.425962426605817483e-08
-1.944000000000000000e+03,-3.881579621541815148e-09,4.528022563060301576e-09,-7.887528490288523545e-09,-1.397274806312618871e-08
-1.945000000000000000e+03,-3.974636972802020334e-09,6.326651765118054979e-09,-8.286637656176499227e-09,-1.358756536467496681e-08
-1.946000000000000000e+03,-4.070067742649507945e-09,8.323840233225693848e-09,-8.822039611989048829e-09,-1.362230647439476600e-08
-1.947000000000000000e+03,-4.169311794140065705e-09,1.067870168065585702e-08,-9.568011806058774232e-09,-1.425424526216086299e-08
-1.948000000000000000e+03,-4.270614963283632583e-09,1.373920393810281458e-08,-1.062358274214668593e-08,-1.560086093123999672e-08
-1.949000000000000000e+03,-4.364291233605470114e-09,1.756766587234673993e-08,-1.204816604074241023e-08,-1.791895914082987496e-08
-1.950000000000000000e+03,-4.440463216174302551e-09,2.077085112797112402e-08,-1.361686406698625077e-08,-2.160874303992161168e-08
-1.951000000000000000e+03,-4.507838324714636648e-09,1.908992738677906728e-08,-1.447036237207015025e-08,-2.692023856814877074e-08
-1.952000000000000000e+03,-4.574486384987320887e-09,1.012680540200188408e-08,-1.391852752147721391e-08,-3.302700595503990521e-08
-1.953000000000000000e+03,-4.640814466205888051e-09,5.333362341037935642e-10,-1.267866358844953700e-08,-3.658805692662521319e-08
-1.954000000000000000e+03,-4.707335543024713281e-09,-2.916730515109077450e-09,-1.163055460224497350e-08,-3.489040067569428081e-08
-1.955000000000000000e+03,-4.793042274512327528e-09,-1.920873627678890302e-09,-1.098412234023730446e-08,-3.051328855287688966e-08
-1.956000000000000000e+03,-4.920055989586150983e-09,-1.690628277319255878e-10,-1.066236121316987749e-08,-2.668889003668783547e-08
-1.957000000000000000e+03,-5.102246356295459790e-09,9.959799036459158821e-10,-1.056660071637291330e-08,-2.424018010446305317e-08
-1.958000000000000000e+03,-5.350313385366766908e-09,1.456198838012059580e-09,-1.063037937714269853e-08,-2.292885773799360893e-08
-1.959000000000000000e+03,-5.669327208063359342e-09,1.347818365283259792e-09,-1.081786113363485948e-08,-2.242978048558227916e-08
-1.960000000000000000e+03,-6.057042929694721577e-09,7.430645868982077313e-10,-1.111141498385561255e-08,-2.259966421400457412e-08
-1.961000000000000000e+03,-6.497335857581804880e-09,-3.541850280160069201e-10,-1.150834686960424183e-08,-2.349665847843875704e-08
-1.962000000000000000e+03,-6.987609463996096821e-09,-2.033827912951878587e-09,-1.201882355920452750e-08,-2.526960575147651725e-08
-1.963000000000000000e+03,-7.575240992682569120e-09,-4.519262034487464036e-09,-1.266090472317790127e-08,-2.800650594163358535e-08
-1.964000000000000000e+03,-8.260962107305569654e-09,-8.176177818082585409e-09,-1.346888675364914450e-08,-3.222806227226682523e-08
-1.965000000000000000e+03,-8.899415392668798367e-09,-1.363931511856066746e-08,-1.449428167450892669e-08,-3.947822149404139519e-08
-1.966000000000000000e+03,-9.274747526815695862e-09,-2.195343748953640706e-08,-1.581702631907746704e-08,-5.216780199441009615e-08
-1.967000000000000000e+03,-9.261622825963132487e-09,-3.472788583432166750e-08,-1.756062097731499440e-08,-7.305534987740172220e-08
-1.968000000000000000e+03,-8.808778040740959659e-09,-5.402253450620837986e-08,-1.992220222628329959e-08,-1.053479304273395657e-07
-1.969000000000000000e+03,-8.176416829281552198e-09,-8.044247148891660336e-08,-2.322053255246186056e-08,-1.499210752823398681e-07
-1.970000000000000000e+03,-7.625367628668655796e-09,-1.057022165059423269e-07,-2.797648555268283155e-08,-1.996902770216656559e-07
-1.971000000000000000e+03,-7.257336515848423820e-09,-1.020759509061903876e-07,-3.501370852447027209e-08,-2.302638756081032960e-07
-1.972000000000000000e+03,-7.089607835217760526e-09,-4.504943296124118613e-08,-4.545905079115249596e-08,-2.222519601129125469e-07
-1.973000000000000000e+03,-7.101664595110094800e-09,4.857417106367263162e-08,-6.005895496365628210e-08,-1.959997648985581722e-07
-1.974000000000000000e+03,-7.283993645687315738e-09,1.418159609531945160e-07,-7.633609476934901419e-08,-1.770890291009548702e-07
-1.975000000000000000e+03,-7.657085523403337822e-09,1.807439112521224687e-07,-8.453652002152950335e-08,-1.743102419891664038e-07
-1.976000000000000000e+03,-8.274451127745950583e-09,1.268636843061328037e-07,-7.679475887680869915e-08,-1.895853115338270598e-07
-1.977000000000000000e+03,-9.182465227221670394e-09,1.589732911569132574e-08,-6.105963549135049008e-08,-2.236882620235536388e-07
-1.978000000000000000e+03,-1.024446856053438523e-08,-9.722847382235596325e-08,-4.711737948274322358e-08,-2.675195308584925537e-07
-1.979000000000000000e+03,-1.088374980641654229e-08,-1.656464908398017249e-07,-3.740237386513684329e-08,-2.881180942244818725e-07
-1.980000000000000000e+03,-1.061655050785118216e-08,-1.642405806461866718e-07,-3.111923786120516011e-08,-2.589286379262309336e-07
-1.981000000000000000e+03,-9.855722639063078301e-09,-1.262755854969871473e-07,-2.714148211941582931e-08,-2.061068269140765692e-07
-1.982000000000000000e+03,-9.135415234386207839e-09,-9.058196717881033217e-08,-2.466753905402919584e-08,-1.623143505765655921e-07
-1.983000000000000000e+03,-8.640389706773261003e-09,-6.817031403639213048e-08,-2.320674230117768304e-08,-1.354424528077350667e-07
-1.984000000000000000e+03,-8.376557869804928990e-09,-5.793522307448307186e-08,-2.247850625403827714e-08,-1.230625926408964653e-07
-1.985000000000000000e+03,-8.293563287894828261e-09,-5.782337444660790977e-08,-2.233789841286617102e-08,-1.226846673032187628e-07
-1.986000000000000000e+03,-8.335565573864457444e-09,-6.738824606327068769e-08,-2.273992233032926589e-08,-1.339122355350806592e-07
-1.987000000000000000e+03,-8.434349585634326398e-09,-8.672379216068505126e-08,-2.372562426827048446e-08,-1.573438561591483220e-07
-1.988000000000000000e+03,-8.536027298573277130e-09,-1.090516728090293622e-07,-2.544213114930416415e-08,-1.871295414421142579e-07
-1.989000000000000000e+03,-8.638331991377984737e-09,-1.108281890445284184e-07,-2.816963837396493756e-08,-2.010300940746000092e-07
-1.990000000000000000e+03,-8.738021024486458874e-09,-7.203802906746933630e-08,-3.233949903917744385e-08,-1.810373062662791867e-07
-1.991000000000000000e+03,-8.809608377943444083e-09,-8.352521413532205037e-09,-3.831110742443238336e-08,-1.446000085559503003e-07
-1.992000000000000000e+03,-8.832674847801105940e-09,5.504928292230383134e-08,-4.531574571675992355e-08,-1.134413663596679712e-07
-1.993000000000000000e+03,-8.852421869568497695e-09,9.706689632509935634e-08,-4.989385722386137880e-08,-9.247575799659344126e-08
-1.994000000000000000e+03,-8.917056986589209924e-09,1.058550148394398942e-07,-4.903104698678004168e-08,-7.940439615420402360e-08
-1.995000000000000000e+03,-9.033218673888898275e-09,9.413586757555678063e-08,-4.488782183883913154e-08,-7.145231409667087535e-08
-1.996000000000000000e+03,-9.191651059323931186e-09,7.747404255118739686e-08,-4.041813850785532184e-08,-6.674000028244296494e-08
-1.997000000000000000e+03,-9.383476325174007794e-09,6.319023564719806651e-08,-3.700221061970004780e-08,-6.436203346812822143e-08
-1.998000000000000000e+03,-9.604396198843451031e-09,5.341367602910619645e-08,-3.500613391641959861e-08,-6.389978413157086557e-08
-1.999000000000000000e+03,-9.851600307136601103e-09,4.757428778626067110e-08,-3.425931700612653742e-08,-6.514846104358875237e-08
-2.000000000000000000e+03,-1.012411149640612788e-08,4.518770037510796269e-08,-3.451372792247565348e-08,-6.745145552618850930e-08
-2.001000000000000000e+03,-1.042243682360716812e-08,4.736906117744066563e-08,-3.562388788452880845e-08,-6.901941026878730665e-08
-2.002000000000000000e+03,-1.074838394682460963e-08,5.535016619016751518e-08,-3.755201598324827853e-08,-6.843769643667639058e-08
-2.003000000000000000e+03,-1.110356911291321050e-08,6.791463867557007291e-08,-4.033824102264308428e-08,-6.710055424249214891e-08
-2.004000000000000000e+03,-1.149148640128018243e-08,8.394603246707972191e-08,-4.411722544643811113e-08,-6.673020788471607901e-08
-2.005000000000000000e+03,-1.191431041976192025e-08,1.041157826772109087e-07,-4.913548068886821587e-08,-6.778364893046409144e-08
-2.006000000000000000e+03,-1.237556083216254252e-08,1.303770401654442119e-07,-5.579563775155077999e-08,-7.015095207233398183e-08
-2.007000000000000000e+03,-1.288577535090676604e-08,1.655202610581785999e-07,-6.468666483687049832e-08,-7.371304071685871953e-08
-2.008000000000000000e+03,-1.345966878947909614e-08,2.129296267026550777e-07,-7.654091467958521678e-08,-7.840001809933762824e-08
-2.009000000000000000e+03,-1.411842324678290056e-08,2.762589328978579984e-07,-9.217944987584114191e-08,-8.425219588264187976e-08
-2.010000000000000000e+03,-1.489248202016478901e-08,3.626047030271251098e-07,-1.131864939749130518e-07,-9.134891163080919346e-08
-2.011000000000000000e+03,-1.582491063520603346e-08,4.854281461106261799e-07,-1.425499727650921118e-07,-9.982927575650655752e-08
-2.012000000000000000e+03,-1.698434625777039615e-08,6.541288443209210211e-07,-1.824138834485221110e-07,-1.098783915776765777e-07
-2.013000000000000000e+03,-1.848006320759849203e-08,8.590536641823094518e-07,-2.308427482347750174e-07,-1.217060644055545166e-07
-2.014000000000000000e+03,-2.047343273780704566e-08,1.086515795701486969e-06,-2.850879167186230481e-07,-1.355596807704319807e-07
-2.015000000000000000e+03,-2.314532313760528357e-08,1.331991316114148874e-06,-3.444663339566764381e-07,-1.519732858598810691e-07
-2.016000000000000000e+03,-2.646559524209135369e-08,1.560041907764902271e-06,-4.017449540442626269e-07,-1.731198387836677350e-07
-2.017000000000000000e+03,-2.979635032955599883e-08,1.675096042000631357e-06,-4.369291219923158497e-07,-2.051750921870622224e-07
-2.018000000000000000e+03,-3.234489024484662016e-08,1.574909586405706751e-06,-4.289610244997090525e-07,-2.567923066815246804e-07
-2.019000000000000000e+03,-3.381791866259368604e-08,1.278112366294968697e-06,-3.836101381401810440e-07,-3.373415077840987591e-07
-2.020000000000000000e+03,-3.403860827559427804e-08,8.303883848088617523e-07,-3.135879489457375496e-07,-4.606611018157767637e-07
-2.021000000000000000e+03,-3.333001457059696121e-08,3.214991337580891328e-07,-2.428165707802431271e-07,-6.459776994938836654e-07
-2.022000000000000000e+03,-3.205421517729614821e-08,-1.947821430139388198e-07,-1.892668855137624374e-07,-9.208412238267202188e-07
-2.023000000000000000e+03,-3.086280416783258406e-08,-7.382404355561522128e-07,-1.535486431866737757e-07,-1.304843415558476168e-06
-2.024000000000000000e+03,-3.023672187194387697e-08,-1.278213345730789024e-06,-1.305729370602988962e-07,-1.741598517014866062e-06
-2.025000000000000000e+03,-3.021810749608452984e-08,-1.596973229394696918e-06,-1.165630188411685498e-07,-1.995742023474083793e-06
-2.026000000000000000e+03,-3.070418632441195244e-08,-1.501605040474100028e-06,-1.093811228715118133e-07,-1.864960640937446605e-06
-2.027000000000000000e+03,-3.165378150800779812e-08,-1.165619366098478228e-06,-1.078223965734191548e-07,-1.517390724747981222e-06
-2.028000000000000000e+03,-3.306878434316088039e-08,-8.156717455368504097e-07,-1.114461727657827207e-07,-1.177643935646233394e-06
-2.029000000000000000e+03,-3.494967354093083440e-08,-5.336675760469525005e-07,-1.205475730708716319e-07,-9.289864273787322718e-07
-2.030000000000000000e+03,-3.731767890586666494e-08,-3.244951436664374075e-07,-1.359428533241837664e-07,-7.799781739457963174e-07
-2.031000000000000000e+03,-4.021853420489772790e-08,-1.678069028411175639e-07,-1.587338045108597327e-07,-7.151488444064061800e-07
-2.032000000000000000e+03,-4.369754365145181072e-08,-4.290302266768245322e-08,-1.909444583141697474e-07,-7.229370128271432380e-07
-2.033000000000000000e+03,-4.774519396248156632e-08,6.281507894540534407e-08,-2.358247221141244347e-07,-8.057971584602995575e-07
-2.034000000000000000e+03,-5.243337330956853940e-08,1.352187949088642962e-07,-2.938626941276389621e-07,-9.797800813220577873e-07
-2.035000000000000000e+03,-5.812015214413861307e-08,1.120031889110302246e-07,-3.561200958037023043e-07,-1.264257164104144979e-06
-2.036000000000000000e+03,-6.537916642193212427e-08,-6.843992528965574289e-08,-4.044720215978143545e-07,-1.634480666231608602e-06
-2.037000000000000000e+03,-7.502842493462097620e-08,-3.767195657599867707e-07,-4.146369667181960247e-07,-1.945141914644655621e-06
-2.038000000000000000e+03,-8.818805779117529694e-08,-7.305269354963526414e-07,-3.708141602600047296e-07,-2.035785905610158134e-06
-2.039000000000000000e+03,-1.058461315867683685e-07,-9.871488487577988718e-07,-3.032927242996968197e-07,-1.899021227160571160e-06
-2.040000000000000000e+03,-1.268415752217128976e-07,-1.039186926136626781e-06,-2.447573168612589523e-07,-1.583760049949967151e-06
-2.041000000000000000e+03,-1.447613005036413283e-07,-9.640977010278856305e-07,-2.036324969385781300e-07,-1.235983972525076772e-06
-2.042000000000000000e+03,-1.538471062721267268e-07,-8.718871650389385218e-07,-1.777112963471066479e-07,-9.820997317048348195e-07
-2.043000000000000000e+03,-1.579604844825922853e-07,-8.264948413125153164e-07,-1.636417321485185033e-07,-8.527326849250178762e-07
-2.044000000000000000e+03,-1.629871726975151058e-07,-8.444889568130932750e-07,-1.590668627684791712e-07,-8.263836945750991325e-07
-2.045000000000000000e+03,-1.737303189904493862e-07,-8.880510036838477618e-07,-1.625092533321241406e-07,-8.362284845434569982e-07
-2.046000000000000000e+03,-1.936290774381499548e-07,-9.122468010510526565e-07,-1.735886693413027912e-07,-8.196936992509948951e-07
-2.047000000000000000e+03,-2.248458668743282572e-07,-9.157711046637109648e-07,-1.932637536977961777e-07,-7.699146669223868795e-07
-2.048000000000000000e+03,-2.705840214950579943e-07,-8.936199607617391560e-07,-2.240064756297372889e-07,-6.785097532631158127e-07
-2.049000000000000000e+03,-3.366313526850503352e-07,-8.158764813725145195e-07,-2.702210919735750447e-07,-5.091723668408079490e-07
-2.050000000000000000e+03,-4.285771863175247527e-07,-6.491378707595357182e-07,-3.386541047757041336e-07,-2.338439266494666770e-07
-2.051000000000000000e+03,-5.474774717567388784e-07,-4.193315132349390067e-07,-4.376714219479489760e-07,8.778842449796623055e-08
-2.052000000000000000e+03,-6.971734411681456521e-07,-1.655481790415013143e-07,-5.727985737180417464e-07,4.088552818485570814e-07
-2.053000000000000000e+03,-8.892949991710879165e-07,7.291631922026097359e-08,-7.365128245684769468e-07,7.785139343433916875e-07
-2.054000000000000000e+03,-1.113859783231082820e-06,2.953780133670429678e-07,-9.100801421624163900e-07,1.236498462285182302e-06
-2.055000000000000000e+03,-1.305681043612587993e-06,5.797017152836893437e-07,-1.063575990707045729e-06,1.697821341370557948e-06
-2.056000000000000000e+03,-1.396090188161314722e-06,8.934498843974060471e-07,-1.156494958071044240e-06,1.999978335025204512e-06
-2.057000000000000000e+03,-1.396107318384118362e-06,8.506418672622317608e-07,-1.163247494062788282e-06,1.926064030394040823e-06
-2.058000000000000000e+03,-1.327015368301713149e-06,1.095699969007172931e-07,-1.069015060142100418e-06,1.301099065078704628e-06
-2.059000000000000000e+03,-1.219034879044967809e-06,-1.049227296075445613e-06,-9.224139541924050781e-07,3.206643010036356228e-07
-2.060000000000000000e+03,-1.094955711721131093e-06,-2.171821523649265942e-06,-7.702796704418642728e-07,-6.723623032910106194e-07
-2.061000000000000000e+03,-9.955023480934653025e-07,-2.896283223891603751e-06,-6.370255883360304280e-07,-1.240721327225216960e-06
-2.062000000000000000e+03,-9.429411369837395550e-07,-3.031227660930861946e-06,-5.306819809699602123e-07,-1.127281221808596024e-06
-2.063000000000000000e+03,-9.146224231994283173e-07,-2.883948924795574479e-06,-4.541014898592459692e-07,-7.571139512504479690e-07
-2.064000000000000000e+03,-8.788539205112714068e-07,-2.740668805087049254e-06,-4.074822292084304883e-07,-5.637215133958808629e-07
-2.065000000000000000e+03,-8.385643691320077877e-07,-2.499526980256540861e-06,-3.879120004941065977e-07,-4.182682379486600758e-07
-2.066000000000000000e+03,-7.987920568837064711e-07,-2.005937237476151958e-06,-3.853866468025470894e-07,-9.669702544894905504e-08
-2.067000000000000000e+03,-7.553785565942146109e-07,-1.498424823306805570e-06,-3.760344464770078688e-07,2.535092626289844002e-07
-2.068000000000000000e+03,-6.973274880343980655e-07,-1.255999308731478967e-06,-3.406437270641733123e-07,3.912819382356554544e-07
-2.069000000000000000e+03,-6.276380484051462220e-07,-1.278399073453848761e-06,-2.939614172007684855e-07,2.626277892185576249e-07
-2.070000000000000000e+03,-5.512389675105410784e-07,-1.468753609324188078e-06,-2.555863174998531027e-07,-1.033338193848319322e-07
-2.071000000000000000e+03,-4.822553961642185192e-07,-1.730610952113731242e-06,-2.325049672337169729e-07,-5.771825008712957828e-07
-2.072000000000000000e+03,-4.294278199835091498e-07,-1.952853038584441804e-06,-2.248071078855478268e-07,-1.007848250973237488e-06
-2.073000000000000000e+03,-3.892326563663907700e-07,-1.992521622290431780e-06,-2.289218257426733965e-07,-1.252154232830784365e-06
-2.074000000000000000e+03,-3.527711494596945088e-07,-1.748165797282123133e-06,-2.406554647028102312e-07,-1.230379216562762442e-06
-2.075000000000000000e+03,-3.150643333697773269e-07,-1.364561176529832253e-06,-2.569806511783820099e-07,-1.096311901125697851e-06
-2.076000000000000000e+03,-2.732739248841720644e-07,-1.007127558231266969e-06,-2.782088082790926627e-07,-1.029918449664927414e-06
-2.077000000000000000e+03,-2.322558275718103895e-07,-7.222523682004904347e-07,-3.136852631096305419e-07,-1.098319901378060466e-06
-2.078000000000000000e+03,-1.971204385086648923e-07,-5.046111557433930905e-07,-3.741097539598224353e-07,-1.322005195391249075e-06
-2.079000000000000000e+03,-1.705664339109240362e-07,-3.544484006677590265e-07,-4.626768278944246943e-07,-1.703508903854980316e-06
-2.080000000000000000e+03,-1.532152625326395793e-07,-2.916472367798899955e-07,-5.667482274922562049e-07,-2.201476538589790555e-06
-2.081000000000000000e+03,-1.434213192364837275e-07,-3.491577580193542838e-07,-6.431782069599001636e-07,-2.657197089415116950e-06
-2.082000000000000000e+03,-1.396006637966582855e-07,-5.215937066164821703e-07,-6.495953533291521042e-07,-2.876914525917346423e-06
-2.083000000000000000e+03,-1.417778614234438797e-07,-6.854081184826488463e-07,-5.957635567745040747e-07,-2.782061244234467645e-06
-2.084000000000000000e+03,-1.508361105749619314e-07,-7.308971234599496962e-07,-5.035405988863013085e-07,-2.359800799186609704e-06
-2.085000000000000000e+03,-1.678628123265604820e-07,-7.184501782488059641e-07,-4.043096285618394148e-07,-1.810438232961432843e-06
-2.086000000000000000e+03,-1.952332676378231689e-07,-7.479847165360838827e-07,-3.205148574564183493e-07,-1.326575715288136076e-06
-2.087000000000000000e+03,-2.375259593155023713e-07,-8.653537240052418227e-07,-2.583893614076440666e-07,-9.617076788946789158e-07
-2.088000000000000000e+03,-2.985081913817004091e-07,-1.090600401292392449e-06,-2.166324900341369179e-07,-7.124718679236360356e-07
-2.089000000000000000e+03,-3.750268949951185525e-07,-1.423483143803073583e-06,-1.905306189053538569e-07,-5.714195261288423324e-07
-2.090000000000000000e+03,-4.533778781862672890e-07,-1.788326512195241862e-06,-1.755468148150056162e-07,-5.052125872116430102e-07
-2.091000000000000000e+03,-5.038012610133626526e-07,-1.948066180687448724e-06,-1.683888428392337549e-07,-3.990228910371963276e-07
-2.092000000000000000e+03,-4.984750346587236920e-07,-1.703957924637922700e-06,-1.670579374640476313e-07,-1.733663225754795533e-07
-2.093000000000000000e+03,-4.489724012336468426e-07,-1.235411283206329409e-06,-1.709946593859154477e-07,4.838005053556280898e-08
-2.094000000000000000e+03,-3.749583606241881052e-07,-7.696337387440354323e-07,-1.806779982171361459e-07,1.276159615971896079e-07
-2.095000000000000000e+03,-3.016047297063405128e-07,-3.667153899685192235e-07,-1.978520530275289124e-07,1.124481081137996806e-07
-2.096000000000000000e+03,-2.454984486715494287e-07,-5.563827311390367792e-09,-2.249789721956611665e-07,8.920176757964137021e-08
-2.097000000000000000e+03,-2.067605532679008784e-07,3.467626627885453067e-07,-2.649578301996231412e-07,7.798877004555055717e-08
-2.098000000000000000e+03,-1.807516474110473209e-07,7.290960659791137099e-07,-3.224570396396577844e-07,7.465462301194005244e-08
-2.099000000000000000e+03,-1.665509659666729620e-07,1.195125797386334357e-06,-4.053268023750030687e-07,9.238157243360673595e-08
-2.100000000000000000e+03,-1.640673896619498336e-07,1.807487511532277163e-06,-5.238981830384037849e-07,1.456722486282298137e-07
-2.101000000000000000e+03,-1.698836804677122358e-07,2.607990157448870747e-06,-6.856728850781364150e-07,2.259083889049617869e-07
-2.102000000000000000e+03,-1.772765473953681967e-07,3.529784747342347749e-06,-8.755228741081000293e-07,3.050568353430484100e-07
-2.103000000000000000e+03,-1.760384235421543206e-07,4.262687044184345584e-06,-1.027108934946336219e-06,3.321675008517576173e-07
-2.104000000000000000e+03,-1.585339786464806999e-07,4.510147357602584292e-06,-1.077232175308712560e-06,2.673012384865780854e-07
-2.105000000000000000e+03,-1.326257927251487169e-07,4.376193341998730628e-06,-1.048830567184552856e-06,1.448626549963617924e-07
-2.106000000000000000e+03,-1.079474084964266922e-07,3.991439950052300780e-06,-9.706540741676927585e-07,7.180873810099086366e-09
-2.107000000000000000e+03,-8.844200100823563097e-08,3.392183467796374615e-06,-8.515585820937986564e-07,-1.321363101843786899e-07
-2.108000000000000000e+03,-7.469471039768052782e-08,2.578148604678496320e-06,-6.932634020933312860e-07,-2.786021568912207559e-07
-2.109000000000000000e+03,-6.544279954226003517e-08,1.729425230394659070e-06,-5.366082013856400961e-07,-4.465693496925599478e-07
-2.110000000000000000e+03,-5.921838041486991827e-08,1.029969994391564150e-06,-4.183269391676343597e-07,-6.285097548679094661e-07
-2.111000000000000000e+03,-5.499444315002061412e-08,5.583232363331339539e-07,-3.402154110325709990e-07,-7.589196635306528179e-07
-2.112000000000000000e+03,-5.207521168571107473e-08,3.332958396796966590e-07,-2.924503242270537582e-07,-7.768343609492649953e-07
-2.113000000000000000e+03,-5.012067593813825091e-08,2.839989167622833177e-07,-2.679167175330374982e-07,-7.218538139789432771e-07
-2.114000000000000000e+03,-4.898912401480481503e-08,3.217561083431454421e-07,-2.596490946002631542e-07,-6.511399329236221006e-07
-2.115000000000000000e+03,-4.889937745137985840e-08,3.490127665512735545e-07,-2.545986360732805182e-07,-6.009730985781056798e-07
-2.116000000000000000e+03,-5.020743206970641717e-08,2.957156759597289188e-07,-2.424108901463899620e-07,-5.919422068402252380e-07
-2.117000000000000000e+03,-5.327705224486849457e-08,1.700226933624069487e-07,-2.287188553692419921e-07,-6.402244326484846473e-07
-2.118000000000000000e+03,-5.779031584102205850e-08,-1.340851564068184493e-08,-2.209424769340743973e-07,-7.668980903824413826e-07
-2.119000000000000000e+03,-6.180429610672297875e-08,-2.642804633874741300e-07,-2.193782367324735178e-07,-9.920080075219541134e-07
-2.120000000000000000e+03,-6.324025651248582799e-08,-5.376015849190545425e-07,-2.230234518173393531e-07,-1.275532183413961590e-06
-2.121000000000000000e+03,-6.232754015035066385e-08,-6.214409709532254244e-07,-2.369211725172535299e-07,-1.427770969424565472e-06
-2.122000000000000000e+03,-6.002797945833344844e-08,-3.286673724018057357e-07,-2.674188376492211724e-07,-1.286465592766507010e-06
-2.123000000000000000e+03,-5.846824408955803382e-08,2.122401623684364145e-07,-3.174188760994823704e-07,-9.836778094504278461e-07
-2.124000000000000000e+03,-5.960498163716995387e-08,8.099931805415597365e-07,-3.851675930392102182e-07,-6.935605080744977267e-07
-2.125000000000000000e+03,-6.434046295065252664e-08,1.356403336974907050e-06,-4.592082907937059612e-07,-4.672243102921849035e-07
-2.126000000000000000e+03,-7.168325136062966852e-08,1.764079232552303199e-06,-5.193993284097719377e-07,-3.036187632370569150e-07
-2.127000000000000000e+03,-7.708315630078988267e-08,1.939488784991093129e-06,-5.414832517094215819e-07,-2.052614166314790775e-07
-2.128000000000000000e+03,-7.673679435098173498e-08,1.814357969127362250e-06,-5.069437474528248179e-07,-1.724772157205795331e-07
-2.129000000000000000e+03,-7.383268724969960822e-08,1.508548093544096811e-06,-4.379011601649555863e-07,-1.728381473487903861e-07
-2.130000000000000000e+03,-7.264193465876421294e-08,1.158263864965605262e-06,-3.604405265765245772e-07,-1.708833383724504363e-07
-2.131000000000000000e+03,-7.518011416821836649e-08,8.555677572705253236e-07,-2.926467007092620956e-07,-1.487634432208844732e-07
-2.132000000000000000e+03,-8.238725689235980846e-08,6.438504857816521125e-07,-2.432208196610729879e-07,-9.893105019617796273e-08
-2.133000000000000000e+03,-9.518639125886300133e-08,5.114543101066446853e-07,-2.118006646923681760e-07,-2.710821158815893094e-08
-2.134000000000000000e+03,-1.142107262998595909e-07,4.351132307163040002e-07,-1.944511230516763103e-07,6.453706414531098829e-08
-2.135000000000000000e+03,-1.382260321833563949e-07,4.020804392935877759e-07,-1.856096160417496343e-07,1.832476870210737069e-07
-2.136000000000000000e+03,-1.611716082534475736e-07,4.095854089016087844e-07,-1.818557217590073025e-07,3.140594668313374959e-07
-2.137000000000000000e+03,-1.688269680307903325e-07,4.617420984142038670e-07,-1.868384531167704242e-07,3.785592208661563564e-07
-2.138000000000000000e+03,-1.505887826895676457e-07,5.694228995412091147e-07,-2.062558967045835890e-07,3.123341194400819013e-07
-2.139000000000000000e+03,-1.206164941939699012e-07,7.412848803919481893e-07,-2.425183273062285062e-07,1.783026938451829776e-07
-2.140000000000000000e+03,-9.526139856493466885e-08,9.391073292372700705e-07,-2.869212343080481025e-07,5.396007061904674097e-08
-2.141000000000000000e+03,-7.822076034897002942e-08,1.015119111483192490e-06,-3.077256878909968573e-07,-4.480905064609327711e-08
-2.142000000000000000e+03,-6.772668206829085954e-08,8.488163968791162285e-07,-2.793645607990176729e-07,-1.285959412456171546e-07
-2.143000000000000000e+03,-6.150796806090716171e-08,5.514753309548137730e-07,-2.263533414189404392e-07,-2.098340469752123053e-07
-2.144000000000000000e+03,-5.815069076757298781e-08,2.593377061972377973e-07,-1.791795955468084523e-07,-2.996130142995342978e-07
-2.145000000000000000e+03,-5.775519243347178256e-08,-8.858035151996387228e-10,-1.461586070357638048e-07,-4.091614330142748371e-07
-2.146000000000000000e+03,-6.095652157743612840e-08,-2.536565736088393075e-07,-1.252035434412419323e-07,-5.503701498082601022e-07
-2.147000000000000000e+03,-6.793550254732982102e-08,-5.314707196367582834e-07,-1.120079591255325357e-07,-7.350116126439596962e-07
-2.148000000000000000e+03,-7.723547322794388332e-08,-8.570946402870913923e-07,-1.033577145133273237e-07,-9.777356195150609444e-07
-2.149000000000000000e+03,-8.393841432072669604e-08,-1.222368651870388435e-06,-9.884922776127736314e-08,-1.291231622505305932e-06
-2.150000000000000000e+03,-8.333990177025244338e-08,-1.580014318279311620e-06,-9.799412904438990176e-08,-1.647692290811108905e-06
-2.151000000000000000e+03,-7.701052846634150217e-08,-1.832805086761552368e-06,-9.760465413984177302e-08,-1.927915435848830330e-06
-2.152000000000000000e+03,-6.798238613088619470e-08,-1.900141348737308391e-06,-9.445646747444521189e-08,-2.022407239422383996e-06
-2.153000000000000000e+03,-5.979682338542242003e-08,-1.864427516500166565e-06,-8.929635146224367733e-08,-2.000665901065659917e-06
-2.154000000000000000e+03,-5.482503204753372862e-08,-1.794547545648270446e-06,-8.389298416951503984e-08,-1.928792772535050912e-06
-2.155000000000000000e+03,-5.320243803443099880e-08,-1.643380724607711803e-06,-8.030315694253781581e-08,-1.768540630725161094e-06
-2.156000000000000000e+03,-5.437951293254305196e-08,-1.346991488941986417e-06,-7.969538632468820031e-08,-1.463908399810143974e-06
-2.157000000000000000e+03,-5.789862082423791998e-08,-9.960961750475912617e-07,-8.142325837538889216e-08,-1.104740578073679171e-06
-2.158000000000000000e+03,-6.284754466769536791e-08,-6.958177479566116669e-07,-8.417508208891262894e-08,-7.943152302709069079e-07
-2.159000000000000000e+03,-6.708668805648710881e-08,-4.712227305757844733e-07,-8.712118408504227547e-08,-5.637485285277452108e-07
-2.160000000000000000e+03,-6.851171931951445773e-08,-3.087605856613525499e-07,-9.037371770561284743e-08,-4.097263819866074644e-07
-2.161000000000000000e+03,-6.764757286862831086e-08,-1.796620780556543819e-07,-9.687955276794675889e-08,-3.146648383968723246e-07
-2.162000000000000000e+03,-6.574676914378509567e-08,-5.713547971324622297e-08,-1.099965343438687936e-07,-2.614952414207090895e-07
-2.163000000000000000e+03,-6.499328339052060883e-08,7.164547976095287440e-08,-1.309502712794862981e-07,-2.329652739229005564e-07
-2.164000000000000000e+03,-6.726990332827010524e-08,1.884952887729157452e-07,-1.551774762021243951e-07,-2.174903828696608567e-07
-2.165000000000000000e+03,-7.353676177695310584e-08,2.169744589310940735e-07,-1.667888664513961023e-07,-2.136939932927498947e-07
-2.166000000000000000e+03,-8.413796403428908205e-08,8.888325438612659716e-08,-1.528900066301012282e-07,-2.286359681058141084e-07
-2.167000000000000000e+03,-9.872406812582314406e-08,-1.514855009312064462e-07,-1.257042023273617865e-07,-2.760885077795089264e-07
-2.168000000000000000e+03,-1.175853115583195639e-07,-4.419741529349269156e-07,-1.004704256726792806e-07,-3.629320611763643231e-07
-2.169000000000000000e+03,-1.427054543451145073e-07,-7.470200557295141296e-07,-8.161289466970097849e-08,-4.648748086098107067e-07
-2.170000000000000000e+03,-1.723588388433230849e-07,-1.024575418287755815e-06,-6.847663402260736971e-08,-5.448137172523985101e-07
-2.171000000000000000e+03,-1.950250707265487344e-07,-1.194484170909607637e-06,-5.963066267936398421e-08,-5.691888989475018043e-07
-2.172000000000000000e+03,-1.998851278275308113e-07,-1.183857375473409965e-06,-5.395344667862771950e-08,-5.098975600865731427e-07
-2.173000000000000000e+03,-1.935285802236432974e-07,-1.040570158645975698e-06,-5.074488659292241341e-08,-3.811487702127031352e-07
-2.174000000000000000e+03,-1.859171331298628985e-07,-8.321796317797192019e-07,-4.965588883735238185e-08,-2.028810290036945737e-07
-2.175000000000000000e+03,-1.855012877809267076e-07,-6.210850354187868538e-07,-5.049436932067338323e-08,2.420684004647664811e-09
-2.176000000000000000e+03,-1.988738291469111411e-07,-4.467387033923499978e-07,-5.269651189412326579e-08,2.283555391587819165e-07
-2.177000000000000000e+03,-2.303630798640465088e-07,-3.235914824620337918e-07,-5.454766358449210236e-08,4.883811102268912608e-07
-2.178000000000000000e+03,-2.726955491354050465e-07,-2.549562820457891327e-07,-5.435400658277020204e-08,7.534157489726247595e-07
-2.179000000000000000e+03,-2.930336147057760202e-07,-2.336799800733527279e-07,-5.230920726780164094e-08,8.780633776315509785e-07
-2.180000000000000000e+03,-2.643610095706821221e-07,-2.487418308171336473e-07,-4.912526545384502425e-08,7.452866161080963647e-07
-2.181000000000000000e+03,-2.111630983875670266e-07,-2.787941052730023571e-07,-4.600815250706328342e-08,4.839449789308804571e-07
-2.182000000000000000e+03,-1.643651726575921939e-07,-2.989285951351373597e-07,-4.388976181361392193e-08,2.574659109228862583e-07
-2.183000000000000000e+03,-1.324955921239623716e-07,-2.878990672972887990e-07,-4.305521735339423940e-08,1.251655804469867597e-07
-2.184000000000000000e+03,-1.141146845626860961e-07,-2.336190969197584548e-07,-4.352528294963808963e-08,9.238564519551950370e-08
-2.185000000000000000e+03,-1.066003351680353482e-07,-1.591746004631764612e-07,-4.521195203568825693e-08,1.243368552882126354e-07
-2.186000000000000000e+03,-1.087505267405327618e-07,-9.016408576175231011e-08,-4.788727540225505552e-08,1.909221411140533594e-07
-2.187000000000000000e+03,-1.211608317253786388e-07,-3.532230944703271500e-08,-5.094090792895109787e-08,2.889760643243831258e-07
-2.188000000000000000e+03,-1.455851623464676784e-07,3.362689963104532837e-09,-5.343153721706311773e-08,4.289580075149445955e-07
-2.189000000000000000e+03,-1.823578279916982654e-07,2.512990836633856784e-08,-5.438426546679164588e-08,6.161533098282644518e-07
-2.190000000000000000e+03,-2.235179819756205300e-07,3.048318418499085233e-08,-5.329753734636898396e-08,8.166163838727132636e-07
-2.191000000000000000e+03,-2.431636098421442211e-07,2.842401678586532862e-08,-5.184054413618308630e-08,9.120159621898498355e-07
-2.192000000000000000e+03,-2.208209354118648125e-07,2.781401123954239017e-08,-5.182868606898639945e-08,8.082750069072314979e-07
-2.193000000000000000e+03,-1.778225562264940104e-07,3.182949287486030693e-08,-5.390012546663909605e-08,6.041434544469235322e-07
-2.194000000000000000e+03,-1.395063650201008388e-07,4.222376633957987570e-08,-5.835651582578522367e-08,4.170000791394389977e-07
-2.195000000000000000e+03,-1.106100086470384745e-07,6.246544631724253238e-08,-6.570332357858213007e-08,2.698590769538286007e-07
-2.196000000000000000e+03,-8.771895391299280022e-08,9.817577352381268097e-08,-7.663837229140293222e-08,1.493494918368742202e-07
-2.197000000000000000e+03,-6.967595304376044473e-08,1.565596176639514946e-07,-9.190934852075717722e-08,5.387858916398017901e-08
-2.198000000000000000e+03,-5.638584641698272949e-08,2.474918846405217153e-07,-1.131309617308343601e-07,-1.457545495248681603e-08
-2.199000000000000000e+03,-4.689404163478474099e-08,3.766414476564649050e-07,-1.426964961684485376e-07,-6.580534705449439479e-08
-2.200000000000000000e+03,-4.006912231505316905e-08,5.180794084657741144e-07,-1.764097422842596446e-07,-1.115857769192569044e-07
-2.201000000000000000e+03,-3.505305365040053840e-08,5.739395878745321368e-07,-1.939905976548374661e-07,-1.600855187503205188e-07
-2.202000000000000000e+03,-3.127530049051558545e-08,4.638085360405868594e-07,-1.788551097842517594e-07,-2.177628694511578491e-07
-2.203000000000000000e+03,-2.836626988713783352e-08,2.591884916616907685e-07,-1.476417089897968489e-07,-2.916641558575846386e-07
-2.204000000000000000e+03,-2.608196122150003457e-08,4.623050557079039977e-08,-1.208386270989733493e-07,-3.913864980755362424e-07
-2.205000000000000000e+03,-2.426050133781378366e-08,-1.652666801395977769e-07,-1.033789243456399379e-07,-5.306612082108793902e-07
-2.206000000000000000e+03,-2.279029095729046571e-08,-3.998719219241419830e-07,-9.358092725550538011e-08,-7.268060310568954512e-07
-2.207000000000000000e+03,-2.159271033926134575e-08,-6.788670785174915813e-07,-8.955827158217300134e-08,-9.927540751402246147e-07
-2.208000000000000000e+03,-2.061083084880333261e-08,-9.873763083533659384e-07,-9.031136812341126312e-08,-1.309275986779096067e-06
-2.209000000000000000e+03,-1.980373436337979236e-08,-1.228814977631218274e-06,-9.565641444386388520e-08,-1.579127246092494511e-06
-2.210000000000000000e+03,-1.914124014668018548e-08,-1.288090944122461031e-06,-1.062879295993284312e-07,-1.690562609443382950e-06
-2.211000000000000000e+03,-1.860006965341247505e-08,-1.140746995978099278e-06,-1.240305229290669174e-07,-1.627659010328895972e-06
-2.212000000000000000e+03,-1.816219316775964912e-08,-7.992110741727987969e-07,-1.517354994222013875e-07,-1.416095907644955407e-06
-2.213000000000000000e+03,-1.781407214765971636e-08,-3.707204830656178214e-07,-1.925803233835742926e-07,-1.177847691438026218e-06
-2.214000000000000000e+03,-1.754497870224438330e-08,3.649529235512543601e-08,-2.471010932704317096e-07,-1.023669268056080727e-06
-2.215000000000000000e+03,-1.734931772016959394e-08,3.545822411487833678e-07,-3.066976484846740571e-07,-9.817221586172621034e-07
-2.216000000000000000e+03,-1.722493962906866626e-08,5.193451603010003253e-07,-3.533872319919080637e-07,-1.033161291465988816e-06
-2.217000000000000000e+03,-1.717053854284145293e-08,4.684897390855506861e-07,-3.611787847686737093e-07,-1.120251871321464991e-06
-2.218000000000000000e+03,-1.718888876671323659e-08,1.677251984816854604e-07,-3.133435755521761429e-07,-1.200013160046622214e-06
-2.219000000000000000e+03,-1.728422867991922074e-08,-2.659389298867604241e-07,-2.421280525225385818e-07,-1.304340603977125094e-06
-2.220000000000000000e+03,-1.746120199448418582e-08,-6.736919238185880261e-07,-1.823746036968590674e-07,-1.435315478697941039e-06
-2.221000000000000000e+03,-1.772282232782196898e-08,-9.032106891264592766e-07,-1.411219426847838253e-07,-1.473107833597895849e-06
-2.222000000000000000e+03,-1.806943704904709031e-08,-8.643408411428454918e-07,-1.140392861352746009e-07,-1.307560718167764405e-06
-2.223000000000000000e+03,-1.848984641240423781e-08,-6.835148878272346143e-07,-9.625771982978971276e-08,-1.042672140034371260e-06
-2.224000000000000000e+03,-1.898502361460873937e-08,-5.068433755186280742e-07,-8.441983519022227316e-08,-8.090425496950330758e-07
-2.225000000000000000e+03,-1.960187845821027801e-08,-3.768836605035763992e-07,-7.642480335955551809e-08,-6.393103499979199230e-07
-2.226000000000000000e+03,-2.039470096443062052e-08,-2.894390118291499530e-07,-7.098090320806452231e-08,-5.230624941109269261e-07
-2.227000000000000000e+03,-2.140129451392975834e-08,-2.375278558637354423e-07,-6.737446845404107467e-08,-4.498468778710911928e-07
-2.228000000000000000e+03,-2.264520843450491831e-08,-2.161550804016266984e-07,-6.519970798498405243e-08,-4.126855557249128133e-07
-2.229000000000000000e+03,-2.413647105616795228e-08,-2.167010346387760736e-07,-6.420169029725290703e-08,-4.017352064551249075e-07
-2.230000000000000000e+03,-2.592918288317723465e-08,-2.245135714672166770e-07,-6.422875884390340658e-08,-4.013934301837568871e-07
-2.231000000000000000e+03,-2.820722967647478600e-08,-2.151993504191293915e-07,-6.519989076205816475e-08,-3.860434525333807858e-07
-2.232000000000000000e+03,-3.115993209401526452e-08,-1.706580303660832937e-07,-6.711934859926831802e-08,-3.367302740248818175e-07
-2.233000000000000000e+03,-3.483642746188162877e-08,-1.100461717384760564e-07,-7.003108604415881317e-08,-2.725865153703123674e-07
-2.234000000000000000e+03,-3.917873472906268917e-08,-5.642180307355173605e-08,-7.406526631219248903e-08,-2.175391163268840141e-07
-2.235000000000000000e+03,-4.406002424673050651e-08,-1.511042868881217408e-08,-7.947964275378259315e-08,-1.786897101864847068e-07
-2.236000000000000000e+03,-4.954571753202881717e-08,1.895506513322837715e-08,-8.666993514623320762e-08,-1.524966076815339816e-07
-2.237000000000000000e+03,-5.650851837533336029e-08,5.776617412427091531e-08,-9.624778665257852874e-08,-1.257626504659982863e-07
-2.238000000000000000e+03,-6.628893158552955737e-08,1.135779249690446703e-07,-1.090850357889357200e-07,-8.406835897099505152e-08
-2.239000000000000000e+03,-8.084492717943367965e-08,1.913944196943831156e-07,-1.264528634003095776e-07,-1.923781611349716153e-08
-2.240000000000000000e+03,-1.029754218899876415e-07,2.994520686851180289e-07,-1.503541797430546618e-07,8.064160446981760524e-08
-2.241000000000000000e+03,-1.361522693951454328e-07,4.553804432909721336e-07,-1.840192720296863961e-07,2.343151063832229623e-07
-2.242000000000000000e+03,-1.819056639927715928e-07,6.853318343412574963e-07,-2.325990984331026518e-07,4.512131190098740881e-07
-2.243000000000000000e+03,-2.338786931682051501e-07,1.013435944187351040e-06,-3.029462095415872636e-07,6.944597615122855457e-07
-2.244000000000000000e+03,-2.770816229675710803e-07,1.445798261395511375e-06,-3.981487963552129826e-07,8.866708040582284226e-07
-2.245000000000000000e+03,-2.874816723654337380e-07,1.922854407696313746e-06,-5.058271133910827152e-07,9.144643722656144195e-07
-2.246000000000000000e+03,-2.489594908014769512e-07,2.311053459464753464e-06,-5.972120545008780823e-07,7.027102149340902054e-07
-2.247000000000000000e+03,-1.891522653818264189e-07,2.399704273414761346e-06,-6.270671044824953706e-07,3.772715720858643395e-07
-2.248000000000000000e+03,-1.385076680303153607e-07,2.044337173233462308e-06,-5.649478808472773417e-07,7.489801621869755939e-08
-2.249000000000000000e+03,-1.033415430025506641e-07,1.474326284062816877e-06,-4.620197494467019293e-07,-1.821659587129322243e-07
-2.250000000000000000e+03,-8.005160880008180696e-08,9.382664767504322527e-07,-3.745749966250075224e-07,-4.219380143021587022e-07
-2.251000000000000000e+03,-6.452566769615872528e-08,4.833837777953282770e-07,-3.168615169444429405e-07,-6.819849826818936464e-07
-2.252000000000000000e+03,-5.394344089614902951e-08,6.673287724359681223e-08,-2.855736129212826995e-07,-1.003010352924445233e-06
-2.253000000000000000e+03,-4.655824389804282688e-08,-3.594029375870634632e-07,-2.774495494608043377e-07,-1.425733842887363054e-06
-2.254000000000000000e+03,-4.129843429543412987e-08,-8.003640912466156198e-07,-2.926183265256782273e-07,-1.961040832835761311e-06
-2.255000000000000000e+03,-3.752918848598071827e-08,-1.164858160755786441e-06,-3.346690284038145266e-07,-2.537146275841362980e-06
-2.256000000000000000e+03,-3.486861384624882484e-08,-1.338794451332527651e-06,-4.111904854942855772e-07,-3.076770860191614613e-06
-2.257000000000000000e+03,-3.306776324692213060e-08,-1.307766748422301907e-06,-5.289284643929789760e-07,-3.597812227039033058e-06
-2.258000000000000000e+03,-3.195089371080488485e-08,-1.123459032126051590e-06,-6.699415111084900487e-07,-4.069906543281240673e-06
-2.259000000000000000e+03,-3.135092372708989816e-08,-9.796823777103254709e-07,-7.570597803273098629e-07,-4.331241156230935839e-06
-2.260000000000000000e+03,-3.112647620097666193e-08,-9.856316323163756032e-07,-7.258710576241975811e-07,-4.194187349283930702e-06
-2.261000000000000000e+03,-3.119531837989670995e-08,-9.745826523820776308e-07,-6.284948404144729338e-07,-3.733105492876983086e-06
-2.262000000000000000e+03,-3.146400167618049244e-08,-7.710103297910164307e-07,-5.317682098902293161e-07,-3.081577364656786287e-06
-2.263000000000000000e+03,-3.183162401919094359e-08,-4.596237095587747082e-07,-4.599635995909211303e-07,-2.436875975453704415e-06
-2.264000000000000000e+03,-3.223969167113618649e-08,-1.721050025100736841e-07,-4.148242389970060325e-07,-1.939004478042758994e-06
-2.265000000000000000e+03,-3.287013584631362028e-08,6.253401662543537832e-08,-3.930671097080976337e-07,-1.600972386477562041e-06
-2.266000000000000000e+03,-3.394603282724163397e-08,2.545745765060999215e-07,-3.902502184100450901e-07,-1.390953668261527314e-06
-2.267000000000000000e+03,-3.563116859661900914e-08,4.048222083628752247e-07,-4.014508907163812756e-07,-1.284651869120896545e-06
-2.268000000000000000e+03,-3.808708730663353709e-08,5.136646371262773601e-07,-4.215111703990410624e-07,-1.257112086758319383e-06
-2.269000000000000000e+03,-4.151121673050578062e-08,6.124475449557371782e-07,-4.478519057852561926e-07,-1.264165494950698646e-06
-2.270000000000000000e+03,-4.621229684030418258e-08,7.200258655380770493e-07,-4.775597691570268376e-07,-1.272076606806683808e-06
-2.271000000000000000e+03,-5.266868908028728527e-08,8.044929105499143238e-07,-5.099042233849953733e-07,-1.307169025105235302e-06
-2.272000000000000000e+03,-6.159797384990142573e-08,7.933345232077982187e-07,-5.399295319830717168e-07,-1.415755689932343087e-06
-2.273000000000000000e+03,-7.406558550511541875e-08,6.059027127660972387e-07,-5.599828669757427098e-07,-1.638220830079000865e-06
-2.274000000000000000e+03,-9.182619653215645700e-08,2.440508834579743481e-07,-5.650883563668132345e-07,-1.941627204813254728e-06
-2.275000000000000000e+03,-1.175333674955397833e-07,-2.925148916744153129e-08,-5.720027720933904484e-07,-2.128138541042094942e-06
-2.276000000000000000e+03,-1.535066101453718319e-07,-1.348300917059733274e-08,-5.894704654169575167e-07,-2.026905434657265846e-06
-2.277000000000000000e+03,-1.987202580481402224e-07,6.247144315897847199e-08,-5.975171041899443818e-07,-1.779301684420751571e-06
-2.278000000000000000e+03,-2.465447202564662291e-07,-3.589059844803194752e-08,-5.720438505904575839e-07,-1.539151110910933236e-06
-2.279000000000000000e+03,-2.808888713958966384e-07,-1.430683178669794940e-07,-5.235418849310924373e-07,-1.263718603793391308e-06
-2.280000000000000000e+03,-2.855563637766030174e-07,-3.038513578032028537e-08,-4.702231588418772748e-07,-8.832362653666293342e-07
-2.281000000000000000e+03,-2.635106506093276401e-07,2.570499851742959687e-07,-4.324512072753184465e-07,-5.231722769524810746e-07
-2.282000000000000000e+03,-2.224668321811498564e-07,5.995503720303167035e-07,-4.225224830831252277e-07,-3.243714829602662851e-07
-2.283000000000000000e+03,-1.771395820862608054e-07,9.351124932460130476e-07,-4.359348761637065002e-07,-2.600880776392660959e-07
-2.284000000000000000e+03,-1.388577588757052316e-07,1.206161637213887735e-06,-4.561715290536019147e-07,-2.592962283100847077e-07
-2.285000000000000000e+03,-1.107015419711401983e-07,1.315105213082456197e-06,-4.564257759589119091e-07,-2.815613851417199770e-07
-2.286000000000000000e+03,-9.196441014496115952e-08,1.193498526281148063e-06,-4.179012463870914861e-07,-3.117834539721647892e-07
-2.287000000000000000e+03,-8.037873941855632891e-08,9.643060470080896321e-07,-3.651380215343320674e-07,-3.508046383037064499e-07
-2.288000000000000000e+03,-7.382447323077997141e-08,7.578658314411389021e-07,-3.260681166639656776e-07,-4.070770926883333331e-07
-2.289000000000000000e+03,-7.075434735928416620e-08,5.938443415649853223e-07,-3.065635741106976320e-07,-4.951991182011874946e-07
-2.290000000000000000e+03,-6.997694317500572561e-08,4.395729199645425812e-07,-3.027446439528212519e-07,-6.354237867763654954e-07
-2.291000000000000000e+03,-7.039108926088173066e-08,2.606564404221200434e-07,-3.099727550083312609e-07,-8.458093656728962090e-07
-2.292000000000000000e+03,-7.138148168778242201e-08,5.963907658927356202e-08,-3.226016151142620700e-07,-1.100576946501744319e-06
-2.293000000000000000e+03,-7.370952876676824880e-08,-6.626549384718094618e-08,-3.336961116244041061e-07,-1.266967822541651586e-06
-2.294000000000000000e+03,-7.825557911307248372e-08,-3.240355759162730574e-08,-3.359794438266582705e-07,-1.222655920311400586e-06
-2.295000000000000000e+03,-8.509916543703635316e-08,9.283277903671658917e-08,-3.292617420991134868e-07,-1.034789158818172715e-06
-2.296000000000000000e+03,-9.445226190683161860e-08,2.153419539106607240e-07,-3.152218850248789409e-07,-8.042437403556945669e-07
-2.297000000000000000e+03,-1.078321696449776581e-07,3.074784754750573942e-07,-3.021295508591136769e-07,-5.898498232348712754e-07
-2.298000000000000000e+03,-1.278481297955096131e-07,3.782708350014533728e-07,-2.981463683926808876e-07,-4.082216424513480829e-07
-2.299000000000000000e+03,-1.582905647071786270e-07,4.625352273474828872e-07,-3.097395073636661624e-07,-2.369050904074339633e-07
-2.300000000000000000e+03,-2.030193594619982971e-07,5.711272828306766286e-07,-3.370979426298178794e-07,-4.809108324097061012e-08
-2.301000000000000000e+03,-2.623567836695920964e-07,6.388417012300922629e-07,-3.673281925607678929e-07,1.540497026714928969e-07
-2.302000000000000000e+03,-3.269052967996570609e-07,5.708237333229826766e-07,-3.829465131300533078e-07,3.120072274434330758e-07
-2.303000000000000000e+03,-3.681323165100374336e-07,3.107218150380255707e-07,-3.748401242228972627e-07,2.797429843124576037e-07
-2.304000000000000000e+03,-3.607710696904526407e-07,-1.541633049299725008e-07,-3.412038572335125575e-07,-6.379557400759396884e-08
-2.305000000000000000e+03,-3.205874120594435245e-07,-7.006278775594459083e-07,-3.034543879687378833e-07,-6.215020176893871036e-07
-2.306000000000000000e+03,-2.695930056220628649e-07,-1.208035833817643639e-06,-2.795127692301528596e-07,-1.253848518200877667e-06
-2.307000000000000000e+03,-2.223659046352281666e-07,-1.669811247450344461e-06,-2.646606156234134398e-07,-1.865141934968098531e-06
-2.308000000000000000e+03,-1.857569737028340533e-07,-2.076731625710658320e-06,-2.486952081197663605e-07,-2.367400797164440239e-06
-2.309000000000000000e+03,-1.613532178343654590e-07,-2.346958555317523687e-06,-2.332282674962950183e-07,-2.678900836936595195e-06
-2.310000000000000000e+03,-1.488858816774031041e-07,-2.374403981639718267e-06,-2.211677752860587129e-07,-2.708225200505781694e-06
-2.311000000000000000e+03,-1.475940235694839892e-07,-2.182950559918984596e-06,-2.100435518799033417e-07,-2.471362728131724706e-06
-2.312000000000000000e+03,-1.578655028398433438e-07,-1.839405158195118900e-06,-1.958181689622824876e-07,-2.014682874808401768e-06
-2.313000000000000000e+03,-1.817583627756907188e-07,-1.507974672252344274e-06,-1.800328895256537206e-07,-1.500005877375902921e-06
-2.314000000000000000e+03,-2.208888739805351098e-07,-1.320989496779901930e-06,-1.645103867342531633e-07,-1.060615364465735238e-06
-2.315000000000000000e+03,-2.712535292755634158e-07,-1.273544994240895870e-06,-1.496717220502445279e-07,-7.120407909941439048e-07
-2.316000000000000000e+03,-3.190763034909100199e-07,-1.286334343537526721e-06,-1.349635581890916366e-07,-4.360419953847904610e-07
-2.317000000000000000e+03,-3.355363583190071359e-07,-1.233772895280169259e-06,-1.213972528629632276e-07,-2.448090812266740450e-07
-2.318000000000000000e+03,-2.997331546956171829e-07,-1.025598813220224127e-06,-1.101057977686167396e-07,-1.498382007154480256e-07
-2.319000000000000000e+03,-2.405351393240723746e-07,-7.506022465562312427e-07,-1.020725079235504910e-07,-1.111369244137897959e-07
-2.320000000000000000e+03,-1.911014087513079898e-07,-5.196421567827314986e-07,-9.727963330139090633e-08,-8.634278022739830677e-08
-2.321000000000000000e+03,-1.591001828020010365e-07,-3.605866500103960050e-07,-9.369728197181047790e-08,-5.853485000199057991e-08
-2.322000000000000000e+03,-1.407662767491298351e-07,-2.632638232766122018e-07,-8.941820782255884033e-08,-2.612179365172782659e-08
-2.323000000000000000e+03,-1.299598241258085105e-07,-2.051874840920568163e-07,-8.530223611624578349e-08,1.055735567943193104e-09
-2.324000000000000000e+03,-1.220612026503138748e-07,-1.706428930081770282e-07,-8.220315587128439197e-08,1.343448921196560778e-08
-2.325000000000000000e+03,-1.167013384648751890e-07,-1.597467967089709002e-07,-7.899901513996035560e-08,1.437475570285391329e-08
-2.326000000000000000e+03,-1.148365419924825999e-07,-1.773659609764255831e-07,-7.437710621206648296e-08,9.488830625691209482e-09
-2.327000000000000000e+03,-1.173363471494769373e-07,-2.203496429626343193e-07,-6.939493635957910461e-08,1.059334930079520120e-09
-2.328000000000000000e+03,-1.250719055886216141e-07,-2.876838882309934165e-07,-6.539468847188138398e-08,-1.207515190896448324e-08
-2.329000000000000000e+03,-1.391861717469746108e-07,-3.886142020123801606e-07,-6.261167553714097121e-08,-3.496835264907046730e-08
-2.330000000000000000e+03,-1.617381405503088558e-07,-5.401258770533876189e-07,-6.072809068981783053e-08,-7.362871879253762661e-08
-2.331000000000000000e+03,-1.963579269431503683e-07,-7.596619996559956902e-07,-5.922689332186821914e-08,-1.263464277692930300e-07
-2.332000000000000000e+03,-2.487983824346803793e-07,-1.037108772222783263e-06,-5.772357563160146086e-08,-1.546633669191894250e-07
-2.333000000000000000e+03,-3.260467903100308278e-07,-1.289764029736070765e-06,-5.633555905838936659e-08,-4.415012197441718380e-08
-2.334000000000000000e+03,-4.294168526430576252e-07,-1.425802817392282263e-06,-5.526713266861226980e-08,3.021418908148247887e-07
-2.335000000000000000e+03,-5.408401144010881075e-07,-1.441086209544501480e-06,-5.451499539420587507e-08,8.049208592661593280e-07
-2.336000000000000000e+03,-6.284874306031815118e-07,-1.343307779441403764e-06,-5.400508544878506470e-08,1.309837940768539383e-06
-2.337000000000000000e+03,-6.557754880954895752e-07,-1.157388105630775349e-06,-5.367994233624217215e-08,1.623284327321522471e-06
-2.338000000000000000e+03,-5.976641492031654932e-07,-9.051845273973885977e-07,-5.350810629895522877e-08,1.607904497069797208e-06
-2.339000000000000000e+03,-4.927184790377064880e-07,-6.507495336575409572e-07,-5.346952092610846992e-08,1.377844561792432710e-06
-2.340000000000000000e+03,-3.845465960074301458e-07,-4.466212722682669482e-07,-5.355508701878686989e-08,1.082004825480716615e-06
-2.341000000000000000e+03,-2.952353491175456259e-07,-2.984423361487097839e-07,-5.375254961005846364e-08,8.168035220080193104e-07
-2.342000000000000000e+03,-2.316624789655978269e-07,-1.940169869993953131e-07,-5.403293191803013651e-08,6.263338497272330643e-07
-2.343000000000000000e+03,-1.895234165993446277e-07,-1.204919913149868948e-07,-5.431758060700534535e-08,5.039323937617617551e-07
-2.344000000000000000e+03,-1.622511241307243298e-07,-6.827068462519840140e-08,-5.453498314176060816e-08,4.291973766179935600e-07
-2.345000000000000000e+03,-1.446182433570120388e-07,-3.060393969942922842e-08,-5.469827841547371095e-08,3.846756109401170352e-07
-2.346000000000000000e+03,-1.331678732949807402e-07,-2.641059173435155561e-09,-5.484663579425410676e-08,3.590718077742029787e-07
-2.347000000000000000e+03,-1.262784242684478396e-07,1.939915772103229412e-08,-5.503172356271703480e-08,3.484395201462442827e-07
-2.348000000000000000e+03,-1.232904876838025587e-07,3.822283311839585058e-08,-5.529096380394121151e-08,3.522666802094333871e-07
-2.349000000000000000e+03,-1.243630969360185138e-07,5.459798548831750713e-08,-5.561964816925134887e-08,3.720775188915624521e-07
-2.350000000000000000e+03,-1.300545279474884214e-07,6.878682441881224052e-08,-5.600682473517643313e-08,4.107631245195953779e-07
-2.351000000000000000e+03,-1.411889015669366409e-07,8.099791085416141724e-08,-5.644502293650419103e-08,4.723726167938118033e-07
-2.352000000000000000e+03,-1.590206032747402129e-07,9.136921448175786136e-08,-5.693665999314768846e-08,5.628259607233164538e-07
-2.353000000000000000e+03,-1.854342807175680124e-07,9.946976366732839978e-08,-5.747414803246392393e-08,6.904311417750193498e-07
-2.354000000000000000e+03,-2.242415604221963422e-07,1.052824412725337385e-07,-5.805733541661374994e-08,8.727750701738962024e-07
-2.355000000000000000e+03,-2.830248732307273783e-07,1.101180484553273477e-07,-5.868117266743689860e-08,1.146209991099075603e-06
-2.356000000000000000e+03,-3.725486476091683076e-07,1.150928892193673899e-07,-5.934561516484040741e-08,1.561566035166287751e-06
-2.357000000000000000e+03,-5.009964846661279952e-07,1.189094301338274148e-07,-6.004681467915954887e-08,2.155357964404261427e-06
-2.358000000000000000e+03,-6.505245989177760084e-07,1.200287858652114753e-07,-6.078752389811372401e-08,2.843625794258973490e-06
-2.359000000000000000e+03,-7.428328281977442653e-07,1.183064308472271284e-07,-6.156375381779250824e-08,3.264627887456615652e-06
-2.360000000000000000e+03,-7.099753490381251897e-07,1.156723418240128661e-07,-6.237706236365791575e-08,3.106491184557783080e-06
-2.361000000000000000e+03,-5.983658848544755896e-07,1.169485240232299623e-07,-6.322665820578459434e-08,2.588394967721774692e-06
-2.362000000000000000e+03,-4.720287367756733791e-07,1.261951092295656729e-07,-6.411760952293246917e-08,2.010060941878888705e-06
-2.363000000000000000e+03,-3.658120471541173589e-07,1.399446849743002749e-07,-6.504628894710172213e-08,1.528978466261661095e-06
-2.364000000000000000e+03,-2.924129785575318152e-07,1.539982780911157341e-07,-6.601861742549500108e-08,1.199560836076595010e-06
-2.365000000000000000e+03,-2.481146679319835276e-07,1.668011521201970272e-07,-6.703079334562167276e-08,1.003105193332668875e-06
-2.366000000000000000e+03,-2.259292380924988044e-07,1.785039369471922649e-07,-6.808692282927508790e-08,9.074709221660340965e-07
-2.367000000000000000e+03,-2.210988579082322928e-07,1.894833688504215703e-07,-6.919579492485404654e-08,8.910209615031888551e-07
-2.368000000000000000e+03,-2.320799615392784433e-07,1.999648371908411505e-07,-7.034894782036756571e-08,9.468910926151415525e-07
-2.369000000000000000e+03,-2.608360056755113285e-07,2.095134038916837704e-07,-7.154892631406111318e-08,1.083702504278919771e-06
-2.370000000000000000e+03,-3.127285920628351238e-07,2.177177362297514265e-07,-7.280028152601322104e-08,1.325784460346206965e-06
-2.371000000000000000e+03,-3.937359657799753653e-07,2.248355786670850264e-07,-7.411209651048137246e-08,1.700962230742688118e-06
-2.372000000000000000e+03,-4.929154780790559181e-07,2.311662062833702135e-07,-7.548244088489853128e-08,2.159007306096915421e-06
-2.373000000000000000e+03,-5.574945321110166114e-07,2.367108813582723047e-07,-7.691343135082841767e-08,2.456190211663882451e-06
-2.374000000000000000e+03,-5.397138818206175397e-07,2.416204719355103861e-07,-7.841016733666830186e-08,2.372070582584437412e-06
-2.375000000000000000e+03,-4.660279893313385455e-07,2.466746255678883887e-07,-7.997451772228971162e-08,2.029594718084329455e-06
-2.376000000000000000e+03,-3.753901941161336077e-07,2.528492991416296155e-07,-8.161867120869361421e-08,1.609581434246594377e-06
-2.377000000000000000e+03,-2.926729474995215168e-07,2.602235836105809579e-07,-8.333745438748118356e-08,1.227002758502335974e-06
-2.378000000000000000e+03,-2.285806206694718113e-07,2.688918645238177275e-07,-8.514342887870178954e-08,9.313313193278393203e-07
-2.379000000000000000e+03,-1.820353163701984065e-07,2.786645638672673638e-07,-8.704467592513024050e-08,7.173621379225689986e-07
-2.380000000000000000e+03,-1.486085990956059905e-07,2.894140406640871577e-07,-8.904739107366787698e-08,5.644870093755433304e-07
-2.381000000000000000e+03,-1.246011625056269448e-07,3.006406679899360428e-07,-9.115934439249675698e-08,4.550858260548805156e-07
-2.382000000000000000e+03,-1.074340348568661249e-07,3.119484102260752511e-07,-9.338718975322554231e-08,3.768212949779291747e-07
-2.383000000000000000e+03,-9.516789027704820501e-08,3.232332709231582004e-07,-9.575195859502304559e-08,3.205358540726390893e-07
-2.384000000000000000e+03,-8.644012529382654630e-08,3.343282988566260422e-07,-9.825402232264905193e-08,2.797678922481384073e-07
-2.385000000000000000e+03,-8.037241309029427063e-08,3.449181635994702581e-07,-1.009140616420763279e-07,2.500501708736537373e-07
-2.386000000000000000e+03,-7.639334566013722717e-08,3.549023827854840326e-07,-1.037398520188204835e-07,2.286073505356504565e-07
-2.387000000000000000e+03,-7.402624007148377163e-08,3.651803475131779086e-07,-1.067516865051957560e-07,2.140436261153641675e-07
-2.388000000000000000e+03,-7.301643743226979862e-08,3.767261656287744978e-07,-1.099785421524973646e-07,2.060231827162751375e-07
-2.389000000000000000e+03,-7.350548510713067032e-08,3.893975663218848461e-07,-1.134402962961093681e-07,2.049656611691592806e-07
-2.390000000000000000e+03,-7.576524424489653691e-08,4.033766651812464444e-07,-1.171805203485861538e-07,2.121074930776442509e-07
-2.391000000000000000e+03,-7.999794304965437278e-08,4.197231220321411929e-07,-1.212323457660061633e-07,2.292892818713967345e-07
-2.392000000000000000e+03,-8.661070875504544052e-08,4.398024520420595880e-07,-1.256610588568966737e-07,2.594552749367623015e-07
-2.393000000000000000e+03,-9.664323626351144334e-08,4.632472857554387951e-07,-1.305199533715747672e-07,3.067936231352843136e-07
-2.394000000000000000e+03,-1.119180998339398149e-07,4.895153034396913753e-07,-1.359032919267917859e-07,3.787439102257521849e-07
-2.395000000000000000e+03,-1.349234494762308651e-07,5.177642686058531495e-07,-1.418983729180801822e-07,4.855518108434462439e-07
-2.396000000000000000e+03,-1.654065238816569644e-07,5.476889354421788899e-07,-1.486358690908513076e-07,6.251412564032102366e-07
-2.397000000000000000e+03,-1.948544624279216147e-07,5.795201281021735395e-07,-1.562027991960408238e-07,7.580260399855054668e-07
-2.398000000000000000e+03,-2.113726266737282223e-07,6.143136813437314345e-07,-1.647256943581957186e-07,8.297443379648956495e-07
-2.399000000000000000e+03,-2.073570491966793969e-07,6.544472950260038802e-07,-1.744225351691058202e-07,8.065495583531166180e-07
-2.400000000000000000e+03,-1.801039451723443329e-07,7.025588644922246308e-07,-1.856240795743948431e-07,6.770650941660925251e-07
-2.401000000000000000e+03,-1.446355671878516218e-07,7.600624708208283463e-07,-1.988190087325830509e-07,5.098257712021236259e-07
-2.402000000000000000e+03,-1.156438048244447658e-07,8.291979129743940749e-07,-2.147534954302727125e-07,3.714772298583386089e-07
-2.403000000000000000e+03,-9.570554518167461833e-08,9.139105471437865772e-07,-2.344254467918591133e-07,2.732570677647278157e-07
-2.404000000000000000e+03,-8.262758022704895722e-08,1.018903522830745314e-06,-2.589326211621784684e-07,2.046696847434100178e-07
-2.405000000000000000e+03,-7.407157479614878596e-08,1.146650518856998330e-06,-2.888682062631841704e-07,1.546500365112512960e-07
-2.406000000000000000e+03,-6.846648347982499145e-08,1.298236913805231748e-06,-3.245535942258075938e-07,1.155436115523492558e-07
-2.407000000000000000e+03,-6.483361224616797634e-08,1.474009383337140117e-06,-3.662257422712568258e-07,8.208281392078248254e-08
-2.408000000000000000e+03,-6.258771164265277922e-08,1.684438704471571324e-06,-4.164152770355465706e-07,5.034829467462311283e-08
-2.409000000000000000e+03,-6.137172887918101857e-08,1.969582828098789161e-06,-4.842372053967911277e-07,1.665296226329543182e-08
-2.410000000000000000e+03,-6.096952036206648509e-08,2.383503899516999672e-06,-5.820727175595371861e-07,-2.311960961906089742e-08
-2.411000000000000000e+03,-6.125472554793724576e-08,2.983744736854704508e-06,-7.234331280134547259e-07,-7.440980755462093857e-08
-2.412000000000000000e+03,-6.216771540703923736e-08,3.844898278586849968e-06,-9.261677978553161786e-07,-1.453342156643106908e-07
-2.413000000000000000e+03,-6.369175257060325443e-08,5.017601286840517402e-06,-1.203984506328908557e-06,-2.486403391004301494e-07
-2.414000000000000000e+03,-6.584832564385463419e-08,6.276255349457375844e-06,-1.512107001285539868e-06,-4.030360995496043937e-07
-2.415000000000000000e+03,-6.869712403685126304e-08,6.789690155049025789e-06,-1.674655188098593685e-06,-6.271448450882254054e-07
-2.416000000000000000e+03,-7.238889781598913430e-08,5.934961017162780540e-06,-1.553274340558416958e-06,-9.042480685008153705e-07
-2.417000000000000000e+03,-7.718378126228071916e-08,4.468542929907453343e-06,-1.288303269174454180e-06,-1.124799516766774622e-06
-2.418000000000000000e+03,-8.351432518663054481e-08,3.295492809544311104e-06,-1.049711837034321286e-06,-1.166720546633319523e-06
-2.419000000000000000e+03,-9.195196602190197992e-08,2.666838316744017332e-06,-8.906772245349408726e-07,-1.021933878122851308e-06
-2.420000000000000000e+03,-1.033883279867445674e-07,2.531078649595787040e-06,-8.078993463555801810e-07,-7.225816395183556480e-07
-2.421000000000000000e+03,-1.192692741076662475e-07,2.677893420636151043e-06,-7.794659352484597531e-07,-3.711087998443320538e-07
-2.422000000000000000e+03,-1.419440725740535911e-07,2.917712852916067471e-06,-7.838550202683703389e-07,-4.684001454127532081e-08
-2.423000000000000000e+03,-1.752097931469587692e-07,3.171582960327043093e-06,-8.062664868298365812e-07,2.571585569024487121e-07
-2.424000000000000000e+03,-2.245057922327411474e-07,3.438824759709234381e-06,-8.425548486194257654e-07,5.844738424649041502e-07
-2.425000000000000000e+03,-2.940698155639794735e-07,3.823685536586043000e-06,-9.114548682897125341e-07,9.724012035215686057e-07
-2.426000000000000000e+03,-3.733146860561582882e-07,4.432414928958548281e-06,-1.033394429669180741e-06,1.383952671526608380e-06
-2.427000000000000000e+03,-4.173189443767253825e-07,5.279137809461343511e-06,-1.209871845463526594e-06,1.618871562300538981e-06
-2.428000000000000000e+03,-3.904107687802589510e-07,6.305771653857869276e-06,-1.427355952307024427e-06,1.516822613088036371e-06
-2.429000000000000000e+03,-3.303336214073045014e-07,7.363554335615861720e-06,-1.653026077184556551e-06,1.254931750780387148e-06
-2.430000000000000000e+03,-2.837976457737243307e-07,8.240691749763784187e-06,-1.840625491244331141e-06,1.050756027363288415e-06
-2.431000000000000000e+03,-2.642598599964160782e-07,8.778184011307659093e-06,-1.955467114745066366e-06,9.676406103290509029e-07
-2.432000000000000000e+03,-2.715988280650750602e-07,8.891261175084689091e-06,-1.979016220521821842e-06,1.005854102755671895e-06
-2.433000000000000000e+03,-3.037371037974635386e-07,8.864649815902067830e-06,-1.972812663397083825e-06,1.156317758337082572e-06
-2.434000000000000000e+03,-3.508463261925163037e-07,8.926025624426751667e-06,-1.986075463806478664e-06,1.374007316784807747e-06
-2.435000000000000000e+03,-3.827935413471794646e-07,9.040365071740487122e-06,-2.011173462566474447e-06,1.519978665962157705e-06
-2.436000000000000000e+03,-3.769916327889565372e-07,9.088905787683397458e-06,-2.022364950140238608e-06,1.490038369216515048e-06
-2.437000000000000000e+03,-3.601902800226459101e-07,9.157934810800869526e-06,-2.038324748755590680e-06,1.407765773910797936e-06
-2.438000000000000000e+03,-3.668581768660471346e-07,9.305377506473736443e-06,-2.071602790647969568e-06,1.432314192594376841e-06
-2.439000000000000000e+03,-4.099606551293858113e-07,9.471764128477630013e-06,-2.109355783172527362e-06,1.623406474072201059e-06
-2.440000000000000000e+03,-4.839404868140328021e-07,9.516767191242637861e-06,-2.121253100005104685e-06,1.955126717911541243e-06
-2.441000000000000000e+03,-5.577457478966517194e-07,9.402379733434125596e-06,-2.099147278052353544e-06,2.283687736452816431e-06
-2.442000000000000000e+03,-5.977479422766224993e-07,9.141798727086109810e-06,-2.046000521729614343e-06,2.453298783844102859e-06
-2.443000000000000000e+03,-5.982070703600375682e-07,8.976456099952695691e-06,-2.014245806474227973e-06,2.436730129151714004e-06
-2.444000000000000000e+03,-5.603011700817346199e-07,9.068240487416995025e-06,-2.039177200222670331e-06,2.238311520609537288e-06
-2.445000000000000000e+03,-4.989820500363765813e-07,9.306045170889517244e-06,-2.097169718532491564e-06,1.925096376678647015e-06
-2.446000000000000000e+03,-4.262775748422776154e-07,9.493987726454082310e-06,-2.146481078286831065e-06,1.549530248256957376e-06
-2.447000000000000000e+03,-3.541578908620226894e-07,9.608574340636849649e-06,-2.183094901834996119e-06,1.161950272681583781e-06
-2.448000000000000000e+03,-2.902339287566432890e-07,9.660707390912453977e-06,-2.211085460753216932e-06,7.895922656847981087e-07
-2.449000000000000000e+03,-2.395967915315074115e-07,9.738849841645039833e-06,-2.252342086790301229e-06,4.433395252168260570e-07
-2.450000000000000000e+03,-2.043187378998246895e-07,9.847536842223033701e-06,-2.311754020136805253e-06,1.147174669230556668e-07
-2.451000000000000000e+03,-1.818616156279755865e-07,9.892523687149263085e-06,-2.371999124753183507e-06,-2.222413844303090439e-07
-2.452000000000000000e+03,-1.689905507394473120e-07,9.785957965285466909e-06,-2.406513910240334604e-06,-5.476503260782662431e-07
-2.453000000000000000e+03,-1.636842707985974049e-07,9.729204678892982986e-06,-2.426519972715778419e-06,-7.213042161476621163e-07
-2.454000000000000000e+03,-1.653355054459289356e-07,9.903210347357951733e-06,-2.443890960376315394e-06,-6.198974635267211855e-07
-2.455000000000000000e+03,-1.746820076665505030e-07,1.029818019393874499e-05,-2.480786838859577862e-06,-3.521595681837595821e-07
-2.456000000000000000e+03,-1.936490249101790386e-07,1.085803150193941023e-05,-2.556346521742979261e-06,-5.367153775619506977e-08
-2.457000000000000000e+03,-2.238156456647016209e-07,1.168913597038622189e-05,-2.703246957392754132e-06,2.383183277694740035e-07
-2.458000000000000000e+03,-2.594333361972617103e-07,1.278762153674782120e-05,-2.919830024829903448e-06,5.010471136306186360e-07
-2.459000000000000000e+03,-2.775821574693632080e-07,1.383540832458969146e-05,-3.134003740456419885e-06,6.435273870116368465e-07
-2.460000000000000000e+03,-2.598251216125171597e-07,1.457238956072126025e-05,-3.286661979596109233e-06,5.934756336543092667e-07
-2.461000000000000000e+03,-2.244947929406233772e-07,1.536727113670861223e-05,-3.455825685640644383e-06,4.439374592478668121e-07
-2.462000000000000000e+03,-1.942177131995428739e-07,1.645160924001481018e-05,-3.690507693046048866e-06,3.046085969408738895e-07
-2.463000000000000000e+03,-1.743856285924086605e-07,1.740757783062272702e-05,-3.899562428553970962e-06,2.035036459110271629e-07
-2.464000000000000000e+03,-1.630080559345750602e-07,1.784542422396465507e-05,-3.998210753353936573e-06,1.332147738011274036e-07
-2.465000000000000000e+03,-1.574724361177785438e-07,1.836951402662999675e-05,-4.117283393903386637e-06,8.182323142241618615e-08
-2.466000000000000000e+03,-1.558719272132389639e-07,1.960515197643587743e-05,-4.392248774106960951e-06,4.019024116826110175e-08
-2.467000000000000000e+03,-1.566626926136422822e-07,2.153686117304755420e-05,-4.820025970091530792e-06,-6.232997052991039728e-11
-2.468000000000000000e+03,-1.588556138182798073e-07,2.365668525450781922e-05,-5.290985723943806272e-06,-4.515545842242850953e-08
-2.469000000000000000e+03,-1.625043271669394526e-07,2.511640087303370670e-05,-5.622093525282347469e-06,-9.775207224323074906e-08
-2.470000000000000000e+03,-1.679294266395795482e-07,2.521710407915475505e-05,-5.662968980943761944e-06,-1.607701041993696220e-07
-2.471000000000000000e+03,-1.752682913952222396e-07,2.444822846639903521e-05,-5.521092108535899242e-06,-2.405190661840789859e-07
-2.472000000000000000e+03,-1.846279189223005308e-07,2.341459186756924391e-05,-5.329789993169834133e-06,-3.474346807097670407e-07
-2.473000000000000000e+03,-1.961887879537618835e-07,2.266926305238205439e-05,-5.212675236764452778e-06,-4.984977402951138272e-07
-2.474000000000000000e+03,-2.102866097780614830e-07,2.234332300550172592e-05,-5.203998342585702723e-06,-7.192567649871134667e-07
-2.475000000000000000e+03,-2.273639893740149517e-07,2.205302934557034334e-05,-5.228730713607551681e-06,-1.044903657112946732e-06
-2.476000000000000000e+03,-2.482153688949429979e-07,2.133588493566388603e-05,-5.194158266846706186e-06,-1.506082868545593163e-06
-2.477000000000000000e+03,-2.741842948643063807e-07,2.040788175158861364e-05,-5.144469220339228421e-06,-2.084673006998467871e-06
-2.478000000000000000e+03,-3.073592314903637154e-07,1.970129253963734728e-05,-5.145934130406671604e-06,-2.644815035739749108e-06
-2.479000000000000000e+03,-3.507951915510212070e-07,1.992389180828459447e-05,-5.279019309483303699e-06,-2.836244925270497288e-06
-2.480000000000000000e+03,-4.087338231875266150e-07,2.147177799288822647e-05,-5.570177336715272311e-06,-2.365441520517576616e-06
-2.481000000000000000e+03,-4.850622007316914289e-07,2.375636655367813140e-05,-5.956180043980857759e-06,-1.511029412475680769e-06
-2.482000000000000000e+03,-5.766205797709390215e-07,2.587452970668957647e-05,-6.322099277979008962e-06,-6.599536369392043043e-07
-2.483000000000000000e+03,-6.635005767106101951e-07,2.732111571399559719e-05,-6.586026958612458909e-06,-3.103123274876922703e-08
-2.484000000000000000e+03,-7.333470316303334003e-07,2.790882212574890845e-05,-6.709418937152122099e-06,3.093845911789752156e-07
-2.485000000000000000e+03,-8.175889937742333283e-07,2.834086667579567429e-05,-6.842804201687989212e-06,5.144694382549038716e-07
-2.486000000000000000e+03,-9.579358143002950664e-07,2.903926490131476549e-05,-7.080602056091470520e-06,7.628071951752181638e-07
-2.487000000000000000e+03,-1.179954156063950209e-06,2.962416214859879085e-05,-7.351955156204455584e-06,1.119860533806254397e-06
-2.488000000000000000e+03,-1.485985456587498890e-06,2.974162747550402252e-05,-7.600343057992454648e-06,1.503541764374244324e-06
-2.489000000000000000e+03,-1.829435081099223874e-06,3.026685407017615183e-05,-8.036614921805892213e-06,1.600085164478481616e-06
-2.490000000000000000e+03,-2.152997982701133277e-06,3.163399509453420510e-05,-8.736753804300813236e-06,1.228076221100558242e-06
-2.491000000000000000e+03,-2.437186284893833153e-06,3.270728936539076307e-05,-9.335877943436963949e-06,8.468946930486446909e-07
-2.492000000000000000e+03,-2.669516663143029146e-06,3.248299671397016607e-05,-9.509748143966455724e-06,8.925900954438025964e-07
-2.493000000000000000e+03,-2.869128239529898129e-06,3.190589233079078792e-05,-9.554763678673938525e-06,1.029460353613632719e-06
-2.494000000000000000e+03,-3.036831231875075437e-06,3.194100717585954101e-05,-9.773853993020875980e-06,8.272518856302211610e-07
-2.495000000000000000e+03,-3.167049338139686276e-06,3.282028508373223630e-05,-1.017039794350450968e-05,4.765507006186975482e-07
-2.496000000000000000e+03,-3.228189946836997320e-06,3.428859509227511398e-05,-1.059316989203512742e-05,2.747299389728791857e-07
-2.497000000000000000e+03,-3.211708342942977718e-06,3.573215907333663878e-05,-1.093142565484256755e-05,8.000175283198429951e-08
-2.498000000000000000e+03,-3.115112956431216879e-06,3.665814842652942256e-05,-1.110272647251535000e-05,-2.312404182994298582e-07
-2.499000000000000000e+03,-3.013483519575835512e-06,3.766975565341756661e-05,-1.123128114831650758e-05,-2.826980505948819102e-07
-2.500000000000000000e+03,-2.946312069726336375e-06,3.916928914829895643e-05,-1.139643400852528110e-05,1.438864596381342866e-07
-2.501000000000000000e+03,-2.871235074946066873e-06,4.072552479425964431e-05,-1.162223706021685446e-05,3.105605040516043422e-07
-2.502000000000000000e+03,-2.741379734554395441e-06,4.173932471221660260e-05,-1.186065734829823403e-05,-3.764558272328299555e-07
-2.503000000000000000e+03,-2.635339063501919459e-06,4.275958201729604055e-05,-1.213302200307843187e-05,-1.103796997904266470e-06
-2.504000000000000000e+03,-2.616761324169945699e-06,4.416313979975604461e-05,-1.240390088562340744e-05,-1.037043738676143661e-06
-2.505000000000000000e+03,-2.643911023604826491e-06,4.550664296616220599e-05,-1.266499631250819186e-05,-7.739777881052100905e-07
-2.506000000000000000e+03,-2.647941649170866324e-06,4.625737617458999367e-05,-1.289490663721122315e-05,-1.066430261713584225e-06
-2.507000000000000000e+03,-2.637682266614045530e-06,4.734938134652865875e-05,-1.323196275213684674e-05,-1.578440658713725098e-06
-2.508000000000000000e+03,-2.640368242949965186e-06,4.943166352532985609e-05,-1.370302626276821113e-05,-1.659277783821625477e-06
-2.509000000000000000e+03,-2.702336323817330141e-06,5.186568467351873932e-05,-1.417204867786598899e-05,-1.105165520328037110e-06
-2.510000000000000000e+03,-2.844870621894330962e-06,5.375537263696798394e-05,-1.448121251915193710e-05,1.497319038214517971e-08
-2.511000000000000000e+03,-3.044809436071146510e-06,5.539241380520009469e-05,-1.476645333356042580e-05,1.258062066174027055e-06
-2.512000000000000000e+03,-3.230828911517956835e-06,5.685761909713927783e-05,-1.508109414296200459e-05,2.129252338177180442e-06
-2.513000000000000000e+03,-3.304640956446841224e-06,5.798748377389287896e-05,-1.535346853920939751e-05,2.342091701552455065e-06
-2.514000000000000000e+03,-3.187116549997459377e-06,5.832200381982751260e-05,-1.545105660134798631e-05,1.683152626920764760e-06
-2.515000000000000000e+03,-2.961927102116396114e-06,5.799119869076693816e-05,-1.549514074816845378e-05,1.087547375710970049e-07
-2.516000000000000000e+03,-2.725062222913045968e-06,5.739419369299822465e-05,-1.562680816621469089e-05,-2.190251889062468983e-06
-2.517000000000000000e+03,-2.552291866430662506e-06,5.843432403024003460e-05,-1.611012411752129399e-05,-4.180140827923693648e-06
-2.518000000000000000e+03,-2.483465393291220681e-06,6.153427071496819420e-05,-1.686147427055313146e-05,-4.868035708557697671e-06
-2.519000000000000000e+03,-2.535057050181694427e-06,6.343081052870449101e-05,-1.724999922656383718e-05,-4.527563105758592502e-06
-2.520000000000000000e+03,-2.724832981165670157e-06,6.177832168646283100e-05,-1.692778077955997242e-05,-3.815495919102765696e-06
-2.521000000000000000e+03,-3.091408704741583675e-06,5.960439578681359497e-05,-1.671870807095143522e-05,-3.330890730585558738e-06
-2.522000000000000000e+03,-3.598902215563682275e-06,5.906012437223849445e-05,-1.712228019082182089e-05,-3.395219469867983795e-06
-2.523000000000000000e+03,-4.021516000079715088e-06,5.876564903426374239e-05,-1.755064889699291453e-05,-3.716272901822570800e-06
-2.524000000000000000e+03,-4.151095058601120245e-06,5.732915006019327473e-05,-1.738322188021028993e-05,-3.781101529161227676e-06
-2.525000000000000000e+03,-4.080388737903375934e-06,5.553985659666164926e-05,-1.692201863647717621e-05,-3.766953600898647669e-06
-2.526000000000000000e+03,-3.938835828810825926e-06,5.357189948321262332e-05,-1.641770839778364886e-05,-4.059579758359892131e-06
-2.527000000000000000e+03,-3.814473107994313796e-06,5.110703769499106683e-05,-1.583423136887274825e-05,-4.404102824456909877e-06
-2.528000000000000000e+03,-3.707069813002716141e-06,4.809770580773382263e-05,-1.508260978774967186e-05,-4.438225807302402027e-06
-2.529000000000000000e+03,-3.545661137074945630e-06,4.610606747802987966e-05,-1.448296636919969347e-05,-4.405954017500525529e-06
-2.530000000000000000e+03,-3.253311121057582831e-06,4.587815853491323485e-05,-1.417912046012220442e-05,-4.580771199434721520e-06
-2.531000000000000000e+03,-2.891319649256095094e-06,4.631189429448676211e-05,-1.396044371048618140e-05,-4.808909290230240765e-06
-2.532000000000000000e+03,-2.529256586345682121e-06,4.615537987384714857e-05,-1.356941885619392380e-05,-4.831668768698916575e-06
-2.533000000000000000e+03,-2.220737852894824937e-06,4.584970790772949353e-05,-1.314183837747416723e-05,-4.587474994702287981e-06
-2.534000000000000000e+03,-1.990149315134729557e-06,4.573734986869572072e-05,-1.278004531177293045e-05,-4.093887986485483849e-06
-2.535000000000000000e+03,-1.846164790509884791e-06,4.575356881377615789e-05,-1.251153058176858187e-05,-3.502548179595630914e-06
-2.536000000000000000e+03,-1.771971467982503670e-06,4.548726898553810086e-05,-1.226059208635411172e-05,-2.952581497699031321e-06
-2.537000000000000000e+03,-1.717452450388780245e-06,4.505685309628328235e-05,-1.201693907973855182e-05,-2.509515307387667509e-06
-2.538000000000000000e+03,-1.639724247977030609e-06,4.449110101292813618e-05,-1.173048611780416217e-05,-2.111308781570056134e-06
-2.539000000000000000e+03,-1.571745532056194198e-06,4.401704658262967616e-05,-1.143259519116376329e-05,-1.523554083981952903e-06
-2.540000000000000000e+03,-1.555876925737755369e-06,4.346973248331718512e-05,-1.107976831640971920e-05,-5.146856559636639575e-07
-2.541000000000000000e+03,-1.606235677918843663e-06,4.263936404816406732e-05,-1.065247872407901672e-05,8.608808200182697331e-07
-2.542000000000000000e+03,-1.687113510397256545e-06,4.117552920342145231e-05,-1.010219920733687412e-05,2.311935238606319709e-06
-2.543000000000000000e+03,-1.691064971937241198e-06,3.947629553915360789e-05,-9.544270852395557583e-06,3.207644731328032730e-06
-2.544000000000000000e+03,-1.539934818479208208e-06,3.778573897338926711e-05,-9.050129444633222823e-06,3.101225344046898185e-06
-2.545000000000000000e+03,-1.343658947812261816e-06,3.641459304942021470e-05,-8.683450267824535825e-06,2.517057133514929795e-06
-2.546000000000000000e+03,-1.231633978065243774e-06,3.546106998352177662e-05,-8.453819662841144186e-06,2.106675019521803846e-06
-2.547000000000000000e+03,-1.237918525060247342e-06,3.517183456013157905e-05,-8.398707608637196855e-06,2.100989005578913256e-06
-2.548000000000000000e+03,-1.325692185465263332e-06,3.540969159533114677e-05,-8.472382736883042468e-06,2.403957633109996259e-06
-2.549000000000000000e+03,-1.377959380252798055e-06,3.564232715656760601e-05,-8.548253521968480768e-06,2.527584161938959512e-06
-2.550000000000000000e+03,-1.293120861904440739e-06,3.547540137824327269e-05,-8.530254328899630105e-06,2.051972709802695011e-06
-2.551000000000000000e+03,-1.112167875935926044e-06,3.571367672775905747e-05,-8.590088466109875858e-06,1.178215059989842803e-06
-2.552000000000000000e+03,-9.035232939228228225e-07,3.674716450363082944e-05,-8.800915453496969404e-06,2.744471334173966094e-07
-2.553000000000000000e+03,-7.172221044301640098e-07,3.774683851757025971e-05,-8.963022636137021071e-06,-3.349416710327931255e-07
-2.554000000000000000e+03,-5.777261649011263048e-07,3.777734068143429714e-05,-8.859970586430949724e-06,-4.727492056776331037e-07
-2.555000000000000000e+03,-4.803147526971061274e-07,3.731569245437399635e-05,-8.634286953825126204e-06,-3.419947323739880949e-07
-2.556000000000000000e+03,-4.125667805851876013e-07,3.668701437229539644e-05,-8.397440260157710960e-06,-1.897200955881625076e-07
-2.557000000000000000e+03,-3.645393088880928015e-07,3.582008658124573932e-05,-8.140800506359675582e-06,-9.320873466424306415e-08
-2.558000000000000000e+03,-3.297497096289664867e-07,3.441505020982449289e-05,-7.792930884417888124e-06,-5.234005909838783307e-08
-2.559000000000000000e+03,-3.040982863272410209e-07,3.285223467360644446e-05,-7.430171015405126565e-06,-5.827950063943338662e-08
-2.560000000000000000e+03,-2.849023923240521590e-07,3.135405163255180902e-05,-7.097960947089313225e-06,-1.108616038281825528e-07
-2.561000000000000000e+03,-2.702086175569309339e-07,3.002153797254521704e-05,-6.818733832907140467e-06,-2.216745392750682587e-07
-2.562000000000000000e+03,-2.587244557759565505e-07,2.867041267704641667e-05,-6.555631738559625461e-06,-4.107466462854135269e-07
-2.563000000000000000e+03,-2.500615704249549288e-07,2.718734088394640506e-05,-6.285951042437600624e-06,-6.883535658572570133e-07
-2.564000000000000000e+03,-2.441595893683565518e-07,2.538575874440456365e-05,-5.957093258285189218e-06,-9.984211026825676735e-07
-2.565000000000000000e+03,-2.408527705602694456e-07,2.349803335471826343e-05,-5.574541642259175797e-06,-1.134671065599731389e-06
-2.566000000000000000e+03,-2.400216884407694065e-07,2.177863982560818924e-05,-5.156729811024493588e-06,-9.283123078792125064e-07
-2.567000000000000000e+03,-2.416058836917215142e-07,2.066130962670122877e-05,-4.833357990731826763e-06,-5.448902745059652236e-07
-2.568000000000000000e+03,-2.457810969625142163e-07,2.013749978572108621e-05,-4.647558097417302765e-06,-1.913334823169071978e-07
-2.569000000000000000e+03,-2.530917832191563891e-07,1.942539856285093697e-05,-4.441106424690359950e-06,8.378917151337439561e-08
-2.570000000000000000e+03,-2.644466428874828044e-07,1.785583682706397054e-05,-4.065210563317004563e-06,3.026768142775003198e-07
-2.571000000000000000e+03,-2.810388626931638357e-07,1.611609011932875043e-05,-3.663319764219128536e-06,4.956203622995881716e-07
-2.572000000000000000e+03,-3.048253196646822888e-07,1.491589075001523166e-05,-3.385270787400868534e-06,6.893948829092415703e-07
-2.573000000000000000e+03,-3.391216099947584532e-07,1.422929719716776183e-05,-3.223044023747231313e-06,9.104085071967736364e-07
-2.574000000000000000e+03,-3.894441464287712840e-07,1.377929840148753180e-05,-3.115159096866799420e-06,1.191063068818899791e-06
-2.575000000000000000e+03,-4.641922062873568650e-07,1.355986013868899143e-05,-3.059361539320461169e-06,1.574526790792322779e-06
-2.576000000000000000e+03,-5.728505115047511669e-07,1.354281085051276106e-05,-3.048964291892808839e-06,2.107314643185732722e-06
-2.577000000000000000e+03,-7.171012216766703400e-07,1.355083173411934276e-05,-3.045166099198984167e-06,2.799073358482269791e-06
-2.578000000000000000e+03,-8.698635062816154736e-07,1.329144045728897549e-05,-2.984366186609253981e-06,3.525981546317611913e-06
-2.579000000000000000e+03,-9.462992409655151145e-07,1.262709686512854121e-05,-2.836590547514354183e-06,3.897118768809087383e-06
-2.580000000000000000e+03,-8.821804586208775286e-07,1.145256967322714273e-05,-2.578918984039690092e-06,3.616481071025822292e-06
-2.581000000000000000e+03,-7.561361018093362069e-07,9.991954584665111241e-06,-2.259774694413480244e-06,3.047664076245722753e-06
-2.582000000000000000e+03,-6.616813831897467826e-07,8.482093496711003462e-06,-1.930366467039957709e-06,2.622894464917017930e-06
-2.583000000000000000e+03,-6.256230420320214817e-07,7.223144071126479618e-06,-1.655634826199734809e-06,2.466215716442365116e-06
-2.584000000000000000e+03,-6.471700891009768584e-07,6.427195301519802793e-06,-1.481462823133536070e-06,2.574160973535637853e-06
-2.585000000000000000e+03,-7.202076113153697202e-07,6.115526045785510055e-06,-1.412427069584543430e-06,2.918632166201944406e-06
-2.586000000000000000e+03,-8.232018163243272572e-07,6.201800877712912234e-06,-1.429794383168118369e-06,3.400359743433607029e-06
-2.587000000000000000e+03,-8.949350304052561531e-07,6.476423703768787914e-06,-1.488104876535785923e-06,3.736973045462059350e-06
-2.588000000000000000e+03,-8.796523349786076720e-07,6.680756346414049493e-06,-1.531300952685524007e-06,3.671231761833178044e-06
-2.589000000000000000e+03,-7.986497837450796429e-07,6.616415209525816337e-06,-1.516447484723668828e-06,3.301392712505385267e-06
-2.590000000000000000e+03,-6.895657812767911982e-07,6.172796923964036534e-06,-1.419634709592563864e-06,2.801101920702145353e-06
-2.591000000000000000e+03,-5.885621881355394793e-07,5.584378772329760011e-06,-1.291641564793959821e-06,2.337330268780309355e-06
-2.592000000000000000e+03,-5.176519687147113380e-07,5.058939002838885961e-06,-1.177448551906669768e-06,2.011784472033560665e-06
-2.593000000000000000e+03,-4.765085587005973423e-07,4.577482247659506082e-06,-1.072933671615217594e-06,1.822997711968729572e-06
-2.594000000000000000e+03,-4.582090297988080228e-07,4.067455424729577110e-06,-9.623800669715287847e-07,1.739030120085773296e-06
-2.595000000000000000e+03,-4.571662442406986963e-07,3.626184722735165689e-06,-8.668607194912895209e-07,1.734082810860694692e-06
-2.596000000000000000e+03,-4.706228465419761642e-07,3.373005839513363210e-06,-8.122132674492762122e-07,1.795430530299388872e-06
-2.597000000000000000e+03,-4.985347180332877792e-07,3.336849502389875043e-06,-8.047065122268615859e-07,1.922848894250449591e-06
-2.598000000000000000e+03,-5.435319934192908121e-07,3.491781650745948353e-06,-8.387215324318601526e-07,2.128500657538997328e-06
-2.599000000000000000e+03,-6.113126763946924772e-07,3.750068427515829328e-06,-8.952543129091006605e-07,2.438733894676279964e-06
-2.600000000000000000e+03,-7.115604876024050875e-07,3.967406325055096408e-06,-9.430540084355915084e-07,2.898294194394523133e-06
-2.601000000000000000e+03,-8.580739488232394026e-07,3.959048776163975022e-06,-9.421459635287768571e-07,3.570776955651413357e-06
-2.602000000000000000e+03,-1.065494889362070157e-06,3.608874377569328951e-06,-8.674205312698389567e-07,4.523645980018656444e-06
-2.603000000000000000e+03,-1.334909485491682845e-06,3.137735465659687310e-06,-7.667244908751331672e-07,5.761797979450709638e-06
-2.604000000000000000e+03,-1.629361174385299191e-06,2.791607876730750007e-06,-6.933263123472513650e-07,7.114520337193060621e-06
-2.605000000000000000e+03,-1.836298616967198713e-06,2.645437090040108051e-06,-6.634342604416876070e-07,8.062104937449993748e-06
-2.606000000000000000e+03,-1.857145721823177872e-06,2.695040685039518449e-06,-6.761212476149858022e-07,8.149394601462365282e-06
-2.607000000000000000e+03,-1.753504603844476278e-06,2.898578714867045953e-06,-7.223708519763912821e-07,7.660688680139482397e-06
-2.608000000000000000e+03,-1.616957454893663140e-06,3.153273095679536704e-06,-7.800006607478113044e-07,7.018610916969599694e-06
-2.609000000000000000e+03,-1.530861940242449027e-06,3.240845142648567641e-06,-8.019037620218582035e-07,6.607410341859713636e-06
-2.610000000000000000e+03,-1.545339814039722304e-06,2.990851234152659001e-06,-7.513538782785985596e-07,6.657735700037084927e-06
-2.611000000000000000e+03,-1.658673026244000633e-06,2.563388694128650071e-06,-6.632125428540351872e-07,7.160747940102330632e-06
-2.612000000000000000e+03,-1.852473039788400880e-06,2.157319726543542163e-06,-5.807881520039455005e-07,8.030372825458549133e-06
-2.613000000000000000e+03,-2.107697422880541490e-06,1.846536213462674374e-06,-5.204440651370481267e-07,9.176986815655184751e-06
-2.614000000000000000e+03,-2.378234237114099943e-06,1.636560071890181048e-06,-4.839344956946764095e-07,1.038505041999828141e-05
-2.615000000000000000e+03,-2.573075977219870246e-06,1.505486090345316030e-06,-4.674430833642163014e-07,1.122998145175625113e-05
-2.616000000000000000e+03,-2.631264386130008010e-06,1.431868120339687085e-06,-4.677962106937440808e-07,1.142346556260132753e-05
-2.617000000000000000e+03,-2.664818594994114915e-06,1.409612415346332985e-06,-4.857163080429018337e-07,1.147341325324761635e-05
-2.618000000000000000e+03,-2.758991020685719551e-06,1.451108932941926226e-06,-5.252946522888911229e-07,1.176704293865587525e-05
-2.619000000000000000e+03,-2.837593793289636969e-06,1.599268939961397181e-06,-5.935192293631071353e-07,1.196313281729869241e-05
-2.620000000000000000e+03,-2.802500902460461031e-06,1.920575425133898529e-06,-6.966708129876692535e-07,1.164598149983666429e-05
-2.621000000000000000e+03,-2.715734000080491196e-06,2.471798143135045777e-06,-8.304428554722795751e-07,1.117868387053310427e-05
-2.622000000000000000e+03,-2.654874613851286224e-06,3.177604080973630759e-06,-9.664725770425455407e-07,1.097519207603889408e-05
-2.623000000000000000e+03,-2.645001467276667651e-06,3.634137563112512296e-06,-1.034940448786289050e-06,1.106992133700124968e-05
-2.624000000000000000e+03,-2.667991444830617026e-06,3.505100321062334332e-06,-9.829531269946415222e-07,1.128715357137546042e-05
-2.625000000000000000e+03,-2.695565773115314121e-06,3.072254046754042452e-06,-8.750747856440900008e-07,1.147987163993167622e-05
-2.626000000000000000e+03,-2.704592951136128635e-06,2.707507718103654978e-06,-7.886116462553460831e-07,1.155613055555658384e-05
-2.627000000000000000e+03,-2.734972640102561641e-06,2.561834109099909800e-06,-7.532680470712150138e-07,1.171398839907803540e-05
-2.628000000000000000e+03,-2.818457739081090174e-06,2.679957192793854845e-06,-7.770481092990507616e-07,1.210784869918287619e-05
-2.629000000000000000e+03,-2.947013570668990225e-06,3.084389161596024925e-06,-8.650884149770135313e-07,1.269939450199001483e-05
-2.630000000000000000e+03,-3.080661496211955257e-06,3.803361567006473772e-06,-1.024123666752160756e-06,1.330112000415161693e-05
-2.631000000000000000e+03,-3.181039276826561725e-06,4.827750916707255573e-06,-1.252118203145580728e-06,1.373613380162261218e-05
-2.632000000000000000e+03,-3.210405477480762418e-06,5.975200630629074368e-06,-1.509295643964248192e-06,1.383147735082733503e-05
-2.633000000000000000e+03,-3.192485941968232842e-06,6.703292338710859481e-06,-1.678144797807599382e-06,1.369701070004328144e-05
-2.634000000000000000e+03,-3.141824537288972171e-06,6.544060736953499515e-06,-1.657378381281597201e-06,1.339971435087714197e-05
-2.635000000000000000e+03,-3.070293167961245123e-06,5.804836453782916665e-06,-1.513789035550366802e-06,1.299327716432405652e-05
-2.636000000000000000e+03,-2.996662485487261429e-06,4.911681843549922815e-06,-1.340024267449087893e-06,1.256257422553067017e-05
-2.637000000000000000e+03,-3.018270658452948796e-06,4.165363375068617912e-06,-1.201978435319189445e-06,1.255358971327370665e-05
-2.638000000000000000e+03,-3.214515032323694692e-06,3.652429533858504152e-06,-1.119346219526162755e-06,1.332859837643129033e-05
-2.639000000000000000e+03,-3.561669212174246373e-06,3.173628852510405578e-06,-1.050265949447873928e-06,1.477210333031702706e-05
-2.640000000000000000e+03,-3.987227204917982675e-06,2.512914000598237849e-06,-9.499128261831638287e-07,1.654021651536331734e-05
-2.641000000000000000e+03,-4.411475684618356413e-06,1.748818675491916260e-06,-8.386629316138332475e-07,1.824922629410697899e-05
-2.642000000000000000e+03,-4.766833015063580676e-06,1.004416989153606222e-06,-7.479968168295441176e-07,1.956470548105459121e-05
-2.643000000000000000e+03,-5.078562257506904065e-06,3.006200355871035455e-07,-6.893023039316165997e-07,2.057164552304119266e-05
-2.644000000000000000e+03,-5.362167993955635625e-06,-4.032684440886974299e-07,-6.641307358645676124e-07,2.129379074289331804e-05
-2.645000000000000000e+03,-5.625481518216171966e-06,-1.167580421902378578e-06,-6.733503416606239156e-07,2.170296685917280885e-05
-2.646000000000000000e+03,-5.871226316469067327e-06,-2.002645165488391931e-06,-7.204828487270014549e-07,2.178515806746636179e-05
-2.647000000000000000e+03,-6.192772818424779079e-06,-2.784316158596444735e-06,-8.108527354343239851e-07,2.207113563228578043e-05
-2.648000000000000000e+03,-6.627382866909580147e-06,-3.387742550074113860e-06,-9.440364595327173321e-07,2.285979373087104039e-05
-2.649000000000000000e+03,-7.088187821517461674e-06,-3.899870909783651122e-06,-1.099008157750650581e-06,2.376010250196798949e-05
-2.650000000000000000e+03,-7.479202570150948162e-06,-4.455138267085701022e-06,-1.246808871356547891e-06,2.432807640973042905e-05
-2.651000000000000000e+03,-7.892651917480020992e-06,-5.198198444188449075e-06,-1.367819132652685052e-06,2.493559474226293634e-05
-2.652000000000000000e+03,-8.369181709309165214e-06,-6.153973253273794225e-06,-1.446619952456957338e-06,2.581666127187476004e-05
-2.653000000000000000e+03,-8.796339936192405212e-06,-7.098778472622640743e-06,-1.499457785970828156e-06,2.660058898580401645e-05
-2.654000000000000000e+03,-9.023362721290918183e-06,-7.668287635965728583e-06,-1.542788758636215507e-06,2.687942816615733593e-05
-2.655000000000000000e+03,-9.098333524597464691e-06,-7.602451877072676570e-06,-1.600104067912657431e-06,2.702680272048817205e-05
-2.656000000000000000e+03,-9.068765348608330145e-06,-6.721881734404476006e-06,-1.692037321118318034e-06,2.734623987171357561e-05
-2.657000000000000000e+03,-9.016480302754323391e-06,-5.375220495967977528e-06,-1.846724242053390278e-06,2.773703746608578485e-05
-2.658000000000000000e+03,-8.998832137547263047e-06,-4.057692707915428356e-06,-2.053165929568650974e-06,2.801964566312301749e-05
-2.659000000000000000e+03,-9.164794207758519446e-06,-3.284442360638805335e-06,-2.217983769502702698e-06,2.879818043678542783e-05
-2.660000000000000000e+03,-9.584521433357446655e-06,-3.328610763075219451e-06,-2.249347122188844564e-06,3.054760230913071601e-05
-2.661000000000000000e+03,-1.017991832299240912e-05,-3.842887128023659304e-06,-2.192595740977645624e-06,3.304515808895045186e-05
-2.662000000000000000e+03,-1.076559426032191300e-05,-4.379357554632705582e-06,-2.129960133058670639e-06,3.550280056441224746e-05
-2.663000000000000000e+03,-1.119000837158058729e-05,-4.778119697887921583e-06,-2.169739308031972135e-06,3.688040725765189063e-05
-2.664000000000000000e+03,-1.145432968455151021e-05,-5.114228239645471863e-06,-2.374079339145024295e-06,3.682131172177034999e-05
-2.665000000000000000e+03,-1.205624845265987496e-05,-5.793553972011496146e-06,-2.681722142256243715e-06,3.750104780162241404e-05
-2.666000000000000000e+03,-1.328718402828466120e-05,-7.078429294443034259e-06,-2.977420808563958515e-06,4.053539973528711820e-05
-2.667000000000000000e+03,-1.471167257663864987e-05,-8.558006010243079443e-06,-3.156189547876442612e-06,4.480896096674801140e-05
-2.668000000000000000e+03,-1.582024446117235171e-05,-9.585389894417428562e-06,-3.152105232986910475e-06,4.892018414067469235e-05
-2.669000000000000000e+03,-1.669640778379044595e-05,-1.008946014319868648e-05,-3.069117741576210104e-06,5.284578331296583463e-05
-2.670000000000000000e+03,-1.746899585234460407e-05,-1.039183761875674861e-05,-3.036012369478755837e-06,5.626435935651293257e-05
-2.671000000000000000e+03,-1.825324173917716784e-05,-1.123727947500260478e-05,-3.176880779721193785e-06,5.839024327362187737e-05
-2.672000000000000000e+03,-1.910438921308063091e-05,-1.318841644703516951e-05,-3.567193579044498050e-06,5.856739023389726266e-05
-2.673000000000000000e+03,-2.023341885033148432e-05,-1.592504139747533300e-05,-4.173478590597155250e-06,5.824496944156951458e-05
-2.674000000000000000e+03,-2.137041649579362731e-05,-1.873919457824274408e-05,-4.845858553606160019e-06,5.757657134993912027e-05
-2.675000000000000000e+03,-2.155759791376149831e-05,-2.089609128200840856e-05,-5.290256877016513905e-06,5.423176358572657309e-05
-2.676000000000000000e+03,-2.023762613364672388e-05,-2.126483675838143739e-05,-5.268210187318487372e-06,4.786877924746683590e-05
-2.677000000000000000e+03,-1.833691288946436484e-05,-2.036937809178042608e-05,-4.934288848526935509e-06,4.152828493255367252e-05
-2.678000000000000000e+03,-1.655130715969532391e-05,-1.938090337523892034e-05,-4.482645497081510244e-06,3.635608890817069061e-05
-2.679000000000000000e+03,-1.508606201473384894e-05,-1.818777808324506523e-05,-4.077525555075208883e-06,3.265321231458651925e-05
-2.680000000000000000e+03,-1.377478140366792551e-05,-1.630728699443620986e-05,-3.752654711292847473e-06,2.997814329869221428e-05
-2.681000000000000000e+03,-1.236721734188976073e-05,-1.449313896510469919e-05,-3.382558083114784092e-06,2.700093036709893244e-05
-2.682000000000000000e+03,-1.070489817945345830e-05,-1.345454315326965531e-05,-2.849283057177116527e-06,2.282523431436081081e-05
-2.683000000000000000e+03,-9.153304986770320747e-06,-1.270096411805713205e-05,-2.281656887028531135e-06,1.903453463207219589e-05
-2.684000000000000000e+03,-7.976842769167486410e-06,-1.165615402215520330e-05,-1.816987191718528462e-06,1.679205609303597560e-05
-2.685000000000000000e+03,-7.110494968442798651e-06,-1.080603109030141104e-05,-1.461091489314186560e-06,1.528474574351219148e-05
-2.686000000000000000e+03,-6.379933635475138723e-06,-1.069366832773689980e-05,-1.173949155552745543e-06,1.334925580890186989e-05
-2.687000000000000000e+03,-5.728450405770978561e-06,-1.096372788065747552e-05,-9.440733162671412420e-07,1.113207663962955487e-05
-2.688000000000000000e+03,-5.116445622108440917e-06,-1.093277725019684624e-05,-7.698680141726257844e-07,9.141127327246585004e-06
-2.689000000000000000e+03,-4.536746653388351740e-06,-1.021615360407770125e-05,-6.409012109510708511e-07,7.776123703284872510e-06
-2.690000000000000000e+03,-3.969994381734471532e-06,-8.685185419298591843e-06,-5.445356770578711631e-07,7.134693431157784506e-06
-2.691000000000000000e+03,-3.438822079479466549e-06,-6.934164161640652888e-06,-4.710826075603475400e-07,6.771818876888005179e-06
-2.692000000000000000e+03,-2.953117356089070180e-06,-5.571528860311099971e-06,-4.137368561894843686e-07,6.156153569133199373e-06
-2.693000000000000000e+03,-2.520820183838669045e-06,-4.699509338224230221e-06,-3.680145707909093702e-07,5.242844934066835730e-06
-2.694000000000000000e+03,-2.141655542473390253e-06,-4.229373377625544837e-06,-3.308204696804203499e-07,4.133650071068091873e-06
-2.695000000000000000e+03,-1.832341893120029697e-06,-4.083371660149901805e-06,-3.000879354266374287e-07,2.993073881507940456e-06
-2.696000000000000000e+03,-1.604728883120708252e-06,-4.239858419983931145e-06,-2.743142774839916907e-07,1.904427556465348191e-06
-2.697000000000000000e+03,-1.450821253313675845e-06,-4.722582335167223236e-06,-2.524487060755349358e-07,8.118906068471352537e-07
-2.698000000000000000e+03,-1.359214609206643001e-06,-5.555535965059445113e-06,-2.336947482621076635e-07,-3.575203475843271901e-07
-2.699000000000000000e+03,-1.326314114071251211e-06,-6.668224030822248854e-06,-2.174819434657092956e-07,-1.547277577572169135e-06
-2.700000000000000000e+03,-1.355297281623675603e-06,-7.882858952935633987e-06,-2.033298900384530256e-07,-2.562700064529185381e-06
-2.701000000000000000e+03,-1.448881427240955333e-06,-8.882432296049376218e-06,-1.909076546632478876e-07,-3.072701572376925443e-06
-2.702000000000000000e+03,-1.583178999134176254e-06,-9.366121600466193801e-06,-1.799190215064080787e-07,-2.885412079298203268e-06
-2.703000000000000000e+03,-1.672737089313733655e-06,-9.466559583305034090e-06,-1.701698039876863891e-07,-2.527216719219516533e-06
-2.704000000000000000e+03,-1.647356188602140891e-06,-9.313653718750874706e-06,-1.614564813581185266e-07,-2.451287133967214169e-06
-2.705000000000000000e+03,-1.565716531223694450e-06,-8.905140220739337238e-06,-1.536450993475273601e-07,-2.383736547131059559e-06
-2.706000000000000000e+03,-1.484776236312329360e-06,-8.187745769144841665e-06,-1.466113715338692073e-07,-2.007666583303011925e-06
-2.707000000000000000e+03,-1.380692263119706469e-06,-7.436752038088029989e-06,-1.402614427828242530e-07,-1.708040355383814085e-06
-2.708000000000000000e+03,-1.216679772450810026e-06,-6.933169821504144339e-06,-1.345146529525714182e-07,-1.935380455869955425e-06
-2.709000000000000000e+03,-1.039480602818510914e-06,-6.788452948252252648e-06,-1.292965090649355197e-07,-2.584927716686685560e-06
-2.710000000000000000e+03,-9.031526545409165931e-07,-6.983138789996308206e-06,-1.245557225478317847e-07,-3.387325732711033245e-06
-2.711000000000000000e+03,-8.171604263261177463e-07,-7.383597138775337024e-06,-1.202377806670335925e-07,-4.164982415026347161e-06
-2.712000000000000000e+03,-7.743539281525010859e-07,-7.815784988785415488e-06,-1.163063529230030303e-07,-4.776707943788583497e-06
-2.713000000000000000e+03,-7.695003803314293847e-07,-8.200219795399467284e-06,-1.127200961752983227e-07,-5.166995511442071743e-06
-2.714000000000000000e+03,-8.009703647162376154e-07,-8.567189319450215599e-06,-1.094576652311812339e-07,-5.373559481066729653e-06
-2.715000000000000000e+03,-8.660792393194227180e-07,-9.256521129713662639e-06,-1.064984901002020612e-07,-5.748530969627516841e-06
-2.716000000000000000e+03,-9.546542578020022661e-07,-1.040455961733902137e-05,-1.038143660773972219e-07,-6.475105150454869715e-06
-2.717000000000000000e+03,-1.041818659476094509e-06,-1.143530245838944779e-05,-1.013911963050778889e-07,-7.092103541790012667e-06
-2.718000000000000000e+03,-1.113152484566619298e-06,-1.173475560390325970e-05,-9.921572855659107951e-08,-7.052066940862503720e-06
-2.719000000000000000e+03,-1.203776083548418234e-06,-1.167056505478256123e-05,-9.728782171130255134e-08,-6.560443532132989098e-06
-2.720000000000000000e+03,-1.329031310186298727e-06,-1.163768820496791679e-05,-9.558727045927842397e-08,-5.941243740272147268e-06
-2.721000000000000000e+03,-1.424193560228551929e-06,-1.138265671699120091e-05,-9.412807685445243171e-08,-5.239983100338012643e-06
-2.722000000000000000e+03,-1.420125353397314068e-06,-1.051553640932306577e-05,-9.290496694317501779e-08,-4.386002372642083739e-06
-2.723000000000000000e+03,-1.349815460124793730e-06,-9.406590316714834703e-06,-9.192428564299174768e-08,-3.597241057828023634e-06
-2.724000000000000000e+03,-1.261981718562131841e-06,-8.496707777960878460e-06,-9.119571162512495486e-08,-3.089638422762894905e-06
-2.725000000000000000e+03,-1.189949444227643102e-06,-7.824781876197345052e-06,-9.074001769705935763e-08,-2.748276374831156233e-06
-2.726000000000000000e+03,-1.146617294471398198e-06,-7.275579512500070108e-06,-9.057452687229924179e-08,-2.398431636944036189e-06
-2.727000000000000000e+03,-1.134514190175453681e-06,-6.909522343434990306e-06,-9.073462415656399248e-08,-2.089009908572716854e-06
-2.728000000000000000e+03,-1.144510477139428829e-06,-6.789425478646004126e-06,-9.126734652529356074e-08,-1.925207234344002093e-06
-2.729000000000000000e+03,-1.159828292109365322e-06,-6.870439255269177007e-06,-9.222290834817368885e-08,-1.939891469613830083e-06
-2.730000000000000000e+03,-1.157187973840319583e-06,-7.032703224117059389e-06,-9.368556110935903909e-08,-2.121104288884746452e-06
-2.731000000000000000e+03,-1.126727643342343987e-06,-7.174014455915131719e-06,-9.575009599644418010e-08,-2.412625893768498808e-06
-2.732000000000000000e+03,-1.064697522487592672e-06,-7.107939761531906072e-06,-9.855296682056574005e-08,-2.645970974165258783e-06
-2.733000000000000000e+03,-9.976528602584910446e-07,-6.604068778245502378e-06,-1.022931161257086217e-07,-2.469007199363172955e-06
-2.734000000000000000e+03,-9.378871287467916277e-07,-5.517341979485933924e-06,-1.072261249638459738e-07,-1.681080159221097844e-06
-2.735000000000000000e+03,-8.594227039685802299e-07,-4.253022920057637105e-06,-1.137375270867451344e-07,-8.092070180453274465e-07
-2.736000000000000000e+03,-7.356685521402454264e-07,-3.244229877039473070e-06,-1.223511052415269635e-07,-4.117310664239862036e-07
-2.737000000000000000e+03,-6.006429215023024675e-07,-2.566425367844874616e-06,-1.339078001967021463e-07,-4.108912596020613406e-07
-2.738000000000000000e+03,-4.928604823663780486e-07,-2.158086754827304016e-06,-1.496247459932074276e-07,-5.729128453717564706e-07
-2.739000000000000000e+03,-4.176278208984391598e-07,-1.957554557114218915e-06,-1.714713173128150370e-07,-8.207240182844844031e-07
-2.740000000000000000e+03,-3.672226819261492785e-07,-1.904016839339830777e-06,-2.025823383502815970e-07,-1.143654355415611190e-06
-2.741000000000000000e+03,-3.344834306000661610e-07,-1.878987724672588915e-06,-2.479613100269999086e-07,-1.479400520926189188e-06
-2.742000000000000000e+03,-3.150395136712295394e-07,-1.709139420636676051e-06,-3.149715232304968156e-07,-1.708825418738503183e-06
-2.743000000000000000e+03,-3.071513390946739652e-07,-1.194434630788583011e-06,-4.109385167404581659e-07,-1.673757465521781550e-06
-2.744000000000000000e+03,-3.112682038074329396e-07,-2.569626337001509904e-07,-5.296540669842025352e-07,-1.265539351729805192e-06
-2.745000000000000000e+03,-3.302471392016460204e-07,7.326488927977890889e-07,-6.320817337278327196e-07,-6.613211211340254791e-07
-2.746000000000000000e+03,-3.691587885988467903e-07,1.434146674477204670e-06,-6.902106407086646394e-07,-4.857486531478303601e-08
-2.747000000000000000e+03,-4.320611566294919936e-07,1.999547325885674715e-06,-7.459281032028704365e-07,5.500080092462432413e-07
-2.748000000000000000e+03,-5.061652330646882284e-07,2.555388209190548984e-06,-8.206396566752817619e-07,1.103043366645913276e-06
-2.749000000000000000e+03,-5.397854017723181673e-07,2.783486415299057758e-06,-8.388337206761901563e-07,1.402384325516735739e-06
-2.750000000000000000e+03,-4.914846291747616518e-07,2.374142181908568911e-06,-7.292323887701490431e-07,1.276145948986078879e-06
-2.751000000000000000e+03,-4.029022351533166120e-07,1.655000025929125284e-06,-5.605149448673909297e-07,9.270934335756178469e-07
-2.752000000000000000e+03,-3.249491672177049943e-07,1.020295437938063435e-06,-4.172684437387414726e-07,5.939350885545890576e-07
-2.753000000000000000e+03,-2.696269790954048806e-07,5.536174781252363230e-07,-3.175548369270964083e-07,3.322710921874617195e-07
-2.754000000000000000e+03,-2.321929911641290320e-07,2.152747973694817853e-07,-2.514770917359677192e-07,1.262145689189081035e-07
-2.755000000000000000e+03,-2.066448949007051050e-07,-2.083963285416576388e-08,-2.076497039516849444e-07,-2.548016681612568827e-08
-2.756000000000000000e+03,-1.887973710639581498e-07,-1.589488802356453245e-07,-1.782788729025331830e-07,-1.103710455721264527e-07
-2.757000000000000000e+03,-1.761076825601751967e-07,-2.079814127041805234e-07,-1.586226408777505125e-07,-1.272298214695538998e-07
-2.758000000000000000e+03,-1.670179988966088987e-07,-1.798330407515448114e-07,-1.459360953326323178e-07,-8.246997522581368840e-08
-2.759000000000000000e+03,-1.606253899650524886e-07,-1.146219154447302037e-07,-1.387256008855947831e-07,-1.348158944559465630e-08
-2.760000000000000000e+03,-1.563863106718971273e-07,-4.612756239235114756e-08,-1.364019650985170106e-07,4.616662449856218158e-08
-2.761000000000000000e+03,-1.540506162794955849e-07,2.182354865791434495e-08,-1.391641252675551208e-07,9.057419043204708997e-08
-2.762000000000000000e+03,-1.535178210325297952e-07,9.928240400127961364e-08,-1.480647873720192967e-07,1.244662813485563188e-07
-2.763000000000000000e+03,-1.549072024052418869e-07,2.017966758856016422e-07,-1.653468033464335422e-07,1.535832141640262245e-07
-2.764000000000000000e+03,-1.584832323538258833e-07,3.490290153899114701e-07,-1.945815148818748258e-07,1.823154434167249574e-07
-2.765000000000000000e+03,-1.647910046415842301e-07,5.594119680469490211e-07,-2.394096652168067122e-07,2.147988017367765571e-07
-2.766000000000000000e+03,-1.746795577818706572e-07,8.159774429364650319e-07,-2.960812252250034879e-07,2.553051836061408245e-07
-2.767000000000000000e+03,-1.894758239049254673e-07,1.012527307602484477e-06,-3.417300522805812058e-07,3.093679193184582809e-07
-2.768000000000000000e+03,-2.111717018475665852e-07,1.034048699165691626e-06,-3.518215549532151534e-07,3.844820780798547522e-07
-2.769000000000000000e+03,-2.427517387604588526e-07,8.797849130829750712e-07,-3.268448971037691161e-07,4.914154443962955671e-07
-2.770000000000000000e+03,-2.885840188063178446e-07,5.853389468694799165e-07,-2.756153274461253365e-07,6.452325680908094090e-07
-2.771000000000000000e+03,-3.539662360449124302e-07,2.418780535750167046e-07,-2.196618809151824256e-07,8.621391077632584830e-07
-2.772000000000000000e+03,-4.397735084919165478e-07,-8.513797712228340735e-08,-1.761209052925932566e-07,1.132495222053744441e-06
-2.773000000000000000e+03,-5.330553773969670155e-07,-4.094534672137952787e-07,-1.467737059551949020e-07,1.374520526113783052e-06
-2.774000000000000000e+03,-6.138644540502252183e-07,-7.804688152098128564e-07,-1.279162592361774872e-07,1.463797495477474150e-06
-2.775000000000000000e+03,-6.655350485510889518e-07,-1.244248339056785722e-06,-1.161461324649280623e-07,1.293007790290467965e-06
-2.776000000000000000e+03,-6.726249243564595404e-07,-1.773069339287735258e-06,-1.092759959487764276e-07,8.286586528718911843e-07
-2.777000000000000000e+03,-6.420929749345751683e-07,-2.168356271385527200e-06,-1.060494164731567063e-07,3.072666698134634019e-07
-2.778000000000000000e+03,-5.881600667776620292e-07,-2.265375415809282612e-06,-1.058371059779607692e-07,-3.785161112074420134e-08
-2.779000000000000000e+03,-5.459686112197619588e-07,-2.234196879114960519e-06,-1.084620950614236489e-07,-2.136499455142553774e-07
-2.780000000000000000e+03,-5.396156042096770228e-07,-2.224449601295579425e-06,-1.141303534879738415e-07,-2.594207688406015944e-07
-2.781000000000000000e+03,-5.551653188480384521e-07,-2.094907738910108483e-06,-1.234580368093438103e-07,-1.011435486170216902e-07
-2.782000000000000000e+03,-5.654252846334027083e-07,-1.671345439873898046e-06,-1.376209911278714346e-07,3.043934840030250459e-07
-2.783000000000000000e+03,-5.546320575838748268e-07,-1.103000832354749168e-06,-1.586184943505120968e-07,7.259181923984089718e-07
-2.784000000000000000e+03,-5.171690403732560033e-07,-5.766563945221912844e-07,-1.898080831359913362e-07,9.352026381943901409e-07
-2.785000000000000000e+03,-4.758447622501185794e-07,-1.087077000307539730e-07,-2.366590757368283319e-07,9.959293455823032863e-07
-2.786000000000000000e+03,-4.459121020893442964e-07,3.626515147460207952e-07,-3.071385550196914335e-07,1.003552746249052586e-06
-2.787000000000000000e+03,-4.105967621438141152e-07,8.964537592443695222e-07,-4.083873147734427415e-07,9.066577035155456763e-07
-2.788000000000000000e+03,-3.503113926733900666e-07,1.453829675907677252e-06,-5.292185695257604118e-07,6.275783305279700248e-07
-2.789000000000000000e+03,-2.814321122201093309e-07,1.781425885552455839e-06,-6.149567316819418806e-07,2.411010623901531124e-07
-2.790000000000000000e+03,-2.246642908148099866e-07,1.663472621165905310e-06,-6.219284691769373107e-07,-1.712221497080833671e-07
-2.791000000000000000e+03,-1.834583744377348291e-07,1.288791010906321071e-06,-5.961601098057907387e-07,-6.171994031606174044e-07
-2.792000000000000000e+03,-1.541134328683910720e-07,8.800034055542002194e-07,-5.882410185147197590e-07,-1.124938531474476231e-06
-2.793000000000000000e+03,-1.329172338030798747e-07,4.708247016748551668e-07,-5.948805923819378701e-07,-1.662671859264548366e-06
-2.794000000000000000e+03,-1.172787673615265686e-07,3.747638454883783129e-08,-5.872624105748296846e-07,-2.133060451052138437e-06
-2.795000000000000000e+03,-1.054294446027140955e-07,-3.537065540677611027e-07,-5.426611865526160781e-07,-2.372984491290620548e-06
-2.796000000000000000e+03,-9.620189305482460365e-08,-6.158108599268753308e-07,-4.505147674431266724e-07,-2.252142584004423522e-06
-2.797000000000000000e+03,-8.883676532976836045e-08,-7.374451178619098082e-07,-3.447960646435585667e-07,-1.919548145483769792e-06
-2.798000000000000000e+03,-8.281188732431114207e-08,-7.488102392466370549e-07,-2.594074909495024590e-07,-1.564385990038675955e-06
-2.799000000000000000e+03,-7.778661345491526306e-08,-7.421934452881163582e-07,-1.993065349326118387e-07,-1.303411840088654121e-06
-2.800000000000000000e+03,-7.353356349395749861e-08,-7.847473022812348863e-07,-1.581868496456698367e-07,-1.175703622783583651e-06
-2.801000000000000000e+03,-6.987632795744304822e-08,-8.506823099694403813e-07,-1.296440159652710912e-07,-1.126708870197666083e-06
-2.802000000000000000e+03,-6.668915955608508755e-08,-8.987516297522852753e-07,-1.092438802846490319e-07,-1.095283126547674466e-06
-2.803000000000000000e+03,-6.388455830672106330e-08,-9.494083998422740434e-07,-9.423093970361742708e-08,-1.089557827594306403e-06
-2.804000000000000000e+03,-6.138964983401178082e-08,-1.010214399021931920e-06,-8.286498754088133268e-08,-1.109394470973022082e-06
-2.805000000000000000e+03,-5.915333860347026662e-08,-1.015391170310157205e-06,-7.403940622228523755e-08,-1.084139856717570393e-06
-2.806000000000000000e+03,-5.713080818324679235e-08,-9.019125945678624756e-07,-6.703723002779714033e-08,-9.476636623615978883e-07
-2.807000000000000000e+03,-5.529171051450220834e-08,-7.311874910595477156e-07,-6.137952057329462655e-08,-7.593029716120356804e-07
-2.808000000000000000e+03,-5.360723485868682360e-08,-5.773730085460642414e-07,-5.673111713969769744e-08,-5.918001096993227531e-07
-2.809000000000000000e+03,-5.205730461774747308e-08,-4.551701344069277852e-07,-5.285940553399234432e-08,-4.588744964836068266e-07
-2.810000000000000000e+03,-5.062231645966711495e-08,-3.544872140219123174e-07,-4.959356468004232133e-08,-3.497361047767075165e-07
-2.811000000000000000e+03,-4.929028292630726095e-08,-2.724687611157240329e-07,-4.681471996791480495e-08,-2.610358087829520996e-07
-2.812000000000000000e+03,-4.804625965957465507e-08,-2.091308928010037214e-07,-4.443097991196171441e-08,-1.924343588332574017e-07
-2.813000000000000000e+03,-4.688260751947078205e-08,-1.618412768126984619e-07,-4.237764753097282098e-08,-1.410359110533935833e-07
-2.814000000000000000e+03,-4.578752160505498591e-08,-1.271089500873497772e-07,-4.060621315346315779e-08,-1.031799878496434968e-07
-2.815000000000000000e+03,-4.475623100519232990e-08,-1.013127918773577044e-07,-3.908742929755209206e-08,-7.513242773526668632e-08
-2.816000000000000000e+03,-4.378083563017521187e-08,-8.158193623536315412e-08,-3.780640602575484895e-08,-5.399008337972252672e-08
-2.817000000000000000e+03,-4.285793896862412229e-08,-6.588639316226093484e-08,-3.675657058258272120e-08,-3.770829585885399411e-08
-2.818000000000000000e+03,-4.197972576746819550e-08,-5.312875874511763973e-08,-3.587327619829372993e-08,-2.492719489065511205e-08
-2.819000000000000000e+03,-4.114496107476491122e-08,-4.334196415400896020e-08,-3.494437667741225618e-08,-1.470565514399857922e-08
-2.820000000000000000e+03,-4.034743811671090748e-08,-3.670522669277698735e-08,-3.379227755693838510e-08,-6.431370009199836073e-09
-2.821000000000000000e+03,-3.958657387007956422e-08,-3.205698967175605577e-08,-3.256528067290525161e-08,3.696186540675336335e-10
-2.822000000000000000e+03,-3.885776764433199217e-08,-2.822513666777927550e-08,-3.144774042331781257e-08,5.996771409812256924e-09
-2.823000000000000000e+03,-3.815880304419377644e-08,-2.476503160063141729e-08,-3.047934652967907901e-08,1.070118830478125760e-08
-2.824000000000000000e+03,-3.748744922698216938e-08,-2.160993225013853491e-08,-2.963536890885939931e-08,1.465352034590808990e-08
-2.825000000000000000e+03,-3.684293196774810145e-08,-1.873896401154824043e-08,-2.888710652839852497e-08,1.800361718905380713e-08
-2.826000000000000000e+03,-3.622155367272623727e-08,-1.615090400902588647e-08,-2.821289568225345943e-08,2.083567504126229125e-08
-2.827000000000000000e+03,-3.562322551531080031e-08,-1.382969473856558947e-08,-2.759617549055167084e-08,2.324182468885404496e-08
-2.828000000000000000e+03,-3.504507902996288641e-08,-1.177156080798522287e-08,-2.702296629684767162e-08,2.527715660592615244e-08
-2.829000000000000000e+03,-3.448772009709979489e-08,-9.952294997592864827e-09,-2.648582795522284848e-08,2.700303717035499061e-08
-2.830000000000000000e+03,-3.394756920386589374e-08,-8.368712507483563918e-09,-2.597926165060079328e-08,2.843151514194931535e-08
-2.831000000000000000e+03,-3.342593432693082517e-08,-7.006805133694309943e-09,-2.549806098333641745e-08,2.960668422648960243e-08
-2.832000000000000000e+03,-3.292005876583127839e-08,-5.886155406189671395e-09,-2.503752553369884339e-08,3.051793861975323117e-08
-2.833000000000000000e+03,-3.243041970741848297e-08,-4.987776162985523311e-09,-2.460086691610003365e-08,3.117163701073261177e-08
-2.834000000000000000e+03,-3.195431042276077698e-08,-4.346569474366703546e-09,-2.418727602687631448e-08,3.152411348043494813e-08
-2.835000000000000000e+03,-3.149292143423222868e-08,-3.985191450775844558e-09,-2.379684026895587355e-08,3.155780648165600924e-08
-2.836000000000000000e+03,-3.104436440224764190e-08,-3.824944402894457975e-09,-2.342569825266144838e-08,3.136052588871296648e-08
-2.837000000000000000e+03,-3.060823476746443938e-08,-3.408827375337575401e-09,-2.307312260763795441e-08,3.139076350290360449e-08
-2.838000000000000000e+03,-3.018423262563230111e-08,-2.408567784572365453e-09,-2.273527711180609618e-08,3.199312376998837572e-08
-2.839000000000000000e+03,-2.977190326861742347e-08,-1.125551064937011431e-09,-2.241294022915752538e-08,3.286052606695265393e-08
-2.840000000000000000e+03,-2.936944560844909367e-08,3.300704086603838621e-11,-2.210307300269125486e-08,3.359147153159963868e-08
-2.841000000000000000e+03,-2.897867624003905581e-08,1.016369709094032117e-09,-2.180564671171713420e-08,3.414374560589741679e-08
-2.842000000000000000e+03,-2.859706098513669018e-08,1.891458610766759838e-09,-2.151841905033168611e-08,3.458292199974014716e-08
-2.843000000000000000e+03,-2.822482731113166645e-08,2.742202290216540962e-09,-2.124287866167863110e-08,3.498710473894785160e-08
-2.844000000000000000e+03,-2.786179897924601897e-08,3.575463294460526321e-09,-2.097680668641653572e-08,3.537258985452845415e-08
-2.845000000000000000e+03,-2.750738876894596983e-08,4.343098389653872568e-09,-2.071934026316601730e-08,3.569250711142640243e-08
-2.846000000000000000e+03,-2.716145752075362349e-08,4.995625976568620650e-09,-2.047060643854325032e-08,3.589614548436582090e-08
-2.847000000000000000e+03,-2.682337874607412687e-08,5.545084962633863646e-09,-2.022971564973648608e-08,3.599675884279953973e-08
-2.848000000000000000e+03,-2.649304825957093039e-08,6.036489384620660924e-09,-1.999681746789917189e-08,3.603818929375854240e-08
-2.849000000000000000e+03,-2.617057841611685769e-08,6.518512673291395669e-09,-1.977022098015151201e-08,3.607743834311602029e-08
-2.850000000000000000e+03,-2.585512237916615417e-08,7.046844176779256114e-09,-1.955087288059738191e-08,3.616191223299280510e-08
-2.851000000000000000e+03,-2.554598153303656298e-08,7.575682221646847538e-09,-1.933705801388174669e-08,3.625050399972803513e-08
-2.852000000000000000e+03,-2.524389281799482437e-08,8.066577353931034058e-09,-1.912974373331605833e-08,3.630370006721701655e-08
-2.853000000000000000e+03,-2.494812481032458340e-08,8.537668544157909021e-09,-1.892796974756858723e-08,3.634069639083366435e-08
-2.854000000000000000e+03,-2.465866810136306567e-08,8.994314849269266609e-09,-1.873194556986048765e-08,3.636584097528423551e-08
-2.855000000000000000e+03,-2.437553742952227207e-08,9.420743795121060291e-09,-1.854068987934596761e-08,3.636796147100484902e-08
-2.856000000000000000e+03,-2.409719555970448554e-08,9.805407500965774708e-09,-1.835365121301834195e-08,3.633095738213905881e-08
-2.857000000000000000e+03,-2.382518452189348642e-08,1.014984464980788648e-08,-1.817216474202683348e-08,3.625732273285405252e-08
-2.858000000000000000e+03,-2.355877199249001019e-08,1.046248172794172038e-08,-1.799413773657696194e-08,3.616176680630469942e-08
-2.859000000000000000e+03,-2.329713670765705773e-08,1.075820040854332201e-08,-1.782088868770132032e-08,3.604928919395912011e-08
-2.860000000000000000e+03,-2.304035032261925121e-08,1.103931240048974629e-08,-1.765189870540518257e-08,3.592492893397539604e-08
-2.861000000000000000e+03,-2.278990397393595920e-08,1.130974309573424532e-08,-1.748613065837053311e-08,3.580428777904254864e-08
-2.862000000000000000e+03,-2.254277416933874362e-08,1.156566422671998483e-08,-1.732464090620086116e-08,3.566469538294915489e-08
-2.863000000000000000e+03,-2.230042742130120947e-08,1.180272528715682984e-08,-1.716637553487613682e-08,3.551344138608868840e-08
-2.864000000000000000e+03,-2.206298389316904350e-08,1.202490212604106715e-08,-1.701084426952873510e-08,3.535732083903375967e-08
-2.865000000000000000e+03,-2.183032635005128014e-08,1.223716846420560172e-08,-1.685932082976628490e-08,3.519488358378781035e-08
-2.866000000000000000e+03,-2.160103455237598988e-08,1.243462668777607078e-08,-1.671054754222658053e-08,3.502048122301517537e-08
-2.867000000000000000e+03,-2.137653117341920901e-08,1.262188485590736095e-08,-1.656500276906235718e-08,3.484308295078891411e-08
-2.868000000000000000e+03,-2.115541635081631085e-08,1.279914386941170190e-08,-1.642222334440288633e-08,3.465856369983030993e-08
-2.869000000000000000e+03,-2.093909249619280971e-08,1.296953126665844309e-08,-1.628267436033194134e-08,3.447437985403663908e-08
-2.870000000000000000e+03,-2.072539621126506756e-08,1.312705120234895517e-08,-1.614512212919271014e-08,3.428024186301724046e-08
-2.871000000000000000e+03,-2.051649324645842533e-08,1.327967783799916062e-08,-1.601080195856852819e-08,3.408842097498712942e-08
-2.872000000000000000e+03,-2.031023809390362199e-08,1.342085560601617575e-08,-1.587849163217543275e-08,3.388809756247635783e-08
-2.873000000000000000e+03,-2.010877877698707823e-08,1.355617944522073659e-08,-1.574863077583373878e-08,3.369275649813766520e-08
-2.874000000000000000e+03,-1.990920241597537040e-08,1.368214888808156402e-08,-1.562079208864436160e-08,3.348741810554465447e-08
-2.875000000000000000e+03,-1.971363948956809403e-08,1.380651770606652369e-08,-1.549618841589938324e-08,3.328407408474288613e-08
-2.876000000000000000e+03,-1.952154706088268236e-08,1.392067979002484690e-08,-1.537283403948542165e-08,3.308078155806290256e-08
-2.877000000000000000e+03,-1.933268475693894658e-08,1.403092810854484549e-08,-1.525193063739482469e-08,3.287717363518115573e-08
-2.878000000000000000e+03,-1.914652604161773015e-08,1.413533100398518097e-08,-1.513307283408386858e-08,3.267075909963802857e-08
-2.879000000000000000e+03,-1.896359817030886269e-08,1.423418306927853098e-08,-1.501588063955327740e-08,3.246602249770693282e-08
-2.880000000000000000e+03,-1.878339093958932143e-08,1.432792418071512110e-08,-1.490074490861563563e-08,3.225924232661815002e-08
-2.881000000000000000e+03,-1.860641541064259647e-08,1.441674918736206704e-08,-1.478727457367578782e-08,3.205477975861356401e-08
-2.882000000000000000e+03,-1.843139007475894592e-08,1.450119597699091071e-08,-1.467587128173878413e-08,3.184539932268564155e-08
-2.883000000000000000e+03,-1.826038447450620538e-08,1.458204390749247650e-08,-1.456613331130633873e-08,3.164329347537976989e-08
-2.884000000000000000e+03,-1.809134437012107849e-08,1.466060566327579777e-08,-1.445847273047920638e-08,3.143838469179839360e-08
-2.885000000000000000e+03,-1.792474998724416333e-08,1.473485022548321897e-08,-1.435247749120262159e-08,3.123276276228899765e-08
-2.886000000000000000e+03,-1.776092352003105844e-08,1.480389872615110220e-08,-1.424778129622152270e-08,3.102872849543505548e-08
-2.887000000000000000e+03,-1.759954296991119802e-08,1.486995120334415503e-08,-1.414475006015053265e-08,3.082530492318687113e-08
-2.888000000000000000e+03,-1.744094515257215983e-08,1.492788897764335689e-08,-1.404223746210738277e-08,3.062422297164586830e-08
-2.889000000000000000e+03,-1.728400433151535056e-08,1.498711838456028525e-08,-1.394217848191797643e-08,3.042075359603632167e-08
-2.890000000000000000e+03,-1.712986027160604146e-08,1.504192061503090517e-08,-1.384343560123598336e-08,3.021969521947292753e-08
-2.891000000000000000e+03,-1.697816252307177665e-08,1.509638030210016735e-08,-1.374635734712537207e-08,3.002190437335792701e-08
-2.892000000000000000e+03,-1.682848528262974089e-08,1.514577453182132518e-08,-1.365060349196906418e-08,2.982226292757609071e-08
-2.893000000000000000e+03,-1.668046405001503913e-08,1.519182414682393814e-08,-1.355572355871294434e-08,2.962288879344379385e-08
-2.894000000000000000e+03,-1.653526635039181249e-08,1.523786357683443643e-08,-1.346296660692604328e-08,2.942673984837172145e-08
-2.895000000000000000e+03,-1.639172431828024016e-08,1.527618887889874791e-08,-1.337029157766200932e-08,2.923014483992834981e-08
-2.896000000000000000e+03,-1.625101878394829595e-08,1.531590964296774201e-08,-1.327974771240774172e-08,2.903820275351192033e-08
-2.897000000000000000e+03,-1.611117684614777896e-08,1.535153618122868628e-08,-1.319007588282547595e-08,2.884212746660023728e-08
-2.898000000000000000e+03,-1.597418366051471739e-08,1.538562518181233243e-08,-1.310175147793602488e-08,2.865144825902765172e-08
-2.899000000000000000e+03,-1.583884533624573665e-08,1.541993015812527125e-08,-1.301509064819621954e-08,2.846094478409755677e-08
-2.900000000000000000e+03,-1.570557531088784134e-08,1.544609674319175601e-08,-1.292819913620370915e-08,2.827292035827753489e-08
-2.901000000000000000e+03,-1.557395974151564545e-08,1.547611286088096488e-08,-1.284376371210945749e-08,2.808504326901463011e-08
-2.902000000000000000e+03,-1.544362994958865914e-08,1.550100157024149734e-08,-1.275989666011912617e-08,2.789535198187580013e-08
-2.903000000000000000e+03,-1.531574765835055646e-08,1.552375302006275746e-08,-1.267689910941927361e-08,2.771081114801552188e-08
-2.904000000000000000e+03,-1.518916114395963151e-08,1.554575848553528105e-08,-1.259526978712589786e-08,2.752518972501644897e-08
-2.905000000000000000e+03,-1.506502268439365471e-08,1.556559860377433876e-08,-1.251450912689396502e-08,2.734469710261347259e-08
-2.906000000000000000e+03,-1.494218978628158013e-08,1.558174139111143192e-08,-1.243432871721464558e-08,2.716385687020039157e-08
-2.907000000000000000e+03,-1.482101050751774749e-08,1.559936183294935908e-08,-1.235581083839383877e-08,2.698445313604458955e-08
-2.908000000000000000e+03,-1.470114588929533387e-08,1.561331579363691016e-08,-1.227787911642040899e-08,2.680474738698229443e-08
-2.909000000000000000e+03,-1.458293442463063571e-08,1.562641954197009226e-08,-1.220081428017855708e-08,2.662782266529905201e-08
-2.910000000000000000e+03,-1.446604648686867510e-08,1.563520048926858235e-08,-1.212434096134782801e-08,2.644995579973482351e-08
-2.911000000000000000e+03,-1.435081138595625497e-08,1.564678223005699504e-08,-1.204952976210509196e-08,2.627484685696481809e-08
-2.912000000000000000e+03,-1.423770515442368018e-08,1.565544087750607409e-08,-1.197531578307853937e-08,2.610388847326225280e-08
-2.913000000000000000e+03,-1.412545499621201758e-08,1.566251474016484505e-08,-1.190196716806135459e-08,2.593130239735798463e-08
-2.914000000000000000e+03,-1.401454569525768508e-08,1.566737801356437105e-08,-1.182922090692380995e-08,2.575991638021942838e-08
-2.915000000000000000e+03,-1.390608632354652493e-08,1.567131776640229643e-08,-1.175733903428160170e-08,2.559492938373368770e-08
-2.916000000000000000e+03,-1.379738072189449638e-08,1.567238774739839455e-08,-1.168606456547148637e-08,2.542313025788987507e-08
-2.917000000000000000e+03,-1.369112530343678180e-08,1.567688297521447704e-08,-1.161645175524002093e-08,2.525839804118515535e-08
-2.918000000000000000e+03,-1.358622697216572933e-08,1.567484869201524820e-08,-1.154665328715570928e-08,2.509426121022386316e-08
-2.919000000000000000e+03,-1.348218229084065532e-08,1.567690721165664132e-08,-1.147851633730009283e-08,2.493048618445832023e-08
-2.920000000000000000e+03,-1.337950226537922056e-08,1.567314542859978372e-08,-1.141019789358510630e-08,2.476803147668550642e-08
-2.921000000000000000e+03,-1.327847428855801475e-08,1.567208435622586015e-08,-1.134354086081528948e-08,2.460823424143609369e-08
-2.922000000000000000e+03,-1.317801897264323468e-08,1.566659882349811845e-08,-1.127670638853361710e-08,2.444747675275108963e-08
-2.923000000000000000e+03,-1.307921548001130463e-08,1.566010153910242587e-08,-1.121073325234033758e-08,2.428935823854240952e-08
-2.924000000000000000e+03,-1.298179154735118133e-08,1.565659204321853412e-08,-1.114618689821053970e-08,2.413400942591649431e-08
-2.925000000000000000e+03,-1.288521899623507212e-08,1.564904284905459671e-08,-1.108170099216276997e-08,2.397827370216289294e-08
-2.926000000000000000e+03,-1.279003306632254872e-08,1.564012201831542876e-08,-1.101784619484983659e-08,2.382465554335597793e-08
-2.927000000000000000e+03,-1.269569771703833533e-08,1.563152556839559098e-08,-1.095485133919418985e-08,2.367131853310168821e-08
-2.928000000000000000e+03,-1.260275588911418439e-08,1.562158104697759667e-08,-1.089249209650303827e-08,2.352013371803797965e-08
-2.929000000000000000e+03,-1.251066392645993357e-08,1.561263158917772533e-08,-1.083099223647791592e-08,2.336990001217146777e-08
-2.930000000000000000e+03,-1.241997226210623325e-08,1.560166843834811291e-08,-1.077013245039629217e-08,2.322116357582493107e-08
-2.931000000000000000e+03,-1.233012982327986369e-08,1.559237204712699186e-08,-1.071013151117357244e-08,2.307404946465841344e-08
-2.932000000000000000e+03,-1.224169434826377011e-08,1.557806609865702115e-08,-1.064997218104003815e-08,2.292915511184151847e-08
-2.933000000000000000e+03,-1.215410750134406463e-08,1.556402939886614950e-08,-1.059067071651984198e-08,2.278448734585557011e-08
-2.934000000000000000e+03,-1.206713063988909600e-08,1.555008971032214276e-08,-1.053201745697205992e-08,2.263974008103906931e-08
-2.935000000000000000e+03,-1.198180525150858651e-08,1.553640301488287549e-08,-1.047422157895247486e-08,2.249891318153672054e-08
-2.936000000000000000e+03,-1.189709556974318370e-08,1.551843234483544663e-08,-1.041627411951134947e-08,2.235734589233840736e-08
-2.937000000000000000e+03,-1.181323310752799820e-08,1.550579203799968130e-08,-1.035998752512854506e-08,2.221735128760703531e-08
-2.938000000000000000e+03,-1.172999154008533338e-08,1.548888676513216094e-08,-1.030355283145775698e-08,2.207664318072735861e-08
-2.939000000000000000e+03,-1.164840136593434992e-08,1.546917439075875185e-08,-1.024716933273774904e-08,2.194051820707304904e-08
-2.940000000000000000e+03,-1.156743762325272115e-08,1.545264894289820700e-08,-1.019225083507820696e-08,2.180370737369104475e-08
-2.941000000000000000e+03,-1.148731993525672565e-08,1.543398962568383337e-08,-1.013738247458107517e-08,2.166843847611822537e-08
-2.942000000000000000e+03,-1.140863966309088417e-08,1.541481973586060872e-08,-1.008317799340524849e-08,2.153623144831914276e-08
-2.943000000000000000e+03,-1.132999881447137012e-08,1.539722030253124670e-08,-1.002982839711490755e-08,2.140182881217270753e-08
-2.944000000000000000e+03,-1.125280097691946326e-08,1.537609813557415097e-08,-9.976340178843177035e-09,2.127120793659281341e-08
-2.945000000000000000e+03,-1.117644806089312660e-08,1.535583904057195864e-08,-9.923706062742430959e-09,2.114140773377087251e-08
-2.946000000000000000e+03,-1.110073687396391958e-08,1.533207248407547572e-08,-9.870936166680990250e-09,2.101169085835634534e-08
-2.947000000000000000e+03,-1.102586992546921745e-08,1.531426743526535307e-08,-9.819827070892744157e-09,2.088416434332330469e-08
-2.948000000000000000e+03,-1.095164942095613954e-08,1.529228025368478495e-08,-9.768585467544493213e-09,2.075605314627938158e-08
-2.949000000000000000e+03,-1.087827248483710510e-08,1.526808869193124516e-08,-9.717388966324860367e-09,2.062942514514331292e-08
-2.950000000000000000e+03,-1.080554664666061018e-08,1.524484672828260973e-08,-9.666870618585409904e-09,2.050362179086775866e-08
-2.951000000000000000e+03,-1.073366376609930365e-08,1.522242450660816418e-08,-9.617204654611663514e-09,2.037859464554731062e-08
-2.952000000000000000e+03,-1.066324566659676587e-08,1.520097228535615794e-08,-9.568220743219120859e-09,2.025815239452350592e-08
-2.953000000000000000e+03,-1.059286101157819393e-08,1.517797741744419826e-08,-9.519279715669122428e-09,2.013612390282153349e-08
-2.954000000000000000e+03,-1.052313670326769419e-08,1.515084443833247058e-08,-9.470214534707451604e-09,2.001358037581195014e-08
-2.955000000000000000e+03,-1.045506409962227185e-08,1.512963018055216826e-08,-9.422810175790572604e-09,1.989691346311839213e-08
-2.956000000000000000e+03,-1.038684648281482118e-08,1.510194090458223767e-08,-9.374474612659894234e-09,1.977740241739966633e-08
-2.957000000000000000e+03,-1.031947010213154080e-08,1.507946597767815584e-08,-9.327799860621744294e-09,1.965932065783228340e-08
-2.958000000000000000e+03,-1.025276291118194639e-08,1.505052766160521103e-08,-9.280195894784340656e-09,1.954215745482220683e-08
-2.959000000000000000e+03,-1.018689639854813811e-08,1.502748829259477274e-08,-9.234252737934840037e-09,1.942710556954000677e-08
-2.960000000000000000e+03,-1.012170349385195465e-08,1.500104960708133016e-08,-9.188193758610864819e-09,1.931230021333550562e-08
-2.961000000000000000e+03,-1.005735075293703261e-08,1.497300436000299758e-08,-9.142172618567310116e-09,1.919959369022893337e-08
-2.962000000000000000e+03,-9.993675977872689624e-09,1.494976782864625752e-08,-9.097661881681987293e-09,1.908785141747654050e-08
-2.963000000000000000e+03,-9.930028415238724280e-09,1.492115950236173428e-08,-9.052375772596865805e-09,1.897444394582079579e-08
-2.964000000000000000e+03,-9.867875424559916585e-09,1.489362770156313280e-08,-9.007791364035574980e-09,1.886577473697405452e-08
-2.965000000000000000e+03,-9.805748423293398897e-09,1.486821209531986765e-08,-8.964055018449688899e-09,1.875542512044747101e-08
-2.966000000000000000e+03,-9.744307652544290833e-09,1.483944032463778742e-08,-8.920210826234960395e-09,1.864538664518759310e-08
-2.967000000000000000e+03,-9.683704808966195555e-09,1.480971106787245273e-08,-8.876400482213161581e-09,1.853810418125200147e-08
-2.968000000000000000e+03,-9.622978567172476465e-09,1.478554903966158423e-08,-8.834112147851070870e-09,1.842878991885244206e-08
-2.969000000000000000e+03,-9.563903449418020839e-09,1.475526259072128323e-08,-8.791042582851109372e-09,1.832458463820502097e-08
-2.970000000000000000e+03,-9.504708610519680522e-09,1.472610573016247227e-08,-8.748684520617023279e-09,1.821767008443651783e-08
-2.971000000000000000e+03,-9.446350063130164363e-09,1.469972307309139812e-08,-8.707172238177932333e-09,1.811348591417407316e-08
-2.972000000000000000e+03,-9.388690224292351784e-09,1.467072632374190826e-08,-8.665560157035539260e-09,1.801037541701718410e-08
-2.973000000000000000e+03,-9.331865956635239113e-09,1.464072526522740194e-08,-8.623977661168450674e-09,1.790998291491141524e-08
-2.974000000000000000e+03,-9.274929050058309667e-09,1.461189079186269544e-08,-8.583113283678918736e-09,1.780692029142014319e-08
-2.975000000000000000e+03,-9.218826444814010801e-09,1.458133701408878824e-08,-8.542276916344791366e-09,1.770586207758007740e-08
-2.976000000000000000e+03,-9.163430918429765141e-09,1.455266750098687237e-08,-8.502162150697746901e-09,1.760662105728839681e-08
-2.977000000000000000e+03,-9.108052097238437304e-09,1.452603241505262176e-08,-8.462890336886805043e-09,1.750559858929251339e-08
-2.978000000000000000e+03,-9.054201465947688247e-09,1.449375878247389553e-08,-8.422710335348189381e-09,1.741018955642625212e-08
-2.979000000000000000e+03,-8.999548492852935700e-09,1.446350162947572380e-08,-8.383371647855502706e-09,1.730920606754342878e-08
-2.980000000000000000e+03,-8.946428661744733516e-09,1.443586980411738336e-08,-8.344761707538358066e-09,1.721456286232681034e-08
-2.981000000000000000e+03,-8.893321238891370974e-09,1.440576319329661009e-08,-8.306174363958644931e-09,1.711739781793200655e-08
-2.982000000000000000e+03,-8.840934430494218576e-09,1.437452700515838543e-08,-8.267501558138237050e-09,1.702282591974048207e-08
-2.983000000000000000e+03,-8.789375713325372579e-09,1.434527084452863689e-08,-8.229666972712542076e-09,1.693018726928304025e-08
-2.984000000000000000e+03,-8.737724148279723206e-09,1.431420767195140064e-08,-8.191750435997017274e-09,1.683569128290674464e-08
-2.985000000000000000e+03,-8.686898000411369369e-09,1.428283250896189557e-08,-8.154178638415606469e-09,1.674310323315999613e-08
-2.986000000000000000e+03,-8.635983687869363367e-09,1.425264527039221949e-08,-8.117020134086930783e-09,1.664938721255365370e-08
-2.987000000000000000e+03,-8.585891369518763395e-09,1.422173914070759391e-08,-8.080121337957962572e-09,1.655754911983818194e-08
-2.988000000000000000e+03,-8.536536329794041499e-09,1.419129572674113896e-08,-8.043476733179990536e-09,1.646840479649580712e-08
-2.989000000000000000e+03,-8.487178875832911839e-09,1.416047577867220194e-08,-8.007169638935824509e-09,1.637731405625664198e-08
-2.990000000000000000e+03,-8.438565987407097599e-09,1.412945537914522818e-08,-7.971122390907270071e-09,1.628826145552646461e-08
-2.991000000000000000e+03,-8.390764381831694020e-09,1.409833269322554804e-08,-7.935324858072799446e-09,1.620170006990377832e-08
-2.992000000000000000e+03,-8.342895862977535432e-09,1.406705953935469452e-08,-7.899794390445374294e-09,1.611344579540485942e-08
-2.993000000000000000e+03,-8.295828410912219776e-09,1.403669506014534850e-08,-7.864586966092765204e-09,1.602830786313303345e-08
-2.994000000000000000e+03,-8.248706317369201992e-09,1.400517158186230527e-08,-7.829574716477958648e-09,1.594085719951254684e-08
-2.995000000000000000e+03,-8.202038111031107100e-09,1.397373428964778791e-08,-7.794870152015720488e-09,1.585416793043784091e-08
-2.996000000000000000e+03,-8.155993467485290316e-09,1.394196275062294202e-08,-7.760377605027273818e-09,1.576904506425880945e-08
-2.997000000000000000e+03,-8.110277664427721791e-09,1.391071061869086230e-08,-7.726157523588461119e-09,1.568470196291612544e-08
-2.998000000000000000e+03,-8.064984339148714411e-09,1.387939891849993527e-08,-7.692186372475823381e-09,1.560110079171472166e-08
-2.999000000000000000e+03,-8.019888394911203906e-09,1.384658500967513780e-08,-7.658313334649377023e-09,1.551645586255661030e-08
+9.989963699999999562e+02,-3.140795719171814891e-10,-6.471473538165549602e-10,-3.542532444717689462e-10,-8.251355643851374176e-10
+1.000924939999999992e+03,-3.155521198927451197e-10,-6.496810668983020223e-10,-3.560381774949187236e-10,-8.290532897339401689e-10
+1.002853500000000054e+03,-3.171054308461795192e-10,-6.524317835270207479e-10,-3.578933220474298476e-10,-8.331412707642677895e-10
+1.004782069999999976e+03,-3.185921934068372566e-10,-6.549752277751699389e-10,-3.596985584590018665e-10,-8.370957035338200173e-10
+1.006710630000000037e+03,-3.201614270167343153e-10,-6.577447951539702656e-10,-3.615739001362251447e-10,-8.412214732132686507e-10
+1.008639199999999960e+03,-3.216624160374660111e-10,-6.603082263457491553e-10,-3.633990629670175063e-10,-8.452211464187073288e-10
+1.010567760000000021e+03,-3.232477800410561595e-10,-6.630967538566189845e-10,-3.652948853572483289e-10,-8.493851501850545771e-10
+1.012496329999999944e+03,-3.247631492265808483e-10,-6.656818296951426938e-10,-3.671401581323318235e-10,-8.534318536476378780e-10
+1.014424890000000005e+03,-3.263648536172164542e-10,-6.684894570379786278e-10,-3.690567481275367488e-10,-8.576345718977080974e-10
+1.016353449999999953e+03,-3.278947666460265749e-10,-6.710968724772287150e-10,-3.709223708054802611e-10,-8.617293385279315329e-10
+1.018282019999999989e+03,-3.295130325202578056e-10,-6.739237666501744566e-10,-3.728600295107471956e-10,-8.659712927352132298e-10
+1.020210580000000050e+03,-3.310576760798678242e-10,-6.765539945359633780e-10,-3.747462829810755339e-10,-8.701150127379752635e-10
+1.022139149999999972e+03,-3.326927117892080963e-10,-6.794002962560283913e-10,-3.767052969485027883e-10,-8.743966900847444875e-10
+1.024067710000000034e+03,-3.342522690637141494e-10,-6.820536980640128081e-10,-3.786124637986512358e-10,-8.785901653391144521e-10
+1.025996280000000070e+03,-3.359042943890665807e-10,-6.849195680577073325e-10,-3.805931342937484702e-10,-8.829120875669036582e-10
+1.027924839999999904e+03,-3.374789522649444218e-10,-6.875964627193499898e-10,-3.825215051477386682e-10,-8.871560966103227923e-10
+1.029853409999999940e+03,-3.391481905382210036e-10,-6.904820647745972893e-10,-3.845241386616725042e-10,-8.915187959415538905e-10
+1.031781970000000001e+03,-3.407381393238536137e-10,-6.931827503331713178e-10,-3.864740108874731214e-10,-8.958141111414722686e-10
+1.033710530000000063e+03,-3.424248090831306393e-10,-6.960882340400966225e-10,-3.884989090253587335e-10,-9.002181051922124297e-10
+1.035639100000000099e+03,-3.440302508469767787e-10,-6.988130146740577294e-10,-3.904705964360155911e-10,-9.045655258080120774e-10
+1.037567659999999933e+03,-3.457345911434678326e-10,-7.017385654086276527e-10,-3.925180866866904468e-10,-9.090113917743760699e-10
+1.039496229999999969e+03,-3.473557144724253601e-10,-7.044877065564261700e-10,-3.945118886695225929e-10,-9.134116741423396108e-10
+1.041424790000000030e+03,-3.490779598159192360e-10,-7.074334952224652253e-10,-3.965822940078557164e-10,-9.178999748699474554e-10
+1.043353360000000066e+03,-3.507149649717940328e-10,-7.102072767158817812e-10,-3.985985259726827618e-10,-9.223539089815580348e-10
+1.045281919999999900e+03,-3.524553537645060063e-10,-7.131734763124524267e-10,-4.006921751253343644e-10,-9.268852176491267440e-10
+1.047210489999999936e+03,-3.541084443716314008e-10,-7.159721775552155375e-10,-4.027311583692342173e-10,-9.313936042535584788e-10
+1.049139049999999997e+03,-3.558672189913048440e-10,-7.189589631222887472e-10,-4.048483859434917658e-10,-9.359685045211923797e-10
+1.051067610000000059e+03,-3.575365932595137306e-10,-7.217828468230254412e-10,-4.069104369212555663e-10,-9.405321302076951613e-10
+1.052996180000000095e+03,-3.593140089718982499e-10,-7.247904128417397062e-10,-4.090515943148064602e-10,-9.451512424661022331e-10
+1.054924739999999929e+03,-3.609998861486816239e-10,-7.276397779560895777e-10,-4.111370569304879181e-10,-9.497709584773510074e-10
+1.056853309999999965e+03,-3.627961847995754220e-10,-7.306682861803909031e-10,-4.133024802501971588e-10,-9.544348621012125876e-10
+1.058781870000000026e+03,-3.644987789304027626e-10,-7.335434164351788820e-10,-4.154116938599511609e-10,-9.591115073491370985e-10
+1.060710440000000062e+03,-3.663142153374502014e-10,-7.365930478948567504e-10,-4.176017361519552028e-10,-9.638208185665295198e-10
+1.062638999999999896e+03,-3.680337440725161947e-10,-7.394942294763076336e-10,-4.197350463314854825e-10,-9.685552460073579490e-10
+1.064567559999999958e+03,-3.698685682243956812e-10,-7.425651492276480780e-10,-4.219500558471262767e-10,-9.733105652242513075e-10
+1.066496129999999994e+03,-3.716052620421545604e-10,-7.454926890329934659e-10,-4.241078257260112290e-10,-9.781036694619059574e-10
+1.068424690000000055e+03,-3.734597465500208923e-10,-7.485850999000168040e-10,-4.263481795802896842e-10,-9.829056625033708986e-10
+1.070353260000000091e+03,-3.752138214714573720e-10,-7.515392720459684073e-10,-4.285307564523870569e-10,-9.877582992549584068e-10
+1.072281819999999925e+03,-3.770882343964876638e-10,-7.546533610455635843e-10,-4.307968273807478352e-10,-9.926076168939797038e-10
+1.074210389999999961e+03,-3.788599193290125711e-10,-7.576344606285195541e-10,-4.330045762275888283e-10,-9.975206841280682294e-10
+1.076138950000000023e+03,-3.807545333362791658e-10,-7.607704167979427583e-10,-4.352967438236084063e-10,-1.002417989145325226e-09
+1.078067520000000059e+03,-3.825440610955474158e-10,-7.637787422396510600e-10,-4.375300363655126385e-10,-1.007392400696472544e-09
+1.079996079999999893e+03,-3.844591535524130350e-10,-7.669367566525507958e-10,-4.398486872343517542e-10,-1.012338368140289553e-09
+1.081924639999999954e+03,-3.862667513572610574e-10,-7.699725911699493050e-10,-4.421078902680624007e-10,-1.017375025621022515e-09
+1.083853209999999990e+03,-3.882026140218309356e-10,-7.731528756124276192e-10,-4.444534299912516635e-10,-1.022370371568658749e-09
+1.085781770000000051e+03,-3.900285322401425795e-10,-7.762165431661863338e-10,-4.467389408235321600e-10,-1.027470249947796059e-09
+1.087710340000000087e+03,-3.919854427030948359e-10,-7.794192743374567217e-10,-4.491117588359621760e-10,-1.032515646620781213e-09
+1.089638899999999921e+03,-3.938299263773271682e-10,-7.825110840625427640e-10,-4.514239702897845630e-10,-1.037679709770278532e-09
+1.091567469999999958e+03,-3.958081767301974936e-10,-7.857364592583256331e-10,-4.538244751946282259e-10,-1.042775870665528426e-09
+1.093496030000000019e+03,-3.976714751547810411e-10,-7.888567240692809769e-10,-4.561637874402807364e-10,-1.048005099950738160e-09
+1.095424600000000055e+03,-3.996713626108506251e-10,-7.921049427017755403e-10,-4.585923955071533607e-10,-1.053152751955847957e-09
+1.097353159999999889e+03,-4.015537294242879742e-10,-7.952539793845905139e-10,-4.609592162264773376e-10,-1.058448146646996534e-09
+1.099281719999999950e+03,-4.035755463770389186e-10,-7.985252236008926085e-10,-4.634163391241405011e-10,-1.063648000354490863e-09
+1.101210289999999986e+03,-4.054772497101430734e-10,-8.017033722986346799e-10,-4.658110961219088749e-10,-1.069010608025174365e-09
+1.103138850000000048e+03,-4.075213139006199632e-10,-8.049978650519210034e-10,-4.682971782765577958e-10,-1.074263447662858703e-09
+1.105067420000000084e+03,-4.094426064206141574e-10,-8.082054313156985464e-10,-4.707202824746946539e-10,-1.079694275006729878e-09
+1.106995979999999918e+03,-4.115092311082955049e-10,-8.115233785077104103e-10,-4.732357642198271992e-10,-1.085000869473851738e-09
+1.108924549999999954e+03,-4.134503800661443513e-10,-8.147606912483180730e-10,-4.756876468713072205e-10,-1.090500972007524216e-09
+1.110853110000000015e+03,-4.155398840972778405e-10,-8.181023009964490699e-10,-4.782329769339791146e-10,-1.095862104854368181e-09
+1.112781680000000051e+03,-4.175011614827798261e-10,-8.213696933293255467e-10,-4.807140775093417690e-10,-1.101432557711512832e-09
+1.114710240000000113e+03,-4.196138694144840133e-10,-8.247351759936465750e-10,-4.832897132043956846e-10,-1.106849027477129716e-09
+1.116638799999999947e+03,-4.215955415162452311e-10,-8.280329651377029876e-10,-4.858004664617637182e-10,-1.112490894275626261e-09
+1.118567369999999983e+03,-4.237317942898860484e-10,-8.314225535236908668e-10,-4.884068870109114843e-10,-1.117963546412278865e-09
+1.120495930000000044e+03,-4.257341533265004916e-10,-8.347511012511385693e-10,-4.909477623905504139e-10,-1.123677974099459393e-09
+1.122424500000000080e+03,-4.278942768753634389e-10,-8.381649902826666685e-10,-4.935854299264043550e-10,-1.129207606957912784e-09
+1.124353059999999914e+03,-4.299176096967847490e-10,-8.415246428020405099e-10,-4.961568927054297188e-10,-1.134995732258319822e-09
+1.126281629999999950e+03,-4.321019464913054353e-10,-8.449630497329844298e-10,-4.988262915282405207e-10,-1.140583191465050549e-09
+1.128210190000000011e+03,-4.341465451264576245e-10,-8.483541577801553547e-10,-5.014288159902429221e-10,-1.146446172588205336e-09
+1.130138760000000048e+03,-4.363554438792711926e-10,-8.518173022201148469e-10,-5.041304398199580299e-10,-1.152092320203211904e-09
+1.132067320000000109e+03,-4.384216056538937050e-10,-8.552402211390562242e-10,-5.067645094663110779e-10,-1.158031337338460926e-09
+1.133995879999999943e+03,-4.406554103883173342e-10,-8.587283040821866434e-10,-5.094988478183160911e-10,-1.163737018953997149e-09
+1.135924449999999979e+03,-4.427434491199255579e-10,-8.621834149025129674e-10,-5.121649694325522694e-10,-1.169753308060910675e-09
+1.137853010000000040e+03,-4.450025324148516558e-10,-8.656966815808614871e-10,-5.149325492179821930e-10,-1.175519452673240656e-09
+1.139781580000000076e+03,-4.471127454378071003e-10,-8.691843282955060939e-10,-5.176312117166759597e-10,-1.181614206543805675e-09
+1.141710139999999910e+03,-4.493974755988697582e-10,-8.727230055706411001e-10,-5.204325562720569974e-10,-1.187441727874056324e-09
+1.143638709999999946e+03,-4.515301768721028677e-10,-8.762435578441293057e-10,-5.231642721410033432e-10,-1.193616195739915091e-09
+1.145567270000000008e+03,-4.538409290393984768e-10,-8.798078750623188873e-10,-5.259999151505725938e-10,-1.199506025559253608e-09
+1.147495840000000044e+03,-4.559964383244345578e-10,-8.833617075021729458e-10,-5.287652069999993335e-10,-1.205761480742817659e-09
+1.149424400000000105e+03,-4.583335946312760700e-10,-8.869518965278023712e-10,-5.316356927444094632e-10,-1.211714569304391392e-09
+1.151352959999999939e+03,-4.605122259956352525e-10,-8.905393669064049900e-10,-5.344350789272786501e-10,-1.218052274658356673e-09
+1.153281529999999975e+03,-4.628761873640862459e-10,-8.941556840150181952e-10,-5.373409771643010411e-10,-1.224069626259077229e-09
+1.155210090000000037e+03,-4.650782840875621113e-10,-8.977771987618735904e-10,-5.401750157191021378e-10,-1.230490939694692193e-09
+1.157138660000000073e+03,-4.674694356289064595e-10,-9.014198592905460817e-10,-5.431168782527852078e-10,-1.236573508198758716e-09
+1.159067219999999907e+03,-4.696953357082393229e-10,-9.050758083716095469e-10,-5.459861236457954245e-10,-1.243079778743550353e-09
+1.160995789999999943e+03,-4.721140815351827114e-10,-9.087450519492115783e-10,-5.489645281128148857e-10,-1.249228572572402330e-09
+1.162924350000000004e+03,-4.743641293359868606e-10,-9.124358306359047523e-10,-5.518695459489201102e-10,-1.255821175691524309e-09
+1.164852920000000040e+03,-4.768108812357877986e-10,-9.161318995525769780e-10,-5.548850816501244442e-10,-1.262037223603759515e-09
+1.166781480000000101e+03,-4.790854276446603412e-10,-9.198579085166674258e-10,-5.578264489449119293e-10,-1.268717561826457420e-09
+1.168710039999999935e+03,-4.815605930291225628e-10,-9.235810249854469415e-10,-5.608797016694198810e-10,-1.275001876330276431e-09
+1.170638609999999971e+03,-4.838600078434085853e-10,-9.273426931645367157e-10,-5.638580225920663242e-10,-1.281771416971286384e-09
+1.172567170000000033e+03,-4.863640264969683014e-10,-9.310931274870599604e-10,-5.669496211046255248e-10,-1.288125105639732995e-09
+1.174495740000000069e+03,-4.886886620253121511e-10,-9.348908440778981428e-10,-5.699654810723265203e-10,-1.294985270676013266e-09
+1.176424299999999903e+03,-4.912219698753550205e-10,-9.386688467608507511e-10,-5.730960514154283456e-10,-1.301409426314855881e-09
+1.178352869999999939e+03,-4.935721975278479660e-10,-9.425030292255879854e-10,-5.761500633923903002e-10,-1.308361703406571860e-09
+1.180281430000000000e+03,-4.961352389403195942e-10,-9.463088535997076925e-10,-5.793202444694440563e-10,-1.314857441238748584e-09
+1.182210000000000036e+03,-4.985114373030898736e-10,-9.501799252017304271e-10,-5.824130340009178492e-10,-1.321903347794023238e-09
+1.184138560000000098e+03,-5.011046652878544636e-10,-9.540138274646124243e-10,-5.856234778977486832e-10,-1.328471806017002165e-09
+1.186067119999999932e+03,-5.035072074294416700e-10,-9.579221936363767268e-10,-5.887556670639465971e-10,-1.335612850706785696e-09
+1.187995689999999968e+03,-5.061310967219508832e-10,-9.617844566270364048e-10,-5.920070557408102572e-10,-1.342255230262650653e-09
+1.189924250000000029e+03,-5.085603888361916505e-10,-9.657305760815788839e-10,-5.951793123526822289e-10,-1.349493030886487513e-09
+1.191852820000000065e+03,-5.112153976533088686e-10,-9.696214383458670888e-10,-5.984723091119233376e-10,-1.356210478945955469e-09
+1.193781379999999899e+03,-5.136718409311679407e-10,-9.736057524000432486e-10,-6.016852983782845626e-10,-1.363546646543602317e-09
+1.195709949999999935e+03,-5.163584495116859046e-10,-9.775254790057491291e-10,-6.050205968828346199e-10,-1.370340373743490482e-09
+1.197638509999999997e+03,-5.188424530579502341e-10,-9.815484352242384736e-10,-6.082749979081949072e-10,-1.377776552105025879e-09
+1.199567080000000033e+03,-5.215611511698919428e-10,-9.854972942897399243e-10,-6.116533063883369324e-10,-1.384647794453980943e-09
+1.201495640000000094e+03,-5.240731322020155012e-10,-9.895593466035364784e-10,-6.149498125265558823e-10,-1.392185660924183286e-09
+1.203424199999999928e+03,-5.268244058242087848e-10,-9.935375845945499360e-10,-6.183718368224076313e-10,-1.399135638976550320e-09
+1.205352769999999964e+03,-5.293648034346169612e-10,-9.976392181672077687e-10,-6.217111733717821065e-10,-1.406776946745210796e-09
+1.207281330000000025e+03,-5.321491755140638132e-10,-1.001647133983647014e-09,-6.251776690819624560e-10,-1.413806990156676831e-09
+1.209209900000000061e+03,-5.347184103692315465e-10,-1.005788791324480651e-09,-6.285605418946228395e-10,-1.421553445239315614e-09
+1.211138459999999895e+03,-5.375364007191987771e-10,-1.009826662543770456e-09,-6.320722632288077111e-10,-1.428664870073330066e-09
+1.213067029999999932e+03,-5.401349156339995602e-10,-1.014008817423790249e-09,-6.354994106420151837e-10,-1.436518255543731356e-09
+1.214995589999999993e+03,-5.429870545956082685e-10,-1.018076924889377121e-09,-6.390571279367951400e-10,-1.443712405936224144e-09
+1.216924150000000054e+03,-5.456152872382925352e-10,-1.022300032364905654e-09,-6.425292859294454404e-10,-1.451674498506775626e-09
+1.218852720000000090e+03,-5.485021300699744080e-10,-1.026398685818348729e-09,-6.461338042029122328e-10,-1.458952790751736605e-09
+1.220781279999999924e+03,-5.511605553854728639e-10,-1.030663258890710764e-09,-6.496517609682483126e-10,-1.467025491260696686e-09
+1.222709849999999960e+03,-5.540826403491503386e-10,-1.034792720533647527e-09,-6.533038661902964196e-10,-1.474389285022253157e-09
+1.224638410000000022e+03,-5.567717287728676195e-10,-1.039099254001364233e-09,-6.568684086332757131e-10,-1.482574490376683290e-09
+1.226566980000000058e+03,-5.597296194477598017e-10,-1.043259814820018399e-09,-6.605689221002875434e-10,-1.490025218448958471e-09
+1.228495539999999892e+03,-5.624498511076904936e-10,-1.047608810777716595e-09,-6.641808541729622409e-10,-1.498324865435932777e-09
+1.230424109999999928e+03,-5.654441227315185213e-10,-1.051800765263273415e-09,-6.679306150696829747e-10,-1.505863991719219422e-09
+1.232352669999999989e+03,-5.681959877038930161e-10,-1.056192733251518993e-09,-6.715907582218806939e-10,-1.514280058019750009e-09
+1.234281230000000050e+03,-5.712272125814629613e-10,-1.060416352757778203e-09,-6.753906048535878817e-10,-1.521909032374687257e-09
+1.236209800000000087e+03,-5.740112260524037405e-10,-1.064851836612281208e-09,-6.790998177416906210e-10,-1.530443583558820058e-09
+1.238138359999999921e+03,-5.770800183823482469e-10,-1.069107449298257250e-09,-6.829506454952370476e-10,-1.538163979940113507e-09
+1.240066929999999957e+03,-5.798966764083870843e-10,-1.073586947464284730e-09,-6.867097669893221072e-10,-1.546819033277899282e-09
+1.241995490000000018e+03,-5.830036482747995217e-10,-1.077874858740538583e-09,-6.906124716220945617e-10,-1.554632413901839301e-09
+1.243924060000000054e+03,-5.858534724000310963e-10,-1.082398904032804684e-09,-6.944223785193303880e-10,-1.563410076145719910e-09
+1.245852619999999888e+03,-5.889992488288685915e-10,-1.086719423098922199e-09,-6.983778756700463502e-10,-1.571318037762716805e-09
+1.247781189999999924e+03,-5.918827716559966245e-10,-1.091288556420451440e-09,-7.022394642157622019e-10,-1.580220460923091719e-09
+1.249709749999999985e+03,-5.950679909627085041e-10,-1.095641996342496192e-09,-7.062486899431793842e-10,-1.588224635741705342e-09
+1.251638310000000047e+03,-5.979857407290182275e-10,-1.100256738956752613e-09,-7.101628559189177926e-10,-1.597253969475475410e-09
+1.253566880000000083e+03,-6.012110706034991307e-10,-1.104643444637228739e-09,-7.142267876976186526e-10,-1.605356074889662705e-09
+1.255495439999999917e+03,-6.041636184745527085e-10,-1.109304381789409167e-09,-7.181944880025952110e-10,-1.614514613423015549e-09
+1.257424009999999953e+03,-6.074297093690746992e-10,-1.113724646642380412e-09,-7.223140842578208395e-10,-1.622716307311530308e-09
+1.259352570000000014e+03,-6.104176229687639297e-10,-1.118432344568099055e-09,-7.263362767080495356e-10,-1.632006345614180349e-09
+1.261281140000000050e+03,-6.137251552748573685e-10,-1.122886493753553832e-09,-7.305125381729513145e-10,-1.640309372400628871e-09
+1.263209700000000112e+03,-6.167490145534189614e-10,-1.127641527514558665e-09,-7.345902022452268887e-10,-1.649733255624348040e-09
+1.265138269999999920e+03,-6.200986834635041474e-10,-1.132129890400971071e-09,-7.388241524082115711e-10,-1.658139399182393837e-09
+1.267066829999999982e+03,-6.231590810421858261e-10,-1.136932844085538473e-09,-7.429582898392324016e-10,-1.667699523988778933e-09
+1.268995390000000043e+03,-6.265515803357730622e-10,-1.141455725183954409e-09,-7.472509538386554741e-10,-1.676210556904557755e-09
+1.270923960000000079e+03,-6.296491384883888353e-10,-1.146307221260814505e-09,-7.514426109822308487e-10,-1.685909424635608375e-09
+1.272852519999999913e+03,-6.330852106208661505e-10,-1.150864987529226806e-09,-7.557950811690108490e-10,-1.694527264068409814e-09
+1.274781089999999949e+03,-6.362205319776682671e-10,-1.155765599893099597e-09,-7.600452847239352565e-10,-1.704367327441370384e-09
+1.276709650000000011e+03,-6.397009190603763191e-10,-1.160358593915987417e-09,-7.644586567246951210e-10,-1.713093882214172705e-09
+1.278638220000000047e+03,-6.428746364509364638e-10,-1.165308935001220808e-09,-7.687684790091669506e-10,-1.723077700804126986e-09
+1.280566780000000108e+03,-6.464000971249030928e-10,-1.169937503986008862e-09,-7.732438738632977124e-10,-1.731914923719062832e-09
+1.282495349999999917e+03,-6.496128575546090727e-10,-1.174938196125104187e-09,-7.776144120572153118e-10,-1.742045114342723372e-09
+1.284423909999999978e+03,-6.531841674612008011e-10,-1.179602692018067091e-09,-7.821529769377761021e-10,-1.750995003405711353e-09
+1.286352470000000039e+03,-6.564366149370045881e-10,-1.184654337171591487e-09,-7.865853306466054824e-10,-1.761274186538731497e-09
+1.288281040000000075e+03,-6.600545847903993233e-10,-1.189355147271771005e-09,-7.911882627484591021e-10,-1.770338841339507242e-09
+1.290209599999999909e+03,-6.633474132746647682e-10,-1.194458418506222678e-09,-7.956836038293190082e-10,-1.780769807346279923e-09
+1.292138169999999946e+03,-6.670128368365447248e-10,-1.199195874401965047e-09,-8.003520820410265887e-10,-1.789951265765882969e-09
+1.294066730000000007e+03,-6.703467383799771319e-10,-1.204351425215700292e-09,-8.049115865836639525e-10,-1.800536812664729592e-09
+1.295995300000000043e+03,-6.740604452915227091e-10,-1.209125893812117722e-09,-8.096468410602554765e-10,-1.809837216072463579e-09
+1.297923860000000104e+03,-6.774361278534048058e-10,-1.214334388620688526e-09,-8.142717129859132399e-10,-1.820580205623022425e-09
+1.299852429999999913e+03,-6.811989668131837552e-10,-1.219146242079662004e-09,-8.190750031535560717e-10,-1.830001745896662653e-09
+1.301780989999999974e+03,-6.846171547351462829e-10,-1.224408356496203182e-09,-8.237664750221692191e-10,-1.840905105357506857e-09
+1.303709550000000036e+03,-6.884299754297905994e-10,-1.229257940450280396e-09,-8.286390657594897515e-10,-1.850449967624859465e-09
+1.305638120000000072e+03,-6.918914285588631243e-10,-1.234574393490769726e-09,-8.333984242774959414e-10,-1.861516750246238844e-09
+1.307566679999999906e+03,-6.957551378950854335e-10,-1.239462122676979710e-09,-8.383416604551317033e-10,-1.871187289629918724e-09
+1.309495249999999942e+03,-6.992605964424006248e-10,-1.244833581627984250e-09,-8.431701736800242100e-10,-1.882420501305331490e-09
+1.311423810000000003e+03,-7.031761037399166521e-10,-1.249759844887336415e-09,-8.481854077679521400e-10,-1.892219070009843966e-09
+1.313352380000000039e+03,-7.067263442223485346e-10,-1.255187020742540231e-09,-8.530843993113277529e-10,-1.903621845619182674e-09
+1.315280940000000101e+03,-7.106945802321238221e-10,-1.260152212813900483e-09,-8.581730166444008688e-10,-1.913550852403205493e-09
+1.317209509999999909e+03,-7.142903976292822127e-10,-1.265635829000498247e-09,-8.631438422766067275e-10,-1.925126399939635709e-09
+1.319138069999999971e+03,-7.183123151834070843e-10,-1.270640350702282519e-09,-8.683072620334503123e-10,-1.935188311755454621e-09
+1.321066630000000032e+03,-7.219545037556133535e-10,-1.276181109961289203e-09,-8.733512843101550724e-10,-1.946939851774905277e-09
+1.322995200000000068e+03,-7.260310981952004330e-10,-1.281225401825040754e-09,-8.785909868602836059e-10,-1.957137258057353842e-09
+1.324923759999999902e+03,-7.297205110706848379e-10,-1.286824086618127620e-09,-8.837096547222262934e-10,-1.969068212750343476e-09
+1.326852329999999938e+03,-7.338527619500489240e-10,-1.291908529091548898e-09,-8.890271040662726385e-10,-1.979403640271515927e-09
+1.328780889999999999e+03,-7.375902530049566147e-10,-1.297565902263220371e-09,-8.942218756434001238e-10,-1.991517449610279002e-09
+1.330709460000000036e+03,-7.417791835563853547e-10,-1.302690915587689304e-09,-8.996185987280480012e-10,-2.001993550302566047e-09
+1.332638020000000097e+03,-7.455656275487137550e-10,-1.308407753888306336e-09,-9.048909683546437153e-10,-2.014293736050989911e-09
+1.334566589999999906e+03,-7.498122859435213564e-10,-1.313573765214565238e-09,-9.103685302489037101e-10,-2.024913227164352385e-09
+1.336495149999999967e+03,-7.536485791787198324e-10,-1.319350859710732566e-09,-9.157200295677850470e-10,-2.037403395231548060e-09
+1.338423710000000028e+03,-7.579540183319765150e-10,-1.324558268256698011e-09,-9.212800064830906552e-10,-2.048168994432213033e-09
+1.340352280000000064e+03,-7.618411003362217945e-10,-1.330396459816478634e-09,-9.267122337397841609e-10,-2.060852904121898136e-09
+1.342280839999999898e+03,-7.662064413773955615e-10,-1.335645741997586255e-09,-9.323562982593559100e-10,-2.071767531024048492e-09
+1.344209409999999934e+03,-7.701452329611964976e-10,-1.341545816916385216e-09,-9.378708354669222450e-10,-2.084648898069033604e-09
+1.346137969999999996e+03,-7.745716037084185390e-10,-1.346837422094624134e-09,-9.436006742000501078e-10,-2.095715477741565321e-09
+1.348066540000000032e+03,-7.785630700920309510e-10,-1.352800217030492811e-09,-9.491991719739075209e-10,-2.108798175421914054e-09
+1.349995100000000093e+03,-7.830516266336622719e-10,-1.358134602528020663e-09,-9.550165145880567779e-10,-2.120019706411417984e-09
+1.351923659999999927e+03,-7.870967355306995747e-10,-1.364160933858404625e-09,-9.607006360193361549e-10,-2.133307631953107365e-09
+1.353852229999999963e+03,-7.916486851407466276e-10,-1.369538601663622522e-09,-9.666072862635862535e-10,-2.144687258912303568e-09
+1.355780790000000025e+03,-7.957484732552334111e-10,-1.375629374916458007e-09,-9.723787968001828428e-10,-2.158184546520389365e-09
+1.357709360000000061e+03,-8.003650096622552278e-10,-1.381050763147238780e-09,-9.783765453461232855e-10,-2.169725352304735993e-09
+1.359637919999999895e+03,-8.045205181497807790e-10,-1.387206865005994788e-09,-9.842372260566740663e-10,-2.183436166824505078e-09
+1.361566489999999931e+03,-8.092028879184415631e-10,-1.392672456728806019e-09,-9.903279400654849489e-10,-2.195141384034088582e-09
+1.363495049999999992e+03,-8.134151849652505818e-10,-1.398894791663492629e-09,-9.962796182886660479e-10,-2.209069993336858027e-09
+1.365423620000000028e+03,-8.181646668344736966e-10,-1.404405079216717362e-09,-1.002465213696038312e-09,-2.220942937390585812e-09
+1.367352180000000089e+03,-8.224348485767109733e-10,-1.410694570083666325e-09,-1.008509764520494723e-09,-2.235093715457580689e-09
+1.369280739999999923e+03,-8.272527311165483195e-10,-1.416250017203423770e-09,-1.014792175803306565e-09,-2.247137711761738462e-09
+1.371209309999999959e+03,-8.315819460221747070e-10,-1.422607644104153332e-09,-1.020931555406825322e-09,-2.261515217227827085e-09
+1.373137870000000021e+03,-8.364695986913130903e-10,-1.428208800692267251e-09,-1.027312832111424458e-09,-2.273733828791525589e-09
+1.375066440000000057e+03,-8.408589786248539373e-10,-1.434635487340365029e-09,-1.033548984452566432e-09,-2.288342583327734674e-09
+1.376994999999999891e+03,-8.458177833360079506e-10,-1.440282875939334723e-09,-1.040031198474870800e-09,-2.300739389642663797e-09
+1.378923569999999927e+03,-8.502685142113684891e-10,-1.446779604251693789e-09,-1.046366151365723570e-09,-2.315584105169678697e-09
+1.380852129999999988e+03,-8.552998896488245651e-10,-1.452473758365258309e-09,-1.052951430017324811e-09,-2.328162779290882803e-09
+1.382780700000000024e+03,-8.598131894225988724e-10,-1.459041531365380251e-09,-1.059387265535365888e-09,-2.343248287292982564e-09
+1.384709260000000086e+03,-8.649185923174808747e-10,-1.464782995948435969e-09,-1.066077793369108891e-09,-2.356012598766926013e-09
+1.386637819999999920e+03,-8.694956871645844826e-10,-1.471422798299320109e-09,-1.072616615518290982e-09,-2.371343773101439513e-09
+1.388566389999999956e+03,-8.746766385887804994e-10,-1.477212170492843782e-09,-1.079414670357605500e-09,-2.384297671833337766e-09
+1.390494950000000017e+03,-8.793188386141844307e-10,-1.483925089601093297e-09,-1.086058708770449283e-09,-2.399879673845167448e-09
+1.392423520000000053e+03,-8.845768508441809201e-10,-1.489762899075107361e-09,-1.092966561838190515e-09,-2.413027051993395034e-09
+1.394352079999999887e+03,-8.892854771586487236e-10,-1.496550006100392256e-09,-1.099718072410379581e-09,-2.428865094377812814e-09
+1.396280649999999923e+03,-8.946221292955725094e-10,-1.502436835428710442e-09,-1.106738091687062381e-09,-2.442210029621855537e-09
+1.398209209999999985e+03,-8.993985399200184860e-10,-1.509299226011332845e-09,-1.113599392182682240e-09,-2.458309460131523409e-09
+1.400137780000000021e+03,-9.048154547989487920e-10,-1.515235671520303348e-09,-1.120734010948437424e-09,-2.471856139449394621e-09
+1.402066340000000082e+03,-9.096610460230257991e-10,-1.522174466745459312e-09,-1.127707483095697355e-09,-2.488222445124477395e-09
+1.403994899999999916e+03,-9.151598651325194936e-10,-1.528161096837246559e-09,-1.134959165453312843e-09,-2.501975081485188812e-09
+1.405923469999999952e+03,-9.200760996021401758e-10,-1.535177486570793785e-09,-1.142047293826141010e-09,-2.518613979811931594e-09
+1.407852030000000013e+03,-9.256585643362482571e-10,-1.541214969029830990e-09,-1.149418646503035366e-09,-2.532577074832567326e-09
+1.409780600000000049e+03,-9.306468929433866432e-10,-1.548310086495616857e-09,-1.156623911297174430e-09,-2.549494259333247764e-09
+1.411709160000000111e+03,-9.363147671296673476e-10,-1.554399063140919639e-09,-1.164117577155880376e-09,-2.563672349370023406e-09
+1.413637729999999920e+03,-9.413767097783808766e-10,-1.561574112097426172e-09,-1.171442565455314527e-09,-2.580873751910695354e-09
+1.415566289999999981e+03,-9.471318077648436415e-10,-1.567715241501954368e-09,-1.179061262105937618e-09,-2.595271497411280304e-09
+1.417494860000000017e+03,-9.522689287288513393e-10,-1.574971455593145946e-09,-1.186508634238358447e-09,-2.612763207669048059e-09
+1.419423420000000078e+03,-9.581131172822302221e-10,-1.581165413966251685e-09,-1.194255156650569632e-09,-2.627385397217125513e-09
+1.421351979999999912e+03,-9.633269984015358117e-10,-1.588504013336017261e-09,-1.201827609231051536e-09,-2.645173574312264439e-09
+1.423280549999999948e+03,-9.692622272114548636e-10,-1.594751540091930510e-09,-1.209704871980868284e-09,-2.660025222221307686e-09
+1.425209110000000010e+03,-9.745545547918073609e-10,-1.602173866230605502e-09,-1.217405258484646286e-09,-2.678116378752370364e-09
+1.427137680000000046e+03,-9.805827734453324379e-10,-1.608475631605577199e-09,-1.225416180687468810e-09,-2.693202450723855953e-09
+1.429066240000000107e+03,-9.859552554642367474e-10,-1.615983015809701590e-09,-1.233247396993348456e-09,-2.711603180947260069e-09
+1.430994809999999916e+03,-9.920785003090091255e-10,-1.622339754831874350e-09,-1.241395022512506329e-09,-2.726928875776344020e-09
+1.432923369999999977e+03,-9.975328964761049818e-10,-1.629933563908942397e-09,-1.249360048678126019e-09,-2.745645953213552712e-09
+1.434851940000000013e+03,-1.003753264823896907e-09,-1.636346033423823326e-09,-1.257647510340182336e-09,-2.761216615561921182e-09
+1.436780500000000075e+03,-1.009291388655220967e-09,-1.644027671320818758e-09,-1.265749413635106368e-09,-2.780256998876043060e-09
+1.438709059999999909e+03,-1.015611010611717560e-09,-1.650496604093413886e-09,-1.274179893796431205e-09,-2.796078023472726305e-09
+1.440637629999999945e+03,-1.021234762182820765e-09,-1.658267560721904706e-09,-1.282421874522173516e-09,-2.815448963186146434e-09
+1.442566190000000006e+03,-1.027655894403723712e-09,-1.664793807622327657e-09,-1.290998735644942424e-09,-2.831526100142555521e-09
+1.444494760000000042e+03,-1.033367171401939335e-09,-1.672655519949743598e-09,-1.299384003215840973e-09,-2.851234844788526582e-09
+1.446423320000000103e+03,-1.039892108980565144e-09,-1.679239911066753104e-09,-1.308110664882245162e-09,-2.867573906206510109e-09
+1.448351889999999912e+03,-1.045692899877458805e-09,-1.687193905284041793e-09,-1.316642567774466826e-09,-2.887628007434191527e-09
+1.450280449999999973e+03,-1.052324009226124992e-09,-1.693837298057308204e-09,-1.325522552277018097e-09,-2.904234971844782361e-09
+1.452209020000000010e+03,-1.058216365710098089e-09,-1.701885145112430788e-09,-1.334204539701014496e-09,-2.924642192280242451e-09
+1.454137580000000071e+03,-1.064956087485253443e-09,-1.708588425972941733e-09,-1.343241475868738436e-09,-2.941523210276189011e-09
+1.456066139999999905e+03,-1.070942094304167760e-09,-1.716731693923394580e-09,-1.352077055421356871e-09,-2.962291421865234618e-09
+1.457994709999999941e+03,-1.077792979308018849e-09,-1.723495829879754335e-09,-1.361274728733866868e-09,-2.979452930655108958e-09
+1.459923270000000002e+03,-1.083874855012061036e-09,-1.731736235281361492e-09,-1.370267607849320861e-09,-3.000590446408081942e-09
+1.461851840000000038e+03,-1.090839469490377794e-09,-1.738562126919758709e-09,-1.379629827093336740e-09,-3.018038851617215954e-09
+1.463780400000000100e+03,-1.097019471978611185e-09,-1.746901388943222612e-09,-1.388783780444430000e-09,-3.039554110723847784e-09
+1.465708969999999908e+03,-1.104100498444253900e-09,-1.753790020760736592e-09,-1.398314518804906177e-09,-3.057296115132017552e-09
+1.467637529999999970e+03,-1.110380960382661797e-09,-1.762229913188060617e-09,-1.407633437915232971e-09,-3.079197797844615889e-09
+1.469566100000000006e+03,-1.117581168903885416e-09,-1.769182306542259554e-09,-1.417336792235847026e-09,-3.097240301046759884e-09
+1.471494660000000067e+03,-1.123964501014612813e-09,-1.777724660659553718e-09,-1.426824689982624706e-09,-3.119537336949806547e-09
+1.473423219999999901e+03,-1.131286717650490868e-09,-1.784741823305553338e-09,-1.436704835579615942e-09,-3.137887324543076372e-09
+1.475351789999999937e+03,-1.137775447532404605e-09,-1.793388583752268720e-09,-1.446365900881281923e-09,-3.160589018700862306e-09
+1.477280349999999999e+03,-1.145222663767742923e-09,-1.800471670157996752e-09,-1.456427245548612172e-09,-3.179253920066984099e-09
+1.479208920000000035e+03,-1.151819334111280142e-09,-1.809224740588567652e-09,-1.466265699295752094e-09,-3.202369611347671291e-09
+1.481137480000000096e+03,-1.159394606201339224e-09,-1.816374897527397829e-09,-1.476512740448698857e-09,-3.221356958274786446e-09
+1.483066049999999905e+03,-1.166101883529263727e-09,-1.825236301147400897e-09,-1.486532988784275196e-09,-3.244896377217295181e-09
+1.484994609999999966e+03,-1.173808371706749138e-09,-1.832454722820061523e-09,-1.496970368030141590e-09,-3.264213927090355565e-09
+1.486923170000000027e+03,-1.180628978219315569e-09,-1.841426498702133394e-09,-1.507176905421353734e-09,-3.288186964741069327e-09
+1.488851740000000063e+03,-1.188469988871182692e-09,-1.848714485184181836e-09,-1.517809467590496981e-09,-3.307842833661420287e-09
+1.490780299999999897e+03,-1.195406818570921219e-09,-1.857798857686034019e-09,-1.528207041308652965e-09,-3.332259925227905842e-09
+1.492708869999999933e+03,-1.203385697397669519e-09,-1.865157653136155074e-09,-1.539039681683939046e-09,-3.352262222730858755e-09
+1.494637429999999995e+03,-1.210441709510152509e-09,-1.874356871603098819e-09,-1.549633139934279964e-09,-3.377133986624274773e-09
+1.496566000000000031e+03,-1.218561957937306879e-09,-1.881787832442722276e-09,-1.560670968421653497e-09,-3.397491195453882758e-09
+1.498494560000000092e+03,-1.225740218610926450e-09,-1.891104230556265560e-09,-1.571465318883631865e-09,-3.422828567248903469e-09
+1.500423129999999901e+03,-1.234005462489199878e-09,-1.898608774829964282e-09,-1.582713614364588062e-09,-3.443549429151361401e-09
+1.502351689999999962e+03,-1.241309149937596115e-09,-1.908044775626744236e-09,-1.593714030751749219e-09,-3.469363672885074985e-09
+1.504280250000000024e+03,-1.249723104867956104e-09,-1.915624328427944180e-09,-1.605178190097751071e-09,-3.490457061770612459e-09
+1.506208820000000060e+03,-1.257155555375389223e-09,-1.925182508478241181e-09,-1.616390077014295491e-09,-3.516759917640661916e-09
+1.508137379999999894e+03,-1.265722153857406148e-09,-1.932838682352066182e-09,-1.628075795187547705e-09,-3.538235254590449677e-09
+1.510065949999999930e+03,-1.273286746635254522e-09,-1.942521601951186428e-09,-1.639504622583162712e-09,-3.565038545843390827e-09
+1.511994509999999991e+03,-1.282010024453748544e-09,-1.950256026885138639e-09,-1.651417728657018603e-09,-3.586905405954174836e-09
+1.513923080000000027e+03,-1.289710308000937540e-09,-1.960066411123178270e-09,-1.663069211123801711e-09,-3.614221454488739023e-09
+1.515851640000000089e+03,-1.298594451066739492e-09,-1.967880798047404470e-09,-1.675215733249025172e-09,-3.636489710677563774e-09
+1.517780209999999897e+03,-1.306434109853112899e-09,-1.977821485495016310e-09,-1.687095781144154274e-09,-3.664331216789215690e-09
+1.519708769999999959e+03,-1.315483461635143542e-09,-1.985717632124298696e-09,-1.699481955062457648e-09,-3.687011050426795410e-09
+1.521637330000000020e+03,-1.323466279073510310e-09,-1.995791519233526524e-09,-1.711596619697973819e-09,-3.715390958424807471e-09
+1.523565900000000056e+03,-1.332685392461480242e-09,-2.003771379129158669e-09,-1.724228960929549455e-09,-3.738493018445928419e-09
+1.525494459999999890e+03,-1.340815389360322483e-09,-2.013981615622574971e-09,-1.736584631840635642e-09,-3.767424972623070182e-09
+1.527423029999999926e+03,-1.350208903977999965e-09,-2.022047117635622975e-09,-1.749469756689880777e-09,-3.790959945501027816e-09
+1.529351589999999987e+03,-1.358490216125242900e-09,-2.032396928172503158e-09,-1.762072983775360609e-09,-3.820457866160056868e-09
+1.531280160000000024e+03,-1.368062997537748070e-09,-2.040550170388358901e-09,-1.775217806460521210e-09,-3.844436926474400084e-09
+1.533208720000000085e+03,-1.376499927235458841e-09,-2.051042925612508719e-09,-1.788075371804172056e-09,-3.874515170855097717e-09
+1.535137289999999894e+03,-1.386257033286089685e-09,-2.059286121482401039e-09,-1.801487052922450446e-09,-3.898949848243023315e-09
+1.537065849999999955e+03,-1.394854058274781541e-09,-2.069925347813744138e-09,-1.814605981150508643e-09,-3.929623226663535192e-09
+1.538994410000000016e+03,-1.404800701342922931e-09,-2.078260767655933651e-09,-1.828291869542308309e-09,-3.954525256967602580e-09
+1.540922980000000052e+03,-1.413562532193182051e-09,-2.089050224970037872e-09,-1.841679507923682449e-09,-3.985809211113660047e-09
+1.542851540000000114e+03,-1.423704232654162209e-09,-2.097480406019094501e-09,-1.855647358397302536e-09,-4.011191031154430963e-09
+1.544780109999999922e+03,-1.432635680260620742e-09,-2.108423898708068836e-09,-1.869311182272506177e-09,-4.043101170162996630e-09
+1.546708669999999984e+03,-1.442978136242828510e-09,-2.116951455726634104e-09,-1.883568963189115711e-09,-4.068975452899053333e-09
+1.548637240000000020e+03,-1.452084264455489429e-09,-2.128053044478492947e-09,-1.897516792855898811e-09,-4.101528049814418100e-09
+1.550565800000000081e+03,-1.462633411096035028e-09,-2.136680747138452567e-09,-1.912072766885151034e-09,-4.127907876978406554e-09
+1.552494369999999890e+03,-1.471919501377943382e-09,-2.147944696180268298e-09,-1.926312712669208455e-09,-4.161119729215897750e-09
+1.554422929999999951e+03,-1.482681523963526524e-09,-2.156675481158586562e-09,-1.941175450497119323e-09,-4.188018605922485952e-09
+1.556351490000000013e+03,-1.492153035566151194e-09,-2.168106200514488867e-09,-1.955715850460387910e-09,-4.221906877986745901e-09
+1.558280060000000049e+03,-1.503134435852371950e-09,-2.176943256778970044e-09,-1.970894321174348953e-09,-4.249338924640735400e-09
+1.560208620000000110e+03,-1.512797174852985104e-09,-2.188545533627415699e-09,-1.985743981528763111e-09,-4.283921695713815956e-09
+1.562137189999999919e+03,-1.524004630383859220e-09,-2.197492101388367935e-09,-2.001247341896663966e-09,-4.311901136650011247e-09
+1.564065749999999980e+03,-1.533864609285526237e-09,-2.209270902615518668e-09,-2.016415327755306474e-09,-4.347196898112100754e-09
+1.565994320000000016e+03,-1.545305144201290009e-09,-2.218330503145984471e-09,-2.032253162937362508e-09,-4.375738601123155758e-09
+1.567922880000000077e+03,-1.555368648483058249e-09,-2.230291065055004043e-09,-2.047748888740182321e-09,-4.411766452041670413e-09
+1.569851450000000114e+03,-1.567049599572848024e-09,-2.239467446588708742e-09,-2.063931155162431184e-09,-4.440885771581372805e-09
+1.571780009999999947e+03,-1.577323204148316433e-09,-2.251615295043360348e-09,-2.079764401753073256e-09,-4.477665441593739496e-09
+1.573708570000000009e+03,-1.589252182044145335e-09,-2.260912373325967732e-09,-2.096301361784420640e-09,-4.507378041845828056e-09
+1.575637140000000045e+03,-1.599742826310388063e-09,-2.273253423443588994e-09,-2.112482378072340764e-09,-4.544930108761369219e-09
+1.577565700000000106e+03,-1.611927906237293772e-09,-2.282675534365928304e-09,-2.129384868137256597e-09,-4.575252559025141720e-09
+1.579494269999999915e+03,-1.622642742272598597e-09,-2.295215882185695843e-09,-2.145924141508857059e-09,-4.613597895862220089e-09
+1.581422829999999976e+03,-1.635092315830429220e-09,-2.304767572570736955e-09,-2.163203345603921718e-09,-4.644547114587783355e-09
+1.583351400000000012e+03,-1.646038898542310990e-09,-2.317513751902113140e-09,-2.180111869343644270e-09,-4.683707488778214879e-09
+1.585279960000000074e+03,-1.658761752918712693e-09,-2.327199880215568924e-09,-2.197779422574066265e-09,-4.715300952041735215e-09
+1.587208530000000110e+03,-1.669948005977489166e-09,-2.340158814364482209e-09,-2.215068635792089235e-09,-4.755298861938749432e-09
+1.589137089999999944e+03,-1.682953348780874430e-09,-2.349984576971418309e-09,-2.233136647528154964e-09,-4.787554622271301043e-09
+1.591065650000000005e+03,-1.694387525285153781e-09,-2.363163524947194674e-09,-2.250818365939891772e-09,-4.828413110947508380e-09
+1.592994220000000041e+03,-1.707685074507393271e-09,-2.373134569301026946e-09,-2.269299536741270308e-09,-4.861350029976653549e-09
+1.594922780000000103e+03,-1.719375970847433664e-09,-2.386541411872800379e-09,-2.287386251940740192e-09,-4.903093349686876678e-09
+1.596851349999999911e+03,-1.732975795648563294e-09,-2.396663615923605830e-09,-2.306293625026991547e-09,-4.936730481841196758e-09
+1.598779909999999973e+03,-1.744932592623160380e-09,-2.410306641504914139e-09,-2.324798257954358129e-09,-4.979383491579329595e-09
+1.600708480000000009e+03,-1.758845331306160437e-09,-2.420586398649718953e-09,-2.344145519838784065e-09,-5.013740735257159455e-09
+1.602637040000000070e+03,-1.771077686059414853e-09,-2.434474426718742279e-09,-2.363081538875481775e-09,-5.057329140070215478e-09
+1.604565610000000106e+03,-1.785314518053320368e-09,-2.444918600481790354e-09,-2.382882958916834593e-09,-5.092427048633599218e-09
+1.606494169999999940e+03,-1.797832596731876594e-09,-2.459061025611544451e-09,-2.402264409619212714e-09,-5.136977430698997919e-09
+1.608422730000000001e+03,-1.812405209125992810e-09,-2.469676898633105069e-09,-2.422534769446699156e-09,-5.172836997051292579e-09
+1.610351300000000037e+03,-1.825219792359508839e-09,-2.484083830910270769e-09,-2.442376408670611496e-09,-5.218377083002583470e-09
+1.612279860000000099e+03,-1.840140628038659570e-09,-2.494879425703986737e-09,-2.463131340772715035e-09,-5.255020461097534150e-09
+1.614208429999999908e+03,-1.853262940920885633e-09,-2.509561468703644508e-09,-2.483448365944945279e-09,-5.301578453808130812e-09
+1.616136989999999969e+03,-1.868545034755163259e-09,-2.520545323975998901e-09,-2.504704087696089063e-09,-5.339028282338985642e-09
+1.618065560000000005e+03,-1.881986995536052313e-09,-2.535513905935057774e-09,-2.525512475414537285e-09,-5.386633590430533970e-09
+1.619994120000000066e+03,-1.897644089585742878e-09,-2.546695222147619892e-09,-2.547285927903747378e-09,-5.424913243056498945e-09
+1.621922690000000102e+03,-1.911418286758234548e-09,-2.561962569199850599e-09,-2.568602372811398317e-09,-5.473596284833226837e-09
+1.623851249999999936e+03,-1.927464881160932796e-09,-2.573351268990432765e-09,-2.590911262442850390e-09,-5.512729889456785088e-09
+1.625779809999999998e+03,-1.941584544990575219e-09,-2.588930373414301578e-09,-2.612753104893332347e-09,-5.562521866814949525e-09
+1.627708380000000034e+03,-1.958036031478747357e-09,-2.600537269745166576e-09,-2.635616062006740031e-09,-5.602534584947348859e-09
+1.629636940000000095e+03,-1.972515320383118178e-09,-2.616442270317380199e-09,-2.658001671934289399e-09,-5.653468295657625828e-09
+1.631565509999999904e+03,-1.989387810475697775e-09,-2.628278837152966494e-09,-2.681437959483004474e-09,-5.694385563595777998e-09
+1.633494069999999965e+03,-2.004241639835635039e-09,-2.644524802969293191e-09,-2.704386448009727460e-09,-5.746494665855534785e-09
+1.635422640000000001e+03,-2.021552261206418987e-09,-2.656603556912625958e-09,-2.728416349442220996e-09,-5.788342981764296764e-09
+1.637351200000000063e+03,-2.036796444227146564e-09,-2.673206680862495653e-09,-2.751947731760863846e-09,-5.841662285238380644e-09
+1.639279759999999897e+03,-2.054563251261276507e-09,-2.685541060773306318e-09,-2.776592370677090174e-09,-5.884468686038554916e-09
+1.641208329999999933e+03,-2.070214655330464222e-09,-2.702518873059399483e-09,-2.800727746061760235e-09,-5.939034470171288603e-09
+1.643136889999999994e+03,-2.088456962285022486e-09,-2.715123667565968563e-09,-2.826009515789133463e-09,-5.982827386216781380e-09
+1.645065460000000030e+03,-2.104533332599588904e-09,-2.732494822138521522e-09,-2.850770757467872908e-09,-6.038676594072293685e-09
+1.646994020000000091e+03,-2.123271548394256241e-09,-2.745385953222618862e-09,-2.876713018396207114e-09,-6.083485023741785616e-09
+1.648922589999999900e+03,-2.139791845291126175e-09,-2.763170679733729126e-09,-2.902123205132186783e-09,-6.140656131531955138e-09
+1.650851149999999961e+03,-2.159047651962645215e-09,-2.776365432204338839e-09,-2.928750475344658854e-09,-6.186509924650216698e-09
+1.652779719999999998e+03,-2.176032061620577573e-09,-2.794585568458043395e-09,-2.954833839973055382e-09,-6.245042698764858260e-09
+1.654708280000000059e+03,-2.195828519021040305e-09,-2.808102724809538657e-09,-2.982171870187834217e-09,-6.291972559624983986e-09
+1.656636839999999893e+03,-2.213298460380253649e-09,-2.826781748296420880e-09,-3.008953735380559151e-09,-6.351907772916907293e-09
+1.658565409999999929e+03,-2.233660218122014287e-09,-2.840641862133557954e-09,-3.037029729880260687e-09,-6.399945573511029244e-09
+1.660493969999999990e+03,-2.251638744154848046e-09,-2.859805431164161569e-09,-3.064537005613538104e-09,-6.461325972626882535e-09
+1.662422540000000026e+03,-2.272591881790628071e-09,-2.874030626088707043e-09,-3.093379294500941862e-09,-6.510503807549020853e-09
+1.664351100000000088e+03,-2.291103521430362415e-09,-2.893706406329135667e-09,-3.121640154915418254e-09,-6.573373208133131161e-09
+1.666279669999999896e+03,-2.312675973406024076e-09,-2.908320926266558717e-09,-3.151278701516461840e-09,-6.623724310199010477e-09
+1.668208229999999958e+03,-2.331746965261283155e-09,-2.928538925385963270e-09,-3.180322817545488133e-09,-6.688127926728802416e-09
+1.670136799999999994e+03,-2.353968582594004664e-09,-2.943569220987930178e-09,-3.210789185957704567e-09,-6.739686336339477376e-09
+1.672065360000000055e+03,-2.373627029969547352e-09,-2.964362026990471294e-09,-3.240647830321487491e-09,-6.805670798815976130e-09
+1.673993919999999889e+03,-2.396529642348989292e-09,-2.979836845996942711e-09,-3.271975140222733650e-09,-6.858470978964125046e-09
+1.675922489999999925e+03,-2.416805795902156713e-09,-3.001240033729334484e-09,-3.302681459973323740e-09,-6.926084694620980942e-09
+1.677851049999999987e+03,-2.440423731137322476e-09,-3.017191097670204797e-09,-3.334904979467439188e-09,-6.980162532783612808e-09
+1.679779620000000023e+03,-2.461349852693470824e-09,-3.039243109052394650e-09,-3.366493651117153687e-09,-7.049454641736485662e-09
+1.681708180000000084e+03,-2.485719825481756524e-09,-3.055704988440210544e-09,-3.399650465804600489e-09,-7.104846351700678791e-09
+1.683636749999999893e+03,-2.507330726225733281e-09,-3.078447879092359033e-09,-3.432158297384700308e-09,-7.175867756535863449e-09
+1.685565309999999954e+03,-2.532492183014128280e-09,-3.095458455030063697e-09,-3.466287611221997573e-09,-7.232610145058039161e-09
+1.687493879999999990e+03,-2.554825355070309984e-09,-3.118938131454801968e-09,-3.499753538191510716e-09,-7.305413146927571696e-09
+1.689422440000000051e+03,-2.580820739648699470e-09,-3.136538960349424175e-09,-3.534896834769968029e-09,-7.363543516284758350e-09
+1.691351000000000113e+03,-2.603916495644655806e-09,-3.160805436837455171e-09,-3.569361904344134153e-09,-7.438181384047235503e-09
+1.693279569999999921e+03,-2.630791674058760577e-09,-3.179042323235593697e-09,-3.605563303991283689e-09,-7.497737804435720800e-09
+1.695208129999999983e+03,-2.654693825160367201e-09,-3.204150677810936068e-09,-3.641071390151155996e-09,-7.574265894415865068e-09
+1.697136700000000019e+03,-2.682498040765248511e-09,-3.223073654516037265e-09,-3.678377310437459099e-09,-7.635285879088045634e-09
+1.699065260000000080e+03,-2.707253859286699786e-09,-3.249084083344983660e-09,-3.714974783880678385e-09,-7.713760392867956289e-09
+1.700993829999999889e+03,-2.736040481836238454e-09,-3.268748410686550869e-09,-3.753434683780109206e-09,-7.776281875564226235e-09
+1.702922389999999950e+03,-2.761701204032421999e-09,-3.295726987583440834e-09,-3.791170806473743461e-09,-7.856760139937279311e-09
+1.704850959999999986e+03,-2.791528028601154337e-09,-3.316193586446094566e-09,-3.830837249213501712e-09,-7.920820862004862525e-09
+1.706779520000000048e+03,-2.818149283005342722e-09,-3.344212943603208096e-09,-3.869764417735649246e-09,-8.003361190086155912e-09
+1.708708080000000109e+03,-2.849078857098961515e-09,-3.365548872365736920e-09,-3.910693127436958901e-09,-8.068997979110520123e-09
+1.710636649999999918e+03,-2.876721299110799835e-09,-3.394689163658509390e-09,-3.950867349501295300e-09,-8.153659933346916734e-09
+1.712565209999999979e+03,-2.908821906244479582e-09,-3.416968946860736371e-09,-3.993118116245618134e-09,-8.220909683973177734e-09
+1.714493780000000015e+03,-2.937551324324723727e-09,-3.447318156988522954e-09,-4.034598697988692664e-09,-8.307752529327630250e-09
+1.716422340000000077e+03,-2.970897158455716158e-09,-3.470624087604004329e-09,-4.078235096573431466e-09,-8.376650486670923044e-09
+1.718350910000000113e+03,-3.000785537896634302e-09,-3.502279590913640902e-09,-4.121085583892515550e-09,-8.465734207012417832e-09
+1.720279469999999947e+03,-3.035457544932711652e-09,-3.526702901117525894e-09,-4.166175536940216485e-09,-8.536313903986497976e-09
+1.722208039999999983e+03,-3.066583636725093163e-09,-3.559772415761593159e-09,-4.210463889587241129e-09,-8.627698407218470407e-09
+1.724136600000000044e+03,-3.102670309886271283e-09,-3.585414403069220250e-09,-4.257080073759307632e-09,-8.699991066566192405e-09
+1.726065160000000105e+03,-3.135120267449660712e-09,-3.620017060817260452e-09,-4.302878845720823443e-09,-8.793735232591980709e-09
+1.727993729999999914e+03,-3.172718736187599366e-09,-3.646990609876986316e-09,-4.351099386853903709e-09,-8.867769544034635366e-09
+1.729922289999999975e+03,-3.206587579655844229e-09,-3.683259136860579761e-09,-4.398486907367546778e-09,-8.963932150487703150e-09
+1.731850860000000011e+03,-3.245804124898322309e-09,-3.711689514748776605e-09,-4.448395184319591026e-09,-9.039731914191425697e-09
+1.733779420000000073e+03,-3.281196295320075821e-09,-3.749771269885355289e-09,-4.497455388629078246e-09,-9.138369469656269716e-09
+1.735707990000000109e+03,-3.322148073160125279e-09,-3.779798507164819319e-09,-4.549141314259124139e-09,-9.215954015880396868e-09
+1.737636549999999943e+03,-3.359178845561733080e-09,-3.819857683098952017e-09,-4.599964576966021906e-09,-9.317120392441693714e-09
+1.739565119999999979e+03,-3.401995103491143618e-09,-3.851638319463583000e-09,-4.653525023438794432e-09,-9.396502822997432587e-09
+1.741493680000000040e+03,-3.440792023988590848e-09,-3.893858228276793161e-09,-4.706208842114634946e-09,-9.500248203592235701e-09
+1.743422240000000102e+03,-3.485615490044234491e-09,-3.927567300915589554e-09,-4.761748107084749665e-09,-9.581433291051628672e-09
+1.745350809999999910e+03,-3.526320264063527033e-09,-3.972153312012366483e-09,-4.816398161630940544e-09,-9.687803435114763952e-09
+1.747279369999999972e+03,-3.573309662081347384e-09,-4.007987854297855585e-09,-4.874029650556675040e-09,-9.770787431183296603e-09
+1.749207940000000008e+03,-3.616079454609903215e-09,-4.055169622824541099e-09,-4.930759863565379055e-09,-9.879820409769762834e-09
+1.751136500000000069e+03,-3.665411050136458729e-09,-4.093350904871206255e-09,-4.990606245148242468e-09,-9.964587125401835792e-09
+1.753065070000000105e+03,-3.710421398658786737e-09,-4.143386801631017684e-09,-5.049540625493739259e-09,-1.007631301340500037e-08
+1.754993629999999939e+03,-3.762291763414375980e-09,-4.184164205627608163e-09,-5.111735224398567004e-09,-1.016283161667127004e-08
+1.756922199999999975e+03,-3.809739044138524794e-09,-4.237345246519365626e-09,-5.173008776508164630e-09,-1.027726952421836589e-08
+1.758850760000000037e+03,-3.864368061963543561e-09,-4.281000487514960753e-09,-5.237696869891010819e-09,-1.036549118756629079e-08
+1.760779320000000098e+03,-3.914472370135249860e-09,-4.337654897146798178e-09,-5.301456626661974773e-09,-1.048264563879602952e-08
+1.762707889999999907e+03,-3.972107062933371029e-09,-4.384507363904025328e-09,-5.368797281881527553e-09,-1.057250007110393844e-08
+1.764636449999999968e+03,-4.025116761374580922e-09,-4.445007498956022966e-09,-5.435204879951464177e-09,-1.069235918502584160e-08
+1.766565020000000004e+03,-4.086034691982480415e-09,-4.495419025410660300e-09,-5.505371722520265672e-09,-1.078374772913776774e-08
+1.768493580000000065e+03,-4.142230065379844082e-09,-4.560187187852911521e-09,-5.574604287882531829e-09,-1.090627676632999110e-08
+1.770422150000000101e+03,-4.206745155562834990e-09,-4.614570093007397828e-09,-5.647788529491461210e-09,-1.099906807806852363e-08
+1.772350709999999935e+03,-4.266443993279409851e-09,-4.684087078990380488e-09,-5.720041181615106865e-09,-1.112420434951983721e-08
+1.774279269999999997e+03,-4.334911942215466614e-09,-4.742911641148028233e-09,-5.796453334449906947e-09,-1.121822546072109437e-08
+1.776207840000000033e+03,-4.398476274441907802e-09,-4.817726997034079749e-09,-5.871942153223985400e-09,-1.134587188450812144e-08
+1.778136400000000094e+03,-4.471302798159228371e-09,-4.881532765901271189e-09,-5.951816038386748377e-09,-1.144090076973838922e-08
+1.780064969999999903e+03,-4.539145637323340733e-09,-4.962275158842487187e-09,-6.030779989869943932e-09,-1.157091490597160132e-08
+1.781993529999999964e+03,-4.616794274951672237e-09,-5.031681558101962182e-09,-6.114375029629257775e-09,-1.166666665548941866e-08
+1.783922100000000000e+03,-4.689389989620873587e-09,-5.119074288659025318e-09,-6.197080758029487803e-09,-1.179885148839570912e-08
+1.785850660000000062e+03,-4.772393117284706579e-09,-5.194795512362790493e-09,-6.284686442728037524e-09,-1.189496419832807787e-08
+1.787779230000000098e+03,-4.850288614141527498e-09,-5.289673258924490296e-09,-6.371432313872240837e-09,-1.202905325374217930e-08
+1.789707789999999932e+03,-4.939260560237456024e-09,-5.372535855215068180e-09,-6.463373147800692555e-09,-1.212506941551700170e-08
+1.791636349999999993e+03,-5.023088984022077506e-09,-5.475864976087654084e-09,-6.554494120050884353e-09,-1.226070794624272574e-08
+1.793564920000000029e+03,-5.118742678895094730e-09,-5.566830025850097139e-09,-6.651136111407938009e-09,-1.235605161293310106e-08
+1.795493480000000091e+03,-5.209242306487925791e-09,-5.679736228041302516e-09,-6.747011669216090906e-09,-1.249277570724922335e-08
+1.797422049999999899e+03,-5.312408074464784021e-09,-5.779923926849252052e-09,-6.848768289645797695e-09,-1.258672022154363016e-08
+1.799350609999999961e+03,-5.410442933181016730e-09,-5.903722198360786352e-09,-6.949829091279827552e-09,-1.272392483932559850e-08
+1.801279179999999997e+03,-5.522095028609040974e-09,-6.014446613186686885e-09,-7.057171754576214696e-09,-1.281555644871692753e-08
+1.803207740000000058e+03,-5.628682930767590179e-09,-6.150681446291927312e-09,-7.163910047708894105e-09,-1.295245758436980299e-08
+1.805136310000000094e+03,-5.749970987321777994e-09,-6.273491002351834462e-09,-7.277378985027967676e-09,-1.304062477510975846e-08
+1.807064869999999928e+03,-5.866318592524711762e-09,-6.423986101430549168e-09,-7.390361074783905721e-09,-1.317620906235672637e-08
+1.808993429999999989e+03,-5.998607595095279179e-09,-6.560714380011823153e-09,-7.510578966719976264e-09,-1.325945665956661738e-08
+1.810922000000000025e+03,-6.126156020113236395e-09,-6.727636561701276141e-09,-7.630461580898274864e-09,-1.339241570402847736e-08
+1.812850560000000087e+03,-6.271080546582633569e-09,-6.880471017118663901e-09,-7.758153432444290081e-09,-1.346890132753972251e-08
+1.814779129999999896e+03,-6.411561624686696488e-09,-7.066407712474929497e-09,-7.885702043344420838e-09,-1.359754112795224578e-08
+1.816707689999999957e+03,-6.571092012551208603e-09,-7.237971416051692086e-09,-8.021716632962923696e-09,-1.366491881656579809e-08
+1.818636259999999993e+03,-6.726606338004996730e-09,-7.446037148884672247e-09,-8.157833182406972585e-09,-1.378704330426386315e-08
+1.820564820000000054e+03,-6.903138811155501916e-09,-7.639499359012089073e-09,-8.303173766534721648e-09,-1.384231081725795942e-08
+1.822493390000000090e+03,-7.076256016375087945e-09,-7.873470144170986180e-09,-8.448930019293361717e-09,-1.395505975093292895e-08
+1.824421949999999924e+03,-7.272731924743287974e-09,-8.092690243589391381e-09,-8.604793943879513256e-09,-1.399434971548043047e-08
+1.826350509999999986e+03,-7.466624987942019001e-09,-8.357180642655318257e-09,-8.761475580979593169e-09,-1.409397604504898339e-08
+1.828279080000000022e+03,-7.686692865008970669e-09,-8.606901086615324814e-09,-8.929307903229105286e-09,-1.411226848308346045e-08
+1.830207640000000083e+03,-7.905325380722406745e-09,-8.907607974088542700e-09,-9.098477250826355654e-09,-1.419383033794631677e-08
+1.832136209999999892e+03,-8.153558550123824461e-09,-9.193707614493743455e-09,-9.280039770364175517e-09,-1.418454773141997485e-08
+1.834064769999999953e+03,-8.401936484226867780e-09,-9.537730497694666719e-09,-9.463615749328063331e-09,-1.424146756172246045e-08
+1.835993339999999989e+03,-8.684143416302910558e-09,-9.867582279873043267e-09,-9.661087629700892080e-09,-1.419590332475054175e-08
+1.837921900000000051e+03,-8.968674300879256113e-09,-1.026387321517883479e-08,-9.861460771439322287e-09,-1.421933598993281759e-08
+1.839850470000000087e+03,-9.292333905463329740e-09,-1.064683496407484917e-08,-1.007757546211973335e-08,-1.412582333247587532e-08
+1.841779029999999921e+03,-9.621340592831278899e-09,-1.110682931271774473e-08,-1.029776961373436128e-08,-1.410372711546667848e-08
+1.843707589999999982e+03,-9.996232087520475168e-09,-1.155494021012507024e-08,-1.053601052520822251e-08,-1.394641184112926651e-08
+1.845636160000000018e+03,-1.038070757851806312e-08,-1.209346528585952834e-08,-1.077991796049366692e-08,-1.386215450469281889e-08
+1.847564720000000079e+03,-1.081985234150118609e-08,-1.262247037311095219e-08,-1.104481013191886628e-08,-1.361913888818135326e-08
+1.849493289999999888e+03,-1.127458488760233120e-08,-1.325906843178384439e-08,-1.131753467198169337e-08,-1.344935611971184424e-08
+1.851421849999999949e+03,-1.179566553629255711e-08,-1.388992426425012544e-08,-1.161507411473134778e-08,-1.308981957070884678e-08
+1.853350419999999986e+03,-1.234098955197333558e-08,-1.465087077623625092e-08,-1.192346288980540322e-08,-1.280103184595259137e-08
+1.855278980000000047e+03,-1.296858365167174259e-08,-1.541206881637719151e-08,-1.226178741953361964e-08,-1.228063002586224896e-08
+1.857207550000000083e+03,-1.363316078806781249e-08,-1.633350051325055045e-08,-1.261526124205409198e-08,-1.182372813714084944e-08
+1.859136109999999917e+03,-1.440236090658405634e-08,-1.726474620891978095e-08,-1.300572336895000584e-08,-1.107698690464852309e-08
+1.861064669999999978e+03,-1.522777876434666411e-08,-1.839770817478634378e-08,-1.341763296090907074e-08,-1.037791332072348907e-08
+1.862993240000000014e+03,-1.619030855251850984e-08,-1.955599201384612398e-08,-1.387659205013881971e-08,-9.305142792580814063e-09
+1.864921800000000076e+03,-1.723904673015858464e-08,-2.097496736332602151e-08,-1.436654394812879329e-08,-8.248432856627685706e-09
+1.866850370000000112e+03,-1.847406799428263583e-08,-2.244501664921043591e-08,-1.491849418662622692e-08,-6.692157143787379875e-09
+1.868778929999999946e+03,-1.984396161331745885e-08,-2.426298842148919929e-08,-1.551652218892309452e-08,-5.090402234719560800e-09
+1.870707499999999982e+03,-2.147836801687129522e-08,-2.617639784808807214e-08,-1.619991816722856646e-08,-2.790389460696275549e-09
+1.872636060000000043e+03,-2.333067474579098772e-08,-2.857326801533311604e-08,-1.695451490449988354e-08,-3.238895471684293620e-10
+1.874564630000000079e+03,-2.557988099286792952e-08,-3.114586140518269542e-08,-1.783339267143525585e-08,3.174714903810511304e-09
+1.876493189999999913e+03,-2.819814858313198720e-08,-3.442625623226595225e-08,-1.882826436351322844e-08,7.086725266218057254e-09
+1.878421749999999975e+03,-3.145575867292787549e-08,-3.803769777631292132e-08,-2.001771363571490170e-08,1.263820609605839498e-08
+1.880350320000000011e+03,-3.538250400621264981e-08,-4.276069900240006278e-08,-2.141068618425649458e-08,1.914100662685629588e-08
+1.882278880000000072e+03,-4.044198686430189228e-08,-4.814434714192644408e-08,-2.314007079181195433e-08,2.851125552835098358e-08
+1.884207450000000108e+03,-4.684222635459529802e-08,-5.545477193041463803e-08,-2.526750732826775439e-08,4.013135173797018260e-08
+1.886136009999999942e+03,-5.554065985793900731e-08,-6.422346154537919322e-08,-2.806690368581674088e-08,5.749816328314809145e-08
+1.888064579999999978e+03,-6.737773588167823703e-08,-7.686421204884676947e-08,-3.179001265344927070e-08,8.080609222805591037e-08
+1.889993140000000039e+03,-8.497833364149414111e-08,-9.330968778031341525e-08,-3.720633408690011077e-08,1.183426749567940160e-07
+1.891921710000000076e+03,-1.121986234675656081e-07,-1.196244851707099072e-07,-4.552701277483152646e-08,1.757620186845332447e-07
+1.893850269999999909e+03,-1.607721770141937696e-07,-1.589944559558757647e-07,-6.049907402705368481e-08,2.852624176119917675e-07
+1.895778829999999971e+03,-2.620036374717184202e-07,-2.349534486753140209e-07,-9.341361843269970959e-08,5.119794031247065044e-07
+1.897707400000000007e+03,-5.794208749415073265e-07,-3.486043897089802064e-07,-2.108301047096746659e-07,1.284425588730669894e-06
+1.899635960000000068e+03,-2.298838588770630281e-06,-6.863545633843056611e-07,-9.299600049501783315e-07,5.378419556751145680e-06
+1.901564530000000104e+03,-3.036883703990658348e-06,-3.206961138174450899e-06,-7.015688135454350447e-07,7.139579071703541545e-06
+1.903493089999999938e+03,-3.103374668932457723e-06,-2.850617435531189295e-06,-7.678886050414731133e-07,7.496681152990589754e-06
+1.905421659999999974e+03,-2.605587477596835383e-06,-2.785018760988385265e-06,-3.560119336460648981e-07,7.181655932807363868e-06
+1.907350220000000036e+03,-3.614087544187546193e-06,8.740233786460816982e-07,-1.222225644949550173e-06,1.147109335759997006e-05
+1.909278780000000097e+03,-3.289912754627452296e-06,-4.756827568180209626e-06,-7.564740408107372026e-07,6.467494097823853459e-06
+1.911207349999999906e+03,-2.083193617095248696e-06,-8.522090301475563658e-06,-4.517610331264246488e-07,-1.294078824821760105e-06
+1.913135909999999967e+03,-2.406202755906582197e-06,-8.997457308317368181e-07,-1.117785548691218698e-06,4.808546755159733562e-06
+1.915064480000000003e+03,-1.051882856002820094e-06,-6.112725799613380634e-06,-1.547696607778872519e-07,-2.138093605392542495e-06
+1.916993040000000065e+03,2.536508528118815218e-07,-3.598726619586970171e-06,-4.870387886167805366e-07,-6.880329109014303461e-06
+1.918921610000000101e+03,-7.069906048442228894e-07,5.286540229001430684e-07,-1.317926736410016795e-06,-2.178079564409658524e-06
+1.920850169999999935e+03,-1.203148750932360494e-06,6.431011615501509806e-06,-2.176335494320509675e-06,2.119337924992882820e-06
+1.922778739999999971e+03,-5.925221141224657243e-07,-5.116553983491654030e-07,-9.063979255466993174e-07,-1.902272448364967637e-06
+1.924707300000000032e+03,-1.266710959498371663e-06,1.547401211703939276e-06,-1.202153023973845276e-06,1.833423143266189085e-06
+1.926635860000000093e+03,-7.826209379945528012e-07,-1.665475207769784323e-06,-5.855782856423090601e-07,-7.924838463200975506e-07
+1.928564429999999902e+03,-1.225490520660764557e-06,-1.911350936492799037e-06,-1.020425965591656603e-06,-1.002818783795067908e-06
+1.930492989999999963e+03,-1.222917309977232685e-06,3.594161039418584149e-07,-1.579771079633545824e-06,-1.221613457382812396e-06
+1.932421559999999999e+03,-6.664285136306144130e-07,-4.290109198727255211e-06,-6.910677447271546265e-07,-4.399272548099907017e-06
+1.934350120000000061e+03,-1.586121805244525654e-06,2.806759604981758157e-06,-1.835598827701593717e-06,1.701459392640551734e-06
+1.936278690000000097e+03,-3.458686664087584403e-06,-1.864617057742886906e-06,-1.341425066889462797e-06,7.515844797687866010e-06
+1.938207249999999931e+03,-3.599176693654168032e-06,-5.575284768835830536e-06,-7.189529819607888663e-07,7.185457077330447147e-06
+1.940135819999999967e+03,-3.786284613497430314e-06,-1.128839109801816536e-05,-1.928702245463730683e-07,4.632119929489600988e-06
+1.942064380000000028e+03,-3.213640710881661458e-06,-1.449271220882643945e-05,5.903745030054017818e-07,2.360859243358549244e-06
+1.943992940000000090e+03,-2.766805461284832758e-06,-1.104023834337953900e-05,-1.980714825471470952e-08,1.130252504993605941e-06
+1.945921509999999898e+03,-2.798896758536371644e-06,-1.123314984340456637e-05,7.418478988838063671e-08,1.495948869860577717e-06
+1.947850069999999960e+03,-1.406406346686948523e-06,-9.873184982317377022e-06,3.404770280022374981e-07,-2.133672357215580044e-06
+1.949778639999999996e+03,-9.751304574639422203e-07,-3.825949907222559559e-06,-7.777014874516700256e-07,-2.951246977358856367e-06
+1.951707200000000057e+03,-9.308655592732192194e-07,-1.976495376157960850e-06,-7.227492140835955784e-07,-1.054442361959618289e-06
+1.953635770000000093e+03,-7.936616314791433125e-07,-3.755468961899765236e-06,-4.057004043557791657e-07,-2.036618774831321579e-06
+1.955564329999999927e+03,-1.071151403851213492e-06,-6.193250152250100959e-06,6.185194181340930072e-08,-1.173513960866329095e-06
+1.957492899999999963e+03,-4.492910703442830914e-07,-3.033715324577160589e-06,-9.539914019481165965e-08,-1.465808101348359731e-06
+1.959421460000000025e+03,-8.694666771335281059e-07,2.069983505400048863e-06,-8.153917317479517218e-07,2.309560874202830546e-06
+1.961350020000000086e+03,1.149712124584035059e-06,-9.643888294037578828e-06,1.222750219962339027e-06,-9.320295277191592142e-06
+1.963278589999999895e+03,2.502157247049861309e-07,-4.492958586156698897e-06,-8.272843029197560149e-08,-5.968057341110111559e-06
+1.965207149999999956e+03,-7.262966824570238991e-07,5.988421504690393045e-07,-1.241857299980336796e-06,-1.685333179230295508e-06
+1.967135719999999992e+03,-4.794206674172993164e-08,-4.745380406476772601e-06,-3.072237755113640636e-07,-5.894119977507149936e-06
+1.969064280000000053e+03,-1.345706189995745665e-06,3.208317803612354154e-06,-1.039884789281625299e-06,4.563250036724012867e-06
+1.970992850000000089e+03,-1.831575269489010898e-06,4.134160003024130295e-06,-1.119093120926407385e-06,7.290790069951782135e-06
+1.972921409999999923e+03,-1.941358220120316176e-06,7.936136605675358041e-07,-6.309932460081966683e-07,6.599145047250048031e-06
+1.974849979999999960e+03,-8.840815926354134822e-07,-3.193398200840673030e-06,6.283166253940805867e-08,1.001871614813574341e-06
+1.976778540000000021e+03,-5.876925941044923435e-07,1.240888193476068356e-07,-5.658235501837048567e-07,2.209789403346215342e-07
+1.978707100000000082e+03,-2.244059847180696658e-07,1.318723869653162403e-06,-9.041666270215468467e-07,-1.692934578405015993e-06
+1.980635669999999891e+03,-4.958226674055009715e-07,1.161183095703718973e-06,-6.577019160362236106e-07,4.439821041135468758e-07
+1.982564229999999952e+03,3.865750956951178060e-07,-4.117208806370382219e-06,3.926428505881364957e-07,-4.090325806462676765e-06
+1.984492799999999988e+03,4.171173392459142590e-07,-5.745460964165111862e-06,4.629819538198095443e-07,-5.542259211441780855e-06
+1.986421360000000050e+03,-1.078117287674354720e-06,2.673270799229655562e-06,-1.051551289532441132e-06,2.790970630252636066e-06
+1.988349930000000086e+03,-1.069663227609473257e-06,-4.586664090903002375e-07,-7.975202254964791301e-07,7.470547233014814617e-07
+1.990278489999999920e+03,-2.022918253195508096e-06,-8.191958844469943491e-07,-9.742272497099800344e-07,3.826997089225915419e-06
+1.992207059999999956e+03,-1.120786005181228079e-06,-6.394165134405218510e-06,-1.343856689880848274e-07,-2.023949030694338731e-06
+1.994135620000000017e+03,-6.414207305248789312e-07,-8.572417402040559002e-06,1.453406773520886176e-07,-5.086695379933577910e-06
+1.996064180000000079e+03,-4.009853021818189546e-07,-4.517561736748870999e-06,-2.802900598073264575e-07,-3.982825207864503711e-06
+1.997992749999999887e+03,-2.138283503628697085e-07,-4.613252440689941161e-06,-2.420065036367733779e-07,-4.738094875036328125e-06
+1.999921309999999949e+03,-2.857535468676053922e-07,-3.634605975919955361e-06,-5.828892766625207108e-07,-4.951056613344880444e-06
+2.001849879999999985e+03,-4.113285630093240790e-07,-3.195909087352324419e-06,-2.630761389043766712e-07,-2.539081319290053373e-06
+2.003778440000000046e+03,-6.735149893853005103e-07,-1.845064614089819255e-06,-7.765132206425024330e-07,-2.301395083958823249e-06
+2.005707010000000082e+03,-6.422559819501081363e-07,-9.416585817931090257e-06,1.415996156336751189e-07,-5.943737898226197173e-06
+2.007635569999999916e+03,-1.339552929320173463e-06,-5.035152510693755114e-06,-4.566888288058760718e-07,-1.123650488759809415e-06
+2.009564139999999952e+03,-1.205917079781747651e-07,-6.135085070952875832e-06,-6.606820508913257120e-08,-5.893520382039630995e-06
+2.011492700000000013e+03,-1.113534586214603743e-06,1.950647898805694681e-06,-1.731310457187423165e-06,-7.863889418638227410e-07
+2.013421260000000075e+03,-4.523914826233274354e-07,-1.896429935257232072e-06,-1.773254117937595095e-06,-7.748470884389797213e-06
+2.015349830000000111e+03,1.549465141650045344e-07,-2.292656313199450752e-06,-2.057065261792694776e-06,-1.209290589765983992e-05
+2.017278389999999945e+03,-9.892887540221177968e-07,2.244785783585660895e-06,-3.332666867011858952e-06,-8.137478283755572564e-06
+2.019206959999999981e+03,-1.769617792581495024e-06,3.516847736589211248e-06,-3.477188197332754558e-06,-4.048489994198898783e-06
+2.021135520000000042e+03,-1.463488291284921428e-07,-3.705849133755698641e-06,-1.955398564271719943e-06,-1.172078789122668538e-05
+2.023064090000000078e+03,-1.113728148472572664e-06,1.538545299723914660e-06,-2.174100955982245071e-06,-3.159403544454613514e-06
+2.024992649999999912e+03,-4.435927001881413873e-07,-1.670132711842568317e-06,-1.540210688345747103e-06,-6.528664705009898465e-06
+2.026921219999999948e+03,9.506992068875907522e-08,-3.706217009879691526e-06,-1.113089793177432769e-06,-9.058931160170613771e-06
+2.028849780000000010e+03,-1.095703619753868690e-06,5.048340730126056033e-06,-2.558413967230116288e-06,-1.432152109399468835e-06
+2.030778340000000071e+03,5.233960883462646720e-07,-3.889986234124799993e-06,-1.151611487205511972e-06,-1.131105535983601258e-05
+2.032706910000000107e+03,1.448793414393957394e-06,-8.610932091315525334e-06,-1.229988200235696288e-06,-2.047919097265360982e-05
+2.034635469999999941e+03,8.195930914801832805e-07,-7.808813849666063764e-06,-1.533156591673559297e-06,-1.823259836803008973e-05
+2.036564039999999977e+03,9.689040516679315146e-08,4.591524207694072598e-06,-3.839037611165485846e-06,-1.284648282544030595e-05
+2.038492600000000039e+03,8.333067693851357376e-08,1.365119284005416492e-06,-3.381407096779361628e-06,-1.398529398964984692e-05
+2.040421170000000075e+03,-6.871660383024946355e-07,7.225782739863256683e-06,-4.624844497490386456e-06,-1.021997957606608721e-05
+2.042349729999999909e+03,-4.144331642695218360e-07,5.105131930892696534e-06,-4.662263322306231170e-06,-1.371474786976242712e-05
+2.044278299999999945e+03,6.359507972522392710e-07,2.419011492057472687e-06,-4.733160772098621165e-06,-2.136867083330935892e-05
+2.046206860000000006e+03,-4.889231764151803921e-07,1.738795676897570709e-06,-4.979900756672435899e-06,-1.815834123851583221e-05
+2.048135420000000067e+03,-1.516452194938792895e-06,1.767047815008882092e-06,-5.493078144895187930e-06,-1.585127015110660503e-05
+2.050063990000000103e+03,-5.911306582058623362e-07,2.946708954850079054e-06,-5.935261795587774966e-06,-2.073029834125866965e-05
+2.051992549999999937e+03,-8.165805729386346710e-07,4.605304018570720366e-06,-6.784992232399020314e-06,-2.183755877323828243e-05
+2.053921119999999974e+03,-3.966536649848665406e-07,4.288486145720542692e-06,-7.784497225488210478e-06,-2.844312567064704740e-05
+2.055849679999999807e+03,-7.169653806570050927e-07,9.633728821850436351e-06,-8.949620362631226529e-06,-2.684079380186706656e-05
+2.057778249999999844e+03,6.028152757534235312e-07,1.292217446076433990e-06,-6.774324200626799507e-06,-3.139197025749037732e-05
+2.059706810000000132e+03,1.293005586859622912e-06,2.160449994078305633e-06,-7.845920976107214454e-06,-3.832928076802524884e-05
+2.061635369999999966e+03,-9.244747534392761325e-08,3.572998882690906881e-06,-7.315079264249056291e-06,-2.842664730241218374e-05
+2.063563940000000002e+03,-9.127650027488458824e-08,5.279972575771385699e-06,-7.727877886832275713e-06,-2.855375307557429112e-05
+2.065492499999999836e+03,-1.723737327415452184e-06,2.606280240042756780e-06,-8.227426239399123820e-06,-2.620811182146971731e-05
+2.067421069999999872e+03,-1.383469565503448640e-06,-3.430827691594424759e-07,-8.011327812224115967e-06,-2.970760321804549286e-05
+2.069349630000000161e+03,1.280561064379240601e-07,5.071328498294119360e-06,-8.080624015288484762e-06,-3.129697425049553791e-05
+2.071278200000000197e+03,4.147082866212712064e-07,3.866617936464614738e-06,-7.757832525948623332e-06,-3.234157072369618852e-05
+2.073206760000000031e+03,-6.145089917582081565e-08,1.322071072374930858e-05,-9.349990172854660245e-06,-2.793187451405001629e-05
+2.075135330000000067e+03,3.926220828442457454e-07,7.757316503370260629e-06,-7.999387109882464918e-06,-2.942322000991296667e-05
+2.077063889999999901e+03,1.130069957066130122e-07,7.454682937514679460e-06,-8.465649265121266511e-06,-3.055278762353476709e-05
+2.078992450000000190e+03,-1.991921270199648432e-06,1.239650647740667525e-05,-1.028136916870435481e-05,-2.432963540199367208e-05
+2.080921020000000226e+03,-1.412066412521868565e-06,1.041420203120473254e-05,-9.792359944164206662e-06,-2.671442860891736209e-05
+2.082849580000000060e+03,1.226356871711389471e-06,6.869027998647244057e-06,-8.970878585431861952e-06,-3.830950750360859777e-05
+2.084778150000000096e+03,5.744440042251579671e-09,1.112210463361292402e-05,-8.725817585878952649e-06,-2.756281017845940023e-05
+2.086706709999999930e+03,9.729513529825816921e-07,6.047938480587650259e-06,-8.460106974431424160e-06,-3.574493394361304068e-05
+2.088635279999999966e+03,-3.092718958300746143e-07,9.015619661800356119e-06,-8.313692137196953242e-06,-2.644771602064142856e-05
+2.090563839999999800e+03,4.957310457153693369e-07,1.288894144989250535e-05,-8.649221004874712803e-06,-2.762748504829062393e-05
+2.092492409999999836e+03,4.422026266827878845e-07,1.744477988030746968e-05,-9.537143366924916464e-06,-2.676840310995822335e-05
+2.094420970000000125e+03,1.884203401627044144e-06,9.675816240445694557e-06,-8.609660856112349826e-06,-3.681692396513850453e-05
+2.096349529999999959e+03,-3.834432921802760619e-07,1.264704768966423888e-05,-8.985342109836430997e-06,-2.546339829871966924e-05
+2.098278099999999995e+03,4.944917641974995714e-07,7.245027754623745504e-06,-8.663134909809997713e-06,-3.332755326960205644e-05
+2.100206659999999829e+03,-1.368393503199396150e-06,1.490962234356074491e-05,-9.750225547118908045e-06,-2.222582462749998021e-05
+2.102135229999999865e+03,-4.499936070594358285e-08,1.432631784970847382e-05,-9.131733769049037443e-06,-2.593217718968199602e-05
+2.104063790000000154e+03,7.792483909885911871e-07,2.034710775718112153e-05,-9.914103456437995144e-06,-2.702945602890390050e-05
+2.105992360000000190e+03,-1.895926946607054428e-07,2.205527202168122331e-05,-8.985394630162384455e-06,-1.691425571786941005e-05
+2.107920920000000024e+03,2.348745385114397146e-06,1.606973298853459244e-05,-8.387552762322962144e-06,-3.149710304809144270e-05
+2.109849490000000060e+03,-1.049048988813143022e-06,2.511697870320627515e-05,-1.025747610619528936e-05,-1.568067211019696428e-05
+2.111778049999999894e+03,3.192594366196146117e-09,1.665045845941450346e-05,-8.508796226217237938e-06,-2.106164407482152251e-05
+2.113706610000000182e+03,9.253034809003687903e-07,1.620919326319579122e-05,-8.706488724221629302e-06,-2.646416344395258880e-05
+2.115635180000000219e+03,1.014344361545085242e-06,1.662379396251457579e-05,-8.451158249172242596e-06,-2.531282185284589050e-05
+2.117563740000000053e+03,1.122989310273777418e-06,2.000585133734429194e-05,-9.552784830081423231e-06,-2.729283496260143173e-05
+2.119492310000000089e+03,-5.739368593883093416e-07,3.968651307486168242e-05,-1.377070081336485988e-05,-1.878134042478161761e-05
+2.121420869999999923e+03,-5.942795712096635018e-07,2.245702419459482272e-05,-1.051150346016677012e-05,-2.148092873726658412e-05
+2.123349439999999959e+03,-1.523820336643162067e-06,3.403916239425038113e-05,-1.262140091113619146e-05,-1.512832423298664884e-05
+2.125277999999999793e+03,-6.160048813214301912e-07,2.661636962936212572e-05,-1.081473162889833598e-05,-1.856877298891885779e-05
+2.127206569999999829e+03,-9.184146612352294105e-07,2.947224368678119809e-05,-1.133666557705813630e-05,-1.668549395202151785e-05
+2.129135130000000117e+03,-2.658406555363138896e-07,2.835114777360264011e-05,-1.193184238767879227e-05,-2.333471116729021204e-05
+2.131063689999999951e+03,-1.140236961903941953e-06,2.888107761530423574e-05,-1.148662357860448849e-05,-1.695826747456798247e-05
+2.132992259999999987e+03,-1.871793099598497678e-06,2.690965601058955899e-05,-1.099744563672736233e-05,-1.352126459163300341e-05
+2.134920819999999821e+03,-1.256152164049327860e-06,2.747603524049198464e-05,-1.082719816760719651e-05,-1.492818730421341945e-05
+2.136849389999999858e+03,-1.168607171548700097e-06,1.869138601557079356e-05,-9.350804261160530114e-06,-1.755958448060742936e-05
+2.138777950000000146e+03,-1.457847837302414939e-06,3.132106500541676717e-05,-1.238599336983216462e-05,-1.709574492215634340e-05
+2.140706520000000182e+03,-7.819313288593262683e-07,2.416608036015715306e-05,-1.035193611780554060e-05,-1.823352911549675078e-05
+2.142635080000000016e+03,-8.560553029175220847e-07,2.478489590766191913e-05,-1.082962634719635707e-05,-1.940270134866887395e-05
+2.144563650000000052e+03,-1.102902631340669846e-06,3.459652348854129169e-05,-1.225954372965763958e-05,-1.483262895817944763e-05
+2.146492209999999886e+03,-1.768239336258079541e-06,3.194373576428997090e-05,-1.213381165637615517e-05,-1.398061098967321287e-05
+2.148420770000000175e+03,-1.673001043270033241e-06,3.283469540783960704e-05,-1.199058325864002663e-05,-1.287703267508960906e-05
+2.150349340000000211e+03,-3.290143193282080965e-06,3.469233884306714287e-05,-1.180658842686466638e-05,-3.039507690779461340e-06
+2.152277900000000045e+03,-1.800637948473726023e-06,3.288904694781964483e-05,-1.130057077951255218e-05,-9.200110891080696011e-06
+2.154206470000000081e+03,-1.465236226843182631e-06,3.162192210965217222e-05,-1.051915045461729142e-05,-8.491164137398641597e-06
+2.156135029999999915e+03,-6.525249925085682419e-07,3.436979527605927643e-05,-1.114911895704574460e-05,-1.213503881085115443e-05
+2.158063599999999951e+03,-1.243426123476679467e-06,2.667179889472563763e-05,-9.899794510940131454e-06,-1.167997283372516863e-05
+2.159992159999999785e+03,-1.775168387395031555e-06,3.054030355127466771e-05,-1.110469957535583981e-05,-1.079389509169477897e-05
+2.161920729999999821e+03,-3.622335107267482425e-06,3.541387586592010297e-05,-1.200174467455700618e-05,-1.710838397546349427e-06
+2.163849290000000110e+03,-2.511936157325382428e-06,3.644530738692853378e-05,-1.247281452944988875e-05,-7.686055378990336212e-06
+2.165777849999999944e+03,-1.833805250457919890e-06,3.128827495193444613e-05,-1.036167517974464964e-05,-6.494188341978298878e-06
+2.167706419999999980e+03,-1.534981294551414670e-06,3.200604173031311190e-05,-9.744804776779578449e-06,-4.367326641726854288e-06
+2.169634979999999814e+03,-1.132951647837320268e-06,3.082379092338026927e-05,-9.156869436650944856e-06,-4.725928038454418985e-06
+2.171563549999999850e+03,-5.318991722931881784e-07,2.878235736428796902e-05,-8.799840573054754450e-06,-7.848500643723790724e-06
+2.173492110000000139e+03,-1.291469016271405543e-06,3.151947008677321958e-05,-9.647870832483161629e-06,-5.503309048955678579e-06
+2.175420680000000175e+03,-1.880516024921622387e-06,3.128236938711495394e-05,-9.730022913907348910e-06,-3.494627491075470057e-06
+2.177349240000000009e+03,-2.052658592657573686e-06,3.989987690593696854e-05,-1.075167863505516854e-05,1.359138342820961274e-06
+2.179277810000000045e+03,-7.508843366928756146e-07,3.931468688574163455e-05,-1.139527520463160222e-05,-7.844956798879227448e-06
+2.181206369999999879e+03,3.911816886670094036e-08,2.726433205854224173e-05,-8.032027009248457171e-06,-8.494626387190372410e-06
+2.183134930000000168e+03,-2.925885164429827382e-07,2.893626714300639782e-05,-8.139868341035294189e-06,-5.830862795444660298e-06
+2.185063500000000204e+03,-5.617408508749226841e-07,3.170331979540344020e-05,-8.344243225900342738e-06,-2.776815661327239945e-06
+2.186992060000000038e+03,5.727038885151287861e-08,2.617314856000799953e-05,-8.034832240273225495e-06,-9.678661222584730050e-06
+2.188920630000000074e+03,-1.994509890565515415e-06,3.484365835441893247e-05,-9.468950099118106706e-06,1.728382774013366842e-06
+2.190849189999999908e+03,-1.375883279174233028e-06,1.877450639547012615e-05,-6.441571134845602289e-06,-3.668866574845719004e-06
+2.192777759999999944e+03,-1.867784369531004193e-06,2.135556352474195381e-05,-6.718944883345980377e-06,-1.373527094323069309e-07
+2.194706319999999778e+03,-2.163541004436183638e-06,1.148987732989280928e-05,-5.251493660583375213e-06,-2.191201163524123623e-06
+2.196634880000000067e+03,-9.022023318624212106e-07,1.707916569933180576e-05,-6.546816208888503757e-06,-7.929121057556638363e-06
+2.198563450000000103e+03,-3.291229583579392440e-07,1.856496294306624821e-05,-6.948041260567546349e-06,-1.075994935886872609e-05
+2.200492009999999937e+03,-1.714422406433171605e-06,2.201882248703352634e-05,-7.977561674442362280e-06,-5.729821835689286909e-06
+2.202420579999999973e+03,-1.598671984220697457e-06,1.890509087340484605e-05,-7.087493405957684265e-06,-5.412962241057356229e-06
+2.204349139999999807e+03,-6.302097285882166792e-07,1.601659226892900668e-05,-6.389470509688316806e-06,-9.499634041547309272e-06
+2.206277709999999843e+03,-3.068568402954499916e-06,2.514937769420490056e-05,-7.715898848486716304e-06,4.559524257299786491e-06
+2.208206270000000131e+03,-2.898232077334754034e-06,2.027407941021508035e-05,-7.084759208073107161e-06,1.725800771152674935e-06
+2.210134840000000167e+03,-2.318561999056977818e-06,1.874920557502336667e-05,-7.498678267698368425e-06,-4.201138930818950285e-06
+2.212063400000000001e+03,-2.063783380808914241e-06,1.730126435921587635e-05,-7.280767543962427979e-06,-5.812422210081750882e-06
+2.213991959999999835e+03,-2.976287523562185024e-06,2.194834384418364924e-05,-7.908091255790904178e-06,9.814033137061549442e-08
+2.215920529999999872e+03,-3.123825384202739267e-06,1.522436297454559089e-05,-6.772951214119224598e-06,-9.429758646878788669e-07
+2.217849090000000160e+03,-3.058133343901282369e-06,8.349820273837028044e-06,-6.364588442517526348e-06,-6.299326515728010973e-06
+2.219777660000000196e+03,-3.418329419398102144e-06,6.511664866055900025e-06,-5.240184709537512436e-06,-1.560008505757633630e-06
+2.221706220000000030e+03,-3.668505376358804983e-06,1.204386611834315266e-05,-5.556892308233167576e-06,3.677426370801747055e-06
+2.223634790000000066e+03,-3.574452546164624512e-06,1.165811215013455251e-05,-6.124445101797171707e-06,3.604492012584391639e-07
+2.225563349999999900e+03,-3.544160479023745494e-06,9.238784158641296992e-06,-6.125921831383637497e-06,-2.199629459064861449e-06
+2.227491919999999936e+03,-3.978330743077082451e-06,1.636093083806095395e-05,-6.459008143000262486e-06,5.370366537266592950e-06
+2.229420480000000225e+03,-4.200773639582165176e-06,1.284241603957284363e-05,-5.368948511594481460e-06,7.666853491286164342e-06
+2.231349040000000059e+03,-5.213204899906326523e-06,1.592061955991454147e-05,-6.284082803274358296e-06,1.117612821427214543e-05
+2.233277610000000095e+03,-1.871219648598386733e-06,3.692658715604646929e-06,-3.919455342969088188e-06,-5.381986017668810317e-06
+2.235206169999999929e+03,-2.999728048649439161e-06,1.153206681762279400e-05,-4.526988901282952518e-06,4.765584966546770404e-06
+2.237134739999999965e+03,-1.035726521975890220e-06,2.818164867896931344e-06,-2.876130235688099039e-06,-5.335686719415931511e-06
+2.239063299999999799e+03,-2.664102499709747434e-06,6.823377554441877891e-06,-4.080386210283036577e-06,5.485764901417021325e-07
+2.240991869999999835e+03,-4.927838375174640023e-06,1.340329588488861206e-05,-4.637470083818161900e-06,1.468976359615328080e-05
+2.242920430000000124e+03,-4.002343405762468143e-06,1.026990610042966532e-05,-4.457867574642279278e-06,8.251720394866132047e-06
+2.244849000000000160e+03,-4.417490874927232766e-06,8.403953370780708115e-06,-5.424156091937213740e-06,3.943954340973803944e-06
+2.246777559999999994e+03,-6.017840045100468805e-06,5.820344434342732428e-06,-5.626953652860935812e-06,7.552154474756353950e-06
+2.248706119999999828e+03,-6.151812980149145758e-06,6.732558627841321912e-06,-6.046996711977386564e-06,7.196943853887520504e-06
+2.250634689999999864e+03,-4.562170213437924895e-06,-5.386859603099338475e-06,-4.541023984360855504e-06,-5.293171890864741742e-06
+2.252563250000000153e+03,-4.803649318883327904e-06,-1.797338138813002123e-06,-4.520890954003384954e-06,-5.445859708379477519e-07
+2.254491820000000189e+03,-4.252013390629381675e-06,-7.701281133919844242e-06,-3.556874347607870229e-06,-4.621489158325930214e-06
+2.256420380000000023e+03,-3.463102882688666592e-06,-1.392789479219240337e-05,-2.197913424661906431e-06,-8.322512128746971562e-06
+2.258348950000000059e+03,-4.839186125479666859e-06,7.646886176359181188e-06,-6.697411812380369990e-06,-5.859251105507573421e-07
+2.260277509999999893e+03,-5.017212924863181509e-06,2.464286354328988134e-06,-5.656535606697436509e-06,-3.682129637497248903e-07
+2.262206079999999929e+03,-5.162658495468596871e-06,-1.184308669757225258e-06,-5.042747721837634070e-06,-6.530477053166656769e-07
+2.264134640000000218e+03,-6.518927380520728930e-06,4.680423342789394345e-06,-5.344696778476797182e-06,9.882815615208188898e-06
+2.266063200000000052e+03,-7.132989281213331721e-06,-2.507347892132130991e-06,-3.604071066383967878e-06,1.312741483579357290e-05
+2.267991770000000088e+03,-5.165741225531851441e-06,-4.627554818163084934e-06,-4.075189588705741385e-06,2.041003935323440119e-07
+2.269920329999999922e+03,-5.552144543430117475e-06,3.964672998005742051e-06,-5.635383923910429649e-06,3.595883503831493001e-06
+2.271848899999999958e+03,-4.229263831390408584e-06,-4.276813383342635226e-06,-4.015991846122341657e-06,-3.331918465640180921e-06
+2.273777459999999792e+03,-6.712455567392754746e-06,-4.778590187006870662e-06,-4.198124564337050761e-06,6.361075358952573825e-06
+2.275706029999999828e+03,-5.647718859328803005e-06,-1.268556182066451805e-08,-5.257714038426721612e-06,1.715218704117685050e-06
+2.277634590000000117e+03,-6.136906725028353790e-06,-8.715121971092591261e-07,-5.187313128308399248e-06,3.335632788650053550e-06
+2.279563160000000153e+03,-7.288798081442434657e-06,-9.443127133033776197e-07,-5.705112851840660662e-06,6.072155590352540316e-06
+2.281491719999999987e+03,-6.053409559921209298e-06,-1.495917158018925902e-05,-4.040621483959690036e-06,-6.041576421136211169e-06
+2.283420279999999821e+03,-6.139537518805309143e-06,-8.387469784205722526e-06,-5.346444714829404031e-06,-4.873696708003066202e-06
+2.285348849999999857e+03,-6.568235152659217468e-06,-1.351847063679999216e-05,-5.069662538047789794e-06,-6.879091134730727855e-06
+2.287277410000000145e+03,-5.901723206554255452e-06,-1.646217416827382713e-05,-4.199545208286973779e-06,-8.920727327208037764e-06
+2.289205980000000181e+03,-6.988583171277879677e-06,-1.305028364828749758e-05,-4.913853743958821917e-06,-3.858259252690355536e-06
+2.291134540000000015e+03,-8.319136338932193637e-06,-7.864655433066664741e-06,-6.930978666093733209e-06,-1.714465906832972251e-06
+2.293063110000000052e+03,-7.620109783592657644e-06,-1.909729568535174950e-05,-4.458275712272798963e-06,-5.088887872889124283e-06
+2.294991669999999885e+03,-5.951341385506697413e-06,-2.481139660005602244e-05,-4.584039299621959362e-06,-1.875360710514151395e-05
+2.296920239999999922e+03,-6.676404351934306506e-06,-2.666875454734526579e-05,-4.460041378121913911e-06,-1.684922711570936105e-05
+2.298848800000000210e+03,-7.613314379656999605e-06,-1.957397429783487840e-05,-5.269725532075567619e-06,-9.190776577419513613e-06
+2.300777360000000044e+03,-7.349468688905482904e-06,-3.002437176339949653e-05,-4.518046815753539014e-06,-1.747984494966880559e-05
+2.302705930000000080e+03,-8.828355236039896813e-06,-2.429205063130065610e-05,-6.731775812808274837e-06,-1.500322050632630784e-05
+2.304634489999999914e+03,-8.216567897130455081e-06,-2.853462449093431804e-05,-4.662796783527433374e-06,-1.278975176561779891e-05
+2.306563059999999950e+03,-9.224483232552866554e-06,-2.719597634164819090e-05,-5.579732190479310751e-06,-1.104801986430165214e-05
+2.308491619999999784e+03,-5.845423594249079153e-06,-3.394597396389700833e-05,-4.383222919277048004e-06,-2.746773921259774943e-05
+2.310420189999999820e+03,-7.861792991644339168e-06,-4.270289885596211302e-05,-2.061575241274465525e-06,-1.700521396310864487e-05
+2.312348750000000109e+03,-9.534933639182181244e-06,-3.964759746811503661e-05,-3.196437378905325191e-06,-1.156508632778106484e-05
+2.314277320000000145e+03,-9.438853154628395597e-06,-4.121158063925231167e-05,-2.162087297764172791e-06,-8.972095144617709151e-06
+2.316205879999999979e+03,-1.045055235275813970e-05,-4.434148288894097941e-05,-2.483203488492185595e-06,-9.042390793254706174e-06
+2.318134439999999813e+03,-4.144608790463835247e-06,-5.459573932536715743e-05,1.131421148323789287e-06,-3.122045227798356102e-05
+2.320063009999999849e+03,-6.523531618216929813e-06,-4.582487376915728199e-05,-1.058731911694398194e-06,-2.161324811909976415e-05
+2.321991570000000138e+03,-4.550696375257657667e-06,-5.767832060645472719e-05,-1.811600619602171675e-07,-3.831922545871861984e-05
+2.323920140000000174e+03,-7.703190522548925128e-06,-4.824933869108133686e-05,-2.289636832793365207e-06,-2.426475692929984130e-05
+2.325848700000000008e+03,-4.896593486259400592e-06,-5.919382639747618728e-05,1.167697169628652244e-06,-3.232617468496087486e-05
+2.327777270000000044e+03,-3.994195580321328168e-06,-7.048203961908173132e-05,6.238717487619388282e-07,-5.002183551222806222e-05
+2.329705829999999878e+03,-6.146176492683067250e-06,-5.901080085227947022e-05,-4.400359236827269742e-07,-3.372992199438699446e-05
+2.331634399999999914e+03,-5.920493371838493257e-06,-6.527511386986597065e-05,-3.872760323887265707e-07,-4.076036601858302593e-05
+2.333562960000000203e+03,-6.246090733446270697e-06,-7.206498767166281873e-05,1.414485606956145036e-06,-3.812504173070975391e-05
+2.335491520000000037e+03,-5.600294419004821906e-06,-7.170771008382741379e-05,9.306072818993341380e-07,-4.277275260480286299e-05
+2.337420090000000073e+03,-7.058005801857102677e-06,-5.576668302719860339e-05,-1.099591084728184354e-06,-2.936811137840914451e-05
+2.339348649999999907e+03,-2.563591702696058299e-06,-7.496792308826386942e-05,2.827259936548298356e-06,-5.108392205733877130e-05
+2.341277219999999943e+03,-5.631408525930149216e-06,-6.629282200629709040e-05,4.146374032212489384e-07,-3.950600298986544636e-05
+2.343205779999999777e+03,-7.816965714074852097e-06,-5.634612029816732088e-05,-3.924885877397774945e-06,-3.910238126537358082e-05
+2.345134349999999813e+03,-1.026541511521482861e-05,-5.645653573460851358e-05,-5.498181534267409436e-06,-3.533545517414091170e-05
+2.347062910000000102e+03,-8.822157479252880436e-06,-6.497774805362320721e-05,-2.909962244003266086e-06,-3.878395038615014022e-05
+2.348991469999999936e+03,-6.501063327700065061e-06,-6.035086280557005550e-05,-2.462889615447467051e-06,-4.245985938704250750e-05
+2.350920039999999972e+03,-5.859820603008575873e-06,-6.979481277831869109e-05,8.787881105169455008e-07,-3.993961582034709357e-05
+2.352848599999999806e+03,-8.081482686582365350e-06,-6.110782710976405720e-05,-2.070347730029779592e-06,-3.447568007493002315e-05
+2.354777169999999842e+03,-8.261262218495436300e-06,-6.252532212586932911e-05,-3.184069816072856186e-06,-4.003097861789928972e-05
+2.356705730000000131e+03,-1.100314524527456940e-05,-6.256950872402841483e-05,-4.566966934584392780e-06,-3.405422028821286520e-05
+2.358634300000000167e+03,-8.202562445007811410e-06,-6.034198388145381778e-05,-3.463924151319471639e-06,-3.934759385451965804e-05
+2.360562860000000001e+03,-9.484555176351203398e-06,-5.498905603779662068e-05,-4.121608746920114761e-06,-3.122868817367887645e-05
+2.362491430000000037e+03,-9.796304759092210255e-06,-5.355951645677164258e-05,-5.338143400728273495e-06,-3.380777079490812165e-05
+2.364419989999999871e+03,-6.639178409937863495e-06,-5.250086528349505124e-05,-4.056294167175983101e-06,-4.105747673468088999e-05
+2.366348550000000159e+03,-6.673926883857708066e-06,-4.560426621040017880e-05,-5.573022165568504462e-06,-4.072674199230552470e-05
+2.368277120000000195e+03,-5.745802754943350484e-06,-4.818156509517508568e-05,-3.764824445392229184e-06,-3.940490211986247862e-05
+2.370205680000000029e+03,-8.725845626080842176e-06,-3.245151525601763982e-05,-6.044109067686212982e-06,-2.057016458795420165e-05
+2.372134250000000065e+03,-8.282384368869987265e-06,-4.883044455907592426e-05,-4.686607197059970680e-06,-3.289946529537548278e-05
+2.374062809999999899e+03,-8.659095261940859094e-06,-5.201062745913450069e-05,-4.016374290540685597e-06,-3.144119615444321254e-05
+2.375991379999999936e+03,-8.105331769695454361e-06,-4.360958316256602270e-05,-4.185336293031506047e-06,-2.624216475240421779e-05
+2.377919940000000224e+03,-8.207817576373859823e-06,-4.358516008583361069e-05,-4.837846580828934038e-06,-2.865460808439422623e-05
+2.379848509999999806e+03,-1.063610277771879970e-05,-5.116209833453172940e-05,-4.993182057283866501e-06,-2.616131305541985662e-05
+2.381777070000000094e+03,-8.332318581392353493e-06,-4.362167093943637529e-05,-5.559492859079900958e-06,-3.133675255508081914e-05
+2.383705629999999928e+03,-1.014848674769950416e-05,-3.963422334070113099e-05,-5.937413689459435860e-06,-2.097719473094981937e-05
+2.385634199999999964e+03,-1.134710359428210715e-05,-4.374604278040654094e-05,-6.128580766254066655e-06,-2.062553920409246428e-05
+2.387562759999999798e+03,-1.228287388538550141e-05,-4.373862049924982803e-05,-6.358991359543527609e-06,-1.749304265320079899e-05
+2.389491329999999834e+03,-1.196577406116132726e-05,-4.282084300711234525e-05,-6.118490342762510773e-06,-1.691463380230391142e-05
+2.391419890000000123e+03,-1.116020792750135283e-05,-4.416913435544148259e-05,-6.082380567557665223e-06,-2.167197768786261776e-05
+2.393348460000000159e+03,-1.293551833908389332e-05,-5.043902590537597131e-05,-4.718596624136361772e-06,-1.403420903337119046e-05
+2.395277019999999993e+03,-1.159125546484907652e-05,-4.174675504650160912e-05,-6.036549752876355309e-06,-1.713680362705606819e-05
+2.397205590000000029e+03,-1.012401107788582136e-05,-3.573963870817664385e-05,-5.589121665849043500e-06,-1.564795178365949651e-05
+2.399134149999999863e+03,-1.082725648066092983e-05,-3.788170592174207367e-05,-4.937995379831612983e-06,-1.178951722568832826e-05
+2.401062710000000152e+03,-1.056732712752297198e-05,-3.765410726631582717e-05,-5.997087203107425795e-06,-1.740580099283500727e-05
+2.402991280000000188e+03,-1.160204958526089867e-05,-3.314151647638419580e-05,-6.555527369815213126e-06,-1.078305628080995318e-05
+2.404919840000000022e+03,-1.471046512611702262e-05,-4.173606185300876646e-05,-6.052762045115167844e-06,-3.378376806221548305e-06
+2.406848410000000058e+03,-1.272618214023417944e-05,-3.969929440935898686e-05,-5.448842715218505147e-06,-7.457267738814291119e-06
+2.408776969999999892e+03,-1.366357993570135904e-05,-3.689023622591911634e-05,-6.967061367965160064e-06,-7.221518353757568688e-06
+2.410705539999999928e+03,-1.202262078511217956e-05,-3.627544066032220425e-05,-6.698242703314743138e-06,-1.268594866448791754e-05
+2.412634100000000217e+03,-1.307396415286078207e-05,-5.241355272708142450e-05,-6.306677951084092017e-06,-2.243130104662979319e-05
+2.414562669999999798e+03,-1.396225919339542952e-05,-3.297172240877699068e-05,-9.492848916348927570e-06,-1.317013876149102057e-05
+2.416491230000000087e+03,-1.289230107668640701e-05,-3.033843780691208514e-05,-8.171791993202931641e-06,-9.424368683649361647e-06
+2.418419789999999921e+03,-1.152715246054130600e-05,-5.258798498866810620e-05,-4.243119775907664761e-06,-2.031630403892714895e-05
+2.420348359999999957e+03,-1.134900194213129492e-05,-3.850607818629024002e-05,-6.759041996318524497e-06,-1.817040296947725541e-05
+2.422276919999999791e+03,-1.182690547884305525e-05,-3.176320049181852141e-05,-6.480414629764280636e-06,-8.075738566205541819e-06
+2.424205489999999827e+03,-1.049777093710721449e-05,-3.642827878912508377e-05,-6.818120315525240148e-06,-2.012570080691465077e-05
+2.426134050000000116e+03,-1.279993781847882499e-05,-3.930632054919860039e-05,-8.058389553238911053e-06,-1.829903798353607432e-05
+2.428062620000000152e+03,-1.104306672390139539e-05,-3.272744786238084171e-05,-8.730232459532710009e-06,-2.248050736926730168e-05
+2.429991179999999986e+03,-1.029903113005359860e-05,-3.827919850795419868e-05,-7.008140468201360613e-06,-2.369900947285805969e-05
+2.431919750000000022e+03,-1.158595002332794171e-05,-2.958498927038104022e-05,-6.857725496323229207e-06,-8.636737113833980263e-06
+2.433848309999999856e+03,-1.060765463841058321e-05,-2.927982478816359440e-05,-8.243321243167506273e-06,-1.880471899256952716e-05
+2.435776870000000145e+03,-1.020941879939185368e-05,-2.760704070743365851e-05,-8.069406397496266015e-06,-1.812578211723599650e-05
+2.437705440000000181e+03,-1.141096828266655693e-05,-3.061279815712856963e-05,-7.775562526302441104e-06,-1.450624567834392165e-05
+2.439634000000000015e+03,-1.156555952635167516e-05,-3.658115785828234818e-05,-7.400393435107546418e-06,-1.812751864234700668e-05
+2.441562570000000051e+03,-1.269254046062303238e-05,-3.576348381761768600e-05,-8.187671746130545752e-06,-1.580480266270422614e-05
+2.443491129999999885e+03,-1.354637752548160696e-05,-2.864030446737886708e-05,-7.840934838426871705e-06,-3.362517553806852279e-06
+2.445419699999999921e+03,-1.278724219684675376e-05,-3.641180782086903640e-05,-7.308378197976007886e-06,-1.213787075966108443e-05
+2.447348260000000209e+03,-1.139601345999300514e-05,-3.779548266092040660e-05,-7.491267029438865877e-06,-2.049562467671355078e-05
+2.449276829999999791e+03,-1.080907629203210886e-05,-3.302737570497291802e-05,-9.169346160818433913e-06,-2.576260220253686874e-05
+2.451205390000000079e+03,-1.149739003401074152e-05,-4.252722100548740380e-05,-6.722367725701801447e-06,-2.137163272995342548e-05
+2.453133949999999913e+03,-1.190315382012493609e-05,-2.716228646798271248e-05,-8.599444306171916968e-06,-1.252530390613443910e-05
+2.455062519999999950e+03,-1.250473435713637051e-05,-3.955923675588936028e-05,-6.962682847335037515e-06,-1.500534938678919366e-05
+2.456991079999999783e+03,-1.288231582906698847e-05,-4.425062203473166409e-05,-5.841435007818884482e-06,-1.305621787619276657e-05
+2.458919649999999820e+03,-1.283800572661077128e-05,-4.642059959516265679e-05,-6.911159473017441945e-06,-2.016189104520898722e-05
+2.460848210000000108e+03,-1.248481584780219090e-05,-4.266192766138991472e-05,-6.655617911174898463e-06,-1.683584695192563292e-05
+2.462776780000000144e+03,-1.250144529155731415e-05,-4.177946025392670072e-05,-6.673367030338060557e-06,-1.595834023163939647e-05
+2.464705339999999978e+03,-1.342464668897613276e-05,-4.010059897203849797e-05,-6.834612579210746626e-06,-1.090365718910149564e-05
+2.466633910000000014e+03,-1.240975937026768524e-05,-4.437110877377607764e-05,-6.383945573782426378e-06,-1.767392759377422022e-05
+2.468562469999999848e+03,-1.163288982824932922e-05,-4.512491969149263024e-05,-5.318674721926612214e-06,-1.714998545085499301e-05
+2.470491030000000137e+03,-1.412232187892063358e-05,-4.735957397624390583e-05,-6.598738908415589227e-06,-1.402657291280140718e-05
+2.472419600000000173e+03,-1.353841044142880611e-05,-5.193896669799613028e-05,-5.790840312304797406e-06,-1.761359747357059343e-05
+2.474348160000000007e+03,-1.496625620299489220e-05,-5.600460171917175702e-05,-5.475256530164194352e-06,-1.395502196071776412e-05
+2.476276730000000043e+03,-1.410675241350641839e-05,-4.703682987312275736e-05,-8.117643409633936637e-06,-2.050226813866852036e-05
+2.478205289999999877e+03,-1.372589513745427371e-05,-5.735905793158538893e-05,-6.466382776768753368e-06,-2.519601351678301689e-05
+2.480133859999999913e+03,-1.175873148636344473e-05,-5.046225716279310056e-05,-5.693111120665994335e-06,-2.358871421219822125e-05
+2.482062420000000202e+03,-1.424820726329949136e-05,-5.053865209617880883e-05,-8.592694456277980247e-06,-2.548207796789401676e-05
+2.483990980000000036e+03,-1.626401496187831642e-05,-6.013440566666503160e-05,-7.334209435409267304e-06,-2.057117917244769155e-05
+2.485919550000000072e+03,-1.633395187698639288e-05,-5.229720122333751675e-05,-8.464060983675463474e-06,-1.742989364604098179e-05
+2.487848109999999906e+03,-1.657901684738727005e-05,-5.387604757407640966e-05,-7.442191937267313808e-06,-1.339562811974399833e-05
+2.489776679999999942e+03,-1.634575823066303002e-05,-5.174491550583970156e-05,-7.919801621909527696e-06,-1.441397601847374004e-05
+2.491705239999999776e+03,-1.561812237290269981e-05,-5.951514464634993979e-05,-5.913704360935588079e-06,-1.652002155391785163e-05
+2.493633809999999812e+03,-1.886076408405971462e-05,-4.102776205251719113e-05,-9.557525432234834279e-06,1.899483243674288754e-07
+2.495562370000000101e+03,-1.629305352749990825e-05,-4.586831157612251627e-05,-8.448975890551628000e-06,-1.111536883073655119e-05
+2.497490940000000137e+03,-1.598131896948869849e-05,-4.976339980796436831e-05,-7.755105221252413985e-06,-1.331741487059634562e-05
+2.499419499999999971e+03,-1.666105390510960225e-05,-5.248044677568889255e-05,-6.810286950820351547e-06,-8.836929232211052863e-06
+2.501348059999999805e+03,-1.478061758277673009e-05,-6.464772137869518839e-05,-4.919365881409000947e-06,-2.095775148839180833e-05
+2.503276629999999841e+03,-1.729517276573744913e-05,-5.879960798906879636e-05,-4.662562103758487837e-06,-2.831218156646552846e-06
+2.505205190000000130e+03,-1.668357426238937326e-05,-5.068305424346340862e-05,-6.988229534512138195e-06,-7.728130054851795530e-06
+2.507133760000000166e+03,-1.442468862757216363e-05,-3.990371858148821117e-05,-5.571868797745471328e-06,-6.815748291120625932e-07
+2.509062320000000000e+03,-1.668339372721174894e-05,-4.959961911991344187e-05,-6.206834790322761704e-06,-3.183549601762493902e-06
+2.510990890000000036e+03,-1.540642351034921765e-05,-4.785343731048059037e-05,-4.782162247509662781e-06,-7.829772170832068028e-07
+2.512919449999999870e+03,-1.683917714723294747e-05,-3.605770677399621182e-05,-5.581736106114729516e-06,1.381803669375281377e-05
+2.514848019999999906e+03,-1.572410002454044601e-05,-3.609639710033047728e-05,-5.954059345038407544e-06,7.189465185821298994e-06
+2.516776580000000195e+03,-1.956912927698259408e-05,-4.293451032816624684e-05,-6.693771871706184393e-06,1.410936142346955388e-05
+2.518705140000000029e+03,-1.595749906984328907e-05,-3.062393522156565089e-05,-9.209611846046317321e-06,-7.276301115396590806e-07
+2.520633710000000065e+03,-1.492178368832841090e-05,-3.405788586781936306e-05,-6.791284292197581314e-06,1.964039600406694645e-06
+2.522562269999999899e+03,-1.494269919019668689e-05,-2.717982861047692659e-05,-6.312278311604227878e-06,1.105698348448791553e-05
+2.524490839999999935e+03,-1.331524675418178173e-05,-3.426138817850559099e-05,-5.163047490327029740e-06,1.856677880812998911e-06
+2.526419400000000223e+03,-1.428578723511560141e-05,-1.720967949958725050e-05,-8.571775342315759855e-06,8.106073014328946019e-06
+2.528347969999999805e+03,-1.326239034040913255e-05,-2.515904947654569793e-05,-6.753804107792869639e-06,3.677040012175864362e-06
+2.530276530000000093e+03,-1.171703424237893133e-05,-1.778792973083950413e-05,-8.322578422196623898e-06,-2.748898473057010318e-06
+2.532205100000000130e+03,-1.186965832371030293e-05,-2.493420673872672944e-05,-6.200028961849891956e-06,1.849103480529548301e-07
+2.534133659999999963e+03,-1.335942342691378466e-05,-2.570362468030427077e-05,-6.441477751032965193e-06,4.946119128594445071e-06
+2.536062219999999797e+03,-1.191145836385874832e-05,-1.728849187350584490e-05,-7.177787357392890199e-06,3.683890741412199454e-06
+2.537990789999999834e+03,-1.123954209052403697e-05,-2.782182556920180736e-05,-5.282870742158839663e-06,-1.430977861662525444e-06
+2.539919350000000122e+03,-1.364155657620412138e-05,-2.957279345565957151e-05,-5.939654638957755454e-06,4.550244260707818961e-06
+2.541847920000000158e+03,-1.126190086553095898e-05,-2.247157486929877597e-05,-5.773918871845860922e-06,1.842759185208091669e-06
+2.543776479999999992e+03,-1.122792500086183713e-05,-2.510897988353789773e-05,-4.940379429826434778e-06,2.747795807964491759e-06
+2.545705050000000028e+03,-1.102162011288937080e-05,-1.740448133905195122e-05,-6.480312303370474291e-06,2.715642096491357159e-06
+2.547633609999999862e+03,-1.118290525581481881e-05,-2.039990931901165152e-05,-6.899665805717961780e-06,-1.423149747837095891e-06
+2.549562179999999898e+03,-1.125125952598923516e-05,-1.014412088323676651e-05,-7.792071146359387239e-06,5.181705971984254441e-06
+2.551490740000000187e+03,-1.083771145702672639e-05,-1.096876997415514980e-05,-8.563127283957617532e-06,-8.912953245052765659e-07
+2.553419300000000021e+03,-1.292749190992805893e-05,-2.885131798441644314e-06,-9.606385306764881658e-06,1.182892802771228490e-05
+2.555347870000000057e+03,-1.022850041845212673e-05,-1.285406202604350572e-05,-6.397370643303027162e-06,4.119639649058604151e-06
+2.557276429999999891e+03,-9.841260859013380274e-06,-2.751712013982191994e-05,-4.399570951741098305e-06,-3.407881738765899101e-06
+2.559204999999999927e+03,-1.068299792691532448e-05,-1.626910071195899836e-05,-6.683684110700862395e-06,1.449735142119204499e-06
+2.561133560000000216e+03,-1.127036389488905702e-05,-1.666685453234273352e-05,-6.801227733786608909e-06,3.133514652752749650e-06
+2.563062129999999797e+03,-1.144429658457902341e-05,-1.371758677727742146e-05,-7.597623812484170265e-06,3.324977663843618457e-06
+2.564990690000000086e+03,-1.062497540924848047e-05,-1.243704360730464810e-05,-7.008754136369198148e-06,3.584512612263012366e-06
+2.566919260000000122e+03,-9.507044138009454169e-06,-2.725451248231144371e-05,-5.115121049685601140e-06,-7.796233421978392510e-06
+2.568847819999999956e+03,-1.242183575093232207e-05,-1.937697245567159365e-05,-4.471112745467482801e-06,1.584845928812240440e-05
+2.570776379999999790e+03,-1.018448212730589889e-05,-1.897506390432536754e-05,-4.059628781440804590e-06,8.160908928236569804e-06
+2.572704949999999826e+03,-1.076765486726059320e-05,-1.903207952878973596e-05,-6.372798451314586967e-06,4.391955486181540163e-07
+2.574633510000000115e+03,-1.097836791140931931e-05,-2.828888812137091732e-05,-4.375747502015462621e-06,9.638168718005485095e-07
+2.576562080000000151e+03,-9.970086068421227281e-06,-2.386039705729088730e-05,-5.032932197488913696e-06,-1.986489920845944321e-06
+2.578490639999999985e+03,-9.100742219122372444e-06,-1.910595947299100489e-05,-4.912284444797469097e-06,-5.491271773827829482e-07
+2.580419210000000021e+03,-9.204697466758020858e-06,-2.192211399411344257e-05,-4.809846136449591277e-06,-2.450861448465131231e-06
+2.582347769999999855e+03,-8.610345475574367392e-06,-2.026695673318284281e-05,-3.890956784922891983e-06,6.421485243782427832e-07
+2.584276339999999891e+03,-9.066820504616070783e-06,-1.692426102410389449e-05,-4.487531854908556714e-06,3.364135346204783561e-06
+2.586204900000000180e+03,-8.492128578161136675e-06,-2.236257906812555980e-05,-3.187717078490591214e-06,1.138451604709023515e-06
+2.588133460000000014e+03,-8.443921749501543211e-06,-2.002127875187866598e-05,-2.833710578615899374e-06,4.834587882195933261e-06
+2.590062030000000050e+03,-9.732247504084194357e-06,-2.000839770304068169e-05,-3.021970237906477680e-06,9.721277655943373142e-06
+2.591990589999999884e+03,-7.779626706176440474e-06,-3.315384588041936484e-05,3.265592671464057491e-07,2.760359721954006191e-06
+2.593919159999999920e+03,-8.546904877315940826e-06,-2.839012499166511399e-05,-7.095644252659074319e-07,6.332968864932318046e-06
+2.595847720000000209e+03,-8.513879630362989123e-06,-1.619078058155518586e-05,-1.749669835409452240e-06,1.377784117385811108e-05
+2.597776289999999790e+03,-9.991082764532040547e-06,-3.734862194643762290e-06,-4.319518763808174764e-06,2.139282624963217733e-05
+2.599704850000000079e+03,-9.284546477200230686e-06,-2.762315736723795284e-06,-4.032903473030821160e-06,2.050492575301128979e-05
+2.601633420000000115e+03,-9.566456536861948882e-06,-2.407228598269416391e-06,-4.664342753994989212e-06,1.931143451450697795e-05
+2.603561979999999949e+03,-9.327186639612863655e-06,-1.049161330331355226e-05,-3.955261680189834452e-06,1.330853365953186718e-05
+2.605490539999999783e+03,-1.015531332657209902e-05,-5.322656612683462027e-06,-4.783800020734969974e-06,1.847566653171397574e-05
+2.607419109999999819e+03,-9.749614613203356697e-06,3.388837413158266030e-07,-5.256758862501073633e-06,2.024434183264858710e-05
+2.609347670000000107e+03,-9.647836999907092922e-06,-2.942044453571268830e-06,-4.666392651815079939e-06,1.912809026859346319e-05
+2.611276240000000143e+03,-1.221996180577556808e-05,-1.612652496479826462e-06,-4.781001028102432085e-06,3.134543256554221549e-05
+2.613204799999999977e+03,-1.201566153044374193e-05,-2.123206546403832363e-06,-6.540161270725542147e-06,2.213582757278984844e-05
+2.615133370000000014e+03,-1.120980538295547525e-05,3.589613692964170847e-06,-8.386740577434581071e-06,1.609711477768713953e-05
+2.617061929999999847e+03,-1.243517439085982105e-05,5.743096697224532657e-06,-9.920984203347787435e-06,1.688213836428407573e-05
+2.618990490000000136e+03,-1.164823690917524654e-05,1.591003823203314516e-05,-1.263741792188694812e-05,1.152750242722857330e-05
+2.620919060000000172e+03,-1.153855257077280284e-05,6.784925468069754532e-06,-1.081522758054149621e-05,9.989594408801336447e-06
+2.622847620000000006e+03,-1.058944435192996451e-05,7.627026829767902927e-06,-1.142918485898130599e-05,3.906582551517441331e-06
+2.624776190000000042e+03,-9.468978135134760701e-06,7.706549663896507169e-07,-7.955476908207106317e-06,7.476175222427245747e-06
+2.626704749999999876e+03,-9.731213184347647382e-06,6.888510154298094164e-06,-8.239528808071579314e-06,1.349737153000948719e-05
+2.628633319999999912e+03,-8.791985720480663809e-06,-1.259307707209650884e-06,-5.882304125455096429e-06,1.163194637764503206e-05
+2.630561880000000201e+03,-8.588667692738192328e-06,-5.583369131886249433e-06,-5.808551898974998832e-06,6.733847687985021911e-06
+2.632490449999999782e+03,-8.788163060336794940e-06,3.123532137163631771e-06,-6.764242793970034075e-06,1.209044812062588235e-05
+2.634419010000000071e+03,-8.041531220523757915e-06,-3.792669498540376758e-06,-3.537373382661817768e-06,1.616286213950395142e-05
+2.636347569999999905e+03,-7.077005994864135072e-06,-6.884572029687482626e-06,-2.513235277215625251e-06,1.333507262380581371e-05
+2.638276139999999941e+03,-7.455756557576984978e-06,-4.939255542269938561e-06,-2.879384158750158889e-06,1.533622046893745873e-05
+2.640204699999999775e+03,-7.961496736174973230e-06,-1.177876145403027797e-05,-1.724586778035791878e-06,1.585367472461837274e-05
+2.642133269999999811e+03,-5.825421714230312439e-06,-1.485537800220775233e-05,-8.680170387725095743e-07,7.108249695760895136e-06
+2.644061830000000100e+03,-6.306168201469945764e-06,-2.230701611950414360e-05,3.758280674806154678e-07,7.297361158187572617e-06
+2.645990400000000136e+03,-6.024503851919034322e-06,-1.216833272841000901e-05,-5.072408525597727890e-07,1.227572991380591250e-05
+2.647918959999999970e+03,-5.493482245927149425e-06,-1.282622152849448795e-05,-6.268814136070338937e-07,8.735102558051359613e-06
+2.649847530000000006e+03,-5.744123274204637362e-06,-1.073844601491043401e-05,-1.277321959524644126e-06,9.051578705508083416e-06
+2.651776089999999840e+03,-5.521895412440159295e-06,-8.278028442975040620e-06,-1.391437145461159985e-06,1.002183883375595834e-05
+2.653704650000000129e+03,-6.806033947990544194e-06,1.981091782336067647e-07,-2.792182883525710557e-06,1.798135185992158315e-05
+2.655633220000000165e+03,-5.747349419399928116e-06,-1.211179352340936184e-05,-8.040966459283798340e-07,9.789134611624058605e-06
+2.657561779999999999e+03,-6.513965545548013874e-06,-6.014970405224369830e-06,-1.438352909835634454e-06,1.647237399532071276e-05
+2.659490350000000035e+03,-6.410750329040323233e-06,-1.732514165411398697e-05,5.268920392277509732e-07,1.341186773966158974e-05
+2.661418909999999869e+03,-8.596173941318742927e-06,-8.110109701498699125e-06,-2.162979373481796746e-07,2.901667109522007972e-05
+2.663347479999999905e+03,-7.334842236737963861e-06,-9.024887230447635982e-06,4.056872616072176892e-07,2.526928869762456103e-05
+2.665276040000000194e+03,-7.333652323119725285e-06,-6.699640627084085253e-06,2.471547857505099757e-07,2.688689020700883262e-05
+2.667204609999999775e+03,-7.172972496216403308e-06,-1.433564805741605556e-05,5.501262892596565752e-07,1.988130163777205998e-05
+2.669133170000000064e+03,-8.924146374543233263e-06,-1.545191851304982073e-05,-4.391444558414652550e-07,2.214061938919542169e-05
+2.671061729999999898e+03,-9.174258867161041672e-06,-1.197887104653733228e-05,-7.033649579737996351e-07,2.555116175700768377e-05
+2.672990299999999934e+03,-9.131884485661369381e-06,-1.175686224774288516e-05,-3.567487704723297647e-07,2.712110444352010318e-05
+2.674918860000000222e+03,-7.980739346143605003e-06,-1.483170841045148257e-05,-2.234311426422314943e-07,1.953680505054979064e-05
+2.676847429999999804e+03,-5.872032432760916564e-06,-8.493322097814265972e-06,-5.849778096849185513e-07,1.493080947146124628e-05
+2.678775990000000093e+03,-4.446923984750107296e-06,-1.370420479520131659e-05,2.017945131828671556e-07,6.891798364825344900e-06
+2.680704560000000129e+03,-3.321427124438596420e-06,-1.212471250249377359e-05,3.466156342824701958e-07,4.126437203242021409e-06
+2.682633119999999963e+03,-3.557944788280882590e-06,-7.882685531154602214e-06,4.240700567739879423e-09,7.899466822778954852e-06
+2.684561689999999999e+03,-2.493472059107507014e-06,-1.148577503515186662e-05,2.283169601592544821e-07,5.730268188795051611e-07
+2.686490249999999833e+03,-2.397907732176565329e-06,-6.956387873785245662e-06,-4.268220859061319176e-07,1.776445963608872504e-06
+2.688418810000000121e+03,-2.266970891356556010e-06,-1.202337430508687616e-05,1.435062172938899472e-07,-1.343830218041938170e-06
+2.690347380000000157e+03,-8.973118711810686882e-07,-1.468034703947901061e-05,7.550281500407228206e-07,-7.359705810362967731e-06
+2.692275939999999991e+03,-8.887408193180015884e-07,-9.904064184158473363e-06,2.761235096739862176e-07,-4.743168894071749401e-06
+2.694204510000000028e+03,-8.455618469677093958e-07,-1.330740772758972258e-05,7.627159060862146283e-07,-6.181983011331329381e-06
+2.696133069999999861e+03,-6.338636297846383512e-07,-1.617019582254805666e-05,1.106289618165993397e-06,-8.460500815277126126e-06
+2.698061639999999898e+03,-1.539746004979737881e-06,-9.903817857432885321e-06,-1.057410636067399677e-07,-3.550503429565384520e-06
+2.699990200000000186e+03,-9.908676877475467093e-07,-9.535156822763574008e-06,-4.328439897089458454e-07,-7.062850131514554102e-06
+2.701918770000000222e+03,-3.620676440448356664e-07,-1.002659860852487571e-05,-6.669870506243931544e-07,-1.137753458459192018e-05
+2.703847330000000056e+03,-4.539926480500033472e-07,-7.874256925111896928e-06,-1.319158683956242972e-06,-1.170734822057230091e-05
+2.705775889999999890e+03,-5.917316105539366602e-07,-9.745359974625851231e-06,-8.558771363284525881e-07,-1.091564853608162860e-05
+2.707704459999999926e+03,-4.334810997286590911e-07,-1.391441194682334742e-05,-1.920205193936313231e-07,-1.284462833273413752e-05
+2.709633020000000215e+03,-7.044710862338745349e-08,-1.453067773873898880e-05,-1.958048085249238838e-07,-1.508607114112584675e-05
+2.711561589999999796e+03,-3.900210941470514237e-07,-1.244597925311577241e-05,-8.806467581410636824e-07,-1.461968104437371796e-05
+2.713490150000000085e+03,-2.579517728321195287e-07,-1.349126214279295837e-05,-8.456446813106339616e-07,-1.609501735092844774e-05
+2.715418720000000121e+03,-5.091098613437474728e-07,-1.548232456036472744e-05,-7.755070420193747709e-07,-1.666258900904172630e-05
+2.717347279999999955e+03,-1.355360952529855101e-06,-1.370405939620413440e-05,-1.533138428215957870e-06,-1.449169698979914560e-05
+2.719275849999999991e+03,-4.525098267867001909e-07,-2.662395682240631899e-05,-5.705444750179095118e-07,-2.714690567143720961e-05
+2.721204409999999825e+03,-6.728279527713405008e-07,-3.351796788586204514e-05,-9.706311343681028777e-07,-3.483737564779905259e-05
+2.723132970000000114e+03,-2.102233059460060047e-07,-5.015086852038187434e-05,-1.103385949557034758e-06,-5.410799791817398017e-05
+2.725061540000000150e+03,-4.078922688694047318e-07,-6.886549724357977898e-05,-2.150084672456009346e-06,-7.658422666666679722e-05
+2.726990099999999984e+03,-6.735028627300027408e-07,-8.252449109972902338e-05,-2.063842823323206656e-06,-8.868434918419283838e-05
+2.728918670000000020e+03,-2.211200316482246686e-09,-8.976302622920064294e-05,-1.403347551581319334e-06,-9.597071738776622059e-05
+2.730847229999999854e+03,-1.104399743875542366e-06,-7.473540557619656429e-05,-1.132117185513563602e-06,-7.485820684192568829e-05
+2.732775799999999890e+03,5.976572653480817289e-07,-5.915374651288227983e-05,5.098106760420390401e-07,-5.954294810290095062e-05
+2.734704360000000179e+03,9.505334984147938463e-07,-4.330474778936802926e-05,6.374013948774310582e-07,-4.469206986465155826e-05
+2.736632930000000215e+03,9.466683026865524711e-07,-3.476401801420444143e-05,2.061030059299432528e-07,-3.804506959841786869e-05
+2.738561490000000049e+03,-3.721920924902759756e-07,-1.763125463217550759e-05,-1.810924243015130184e-06,-2.400551281361143811e-05
+2.740490049999999883e+03,7.802127451319687138e-07,-1.804014558623623946e-05,2.925917138409332727e-07,-2.020053544546974807e-05
+2.742418619999999919e+03,-2.518191381782286337e-07,-5.179007004994381405e-06,-4.134054251712767007e-07,-5.894910039132839944e-06
+2.744347180000000208e+03,8.191920146900887457e-08,-4.469877895979809744e-06,-8.640417435437617502e-09,-4.871099479510007172e-06
+2.746275749999999789e+03,-3.374024534204674675e-07,-1.718816392603065141e-06,-5.367731571042888393e-07,-2.602122113290291001e-06
+2.748204310000000078e+03,3.321511799746463570e-07,-5.427599762682053071e-06,-2.594547042808017199e-07,-8.048691288665704650e-06
+2.750132880000000114e+03,-6.838999653523931634e-08,-2.827403334046409197e-07,-5.255862464922086994e-07,-2.308334142333496315e-06
+2.752061439999999948e+03,4.121706903012297769e-07,-5.344884810732012668e-06,2.259439976834055483e-07,-6.169956397954055051e-06
+2.753990009999999984e+03,-1.789066137203236485e-06,3.081672127316419189e-06,-1.175748401225589173e-06,5.798957339125377204e-06
+2.755918569999999818e+03,-6.016384824085109990e-07,-5.081539940903397068e-07,-5.085917710017807764e-07,-9.591342434725497012e-08
+2.757847130000000107e+03,-7.303889934912214227e-07,3.188655737467853898e-06,-7.455854520888071304e-07,3.121328298855200494e-06
+2.759775700000000143e+03,-3.922394727749878726e-08,-1.194146607198047218e-06,-5.605911142546173597e-08,-1.268734279939510486e-06
+2.761704259999999977e+03,-1.229869240095863255e-07,-1.670608361841801763e-06,-1.991061444716516380e-07,-2.007852207833456950e-06
+2.763632830000000013e+03,4.887571037181728887e-07,-5.597450827387029484e-06,1.941885839229500375e-07,-6.902527520511039825e-06
+2.765561389999999847e+03,1.528691179571403663e-07,9.833914844409979662e-07,-6.524434484993868542e-07,-2.584520870527964626e-06
+2.767489959999999883e+03,5.362887417884648332e-07,-2.190413073006887769e-06,1.121510768094063646e-08,-4.516735527707859622e-06
+2.769418520000000171e+03,-3.942790174082070299e-07,2.290035058096983582e-06,-5.100966025995223534e-07,1.776908838118803956e-06
+2.771347080000000005e+03,-2.941781146242632214e-07,1.330928223358317839e-06,-3.288015308858582616e-07,1.177530251196353560e-06
+2.773275650000000041e+03,1.743840081853523131e-07,-1.969667614474662449e-06,1.836340095207429334e-07,-1.928685770377485000e-06
+2.775204209999999875e+03,-1.424299323451872908e-07,1.938799962597440877e-08,-1.270319122326478368e-07,8.760845028071520615e-08
+2.777132779999999912e+03,5.169490614543114833e-07,-4.735598768540526245e-06,5.774691420914222312e-07,-4.467466427853251311e-06
+2.779061340000000200e+03,-1.394129317630247955e-07,-1.580351334629364123e-06,-6.121515620892882184e-08,-1.233898514753231950e-06
+2.780989909999999782e+03,-4.095980630536903775e-07,-1.672085938185853503e-06,-2.181628334014830250e-07,-8.239380891366079462e-07
+2.782918470000000070e+03,-1.375503528109051986e-06,-1.187900481850742145e-06,-5.466261986129501422e-07,2.484414825081038795e-06
+2.784847040000000106e+03,-1.430097299714483432e-06,-8.825846596969270279e-06,2.016821593536125254e-07,-1.596298300943868554e-06
+2.786775599999999940e+03,-1.172377632545468419e-06,-2.371664046912319185e-06,-3.068608625539841509e-07,1.462981165037379331e-06
+2.788704159999999774e+03,4.036113246950310560e-08,-5.253003441310678585e-06,1.676259557084188548e-07,-4.689160588112658457e-06
+2.790632729999999810e+03,1.035365169548496805e-07,-2.134193941668906343e-06,-5.593641643277065831e-07,-5.071154855208869080e-06
+2.792561290000000099e+03,-2.422071148247040565e-07,-1.116867280159202755e-06,-1.185418926056678315e-06,-5.295737963197131388e-06
+2.794489860000000135e+03,-1.803915802208921670e-07,-1.225039694994325325e-06,-1.036078062644315895e-06,-5.016132122686219910e-06
+2.796418419999999969e+03,-4.427253243047642804e-07,-7.264907074067881150e-07,-6.348897754168534151e-07,-1.577869349522717638e-06
+2.798346990000000005e+03,-1.284279917752730413e-07,-2.941034723852204241e-06,-2.176365745496850174e-07,-3.336270583700515147e-06
+2.800275549999999839e+03,4.395955557551461926e-07,-6.787069622555993186e-06,3.746262781519247939e-07,-7.074913992443217352e-06
+2.802204119999999875e+03,-9.757628012636476538e-08,-5.669911917275681748e-06,-2.372182554558420291e-07,-6.288591359026584888e-06
+2.804132680000000164e+03,2.863872861892948310e-07,-5.214836136772778050e-06,-6.550510480585895030e-08,-6.773884463779051487e-06
+2.806061239999999998e+03,4.572478899465631437e-07,-2.333458978808418234e-06,-1.052266704056855810e-06,-9.021316581290639275e-06
+2.807989810000000034e+03,-6.062703912221728551e-08,2.188171009143768430e-06,-1.926514285289672288e-06,-6.078584578531833653e-06
+2.809918369999999868e+03,-3.456752312573398003e-07,4.923173589563079076e-06,-2.106757040150604479e-06,-2.879244758022163299e-06
+2.811846939999999904e+03,-2.188036473601842917e-07,2.986841806139900372e-07,-8.803330530739069128e-07,-2.632201339038061702e-06
+2.813775500000000193e+03,-5.394197194038973197e-07,-2.283887173953936354e-06,-1.774164687960818067e-07,-6.800429969460832419e-07
+2.815704069999999774e+03,5.648900331407176218e-07,-5.690010743322508063e-06,6.711437592957878660e-07,-5.219256904253204932e-06
+2.817632630000000063e+03,-5.860835383883766639e-08,-9.233775813690725975e-07,-9.823311368467128619e-09,-7.072369634055296431e-07
+2.819561200000000099e+03,-1.651727361725572225e-07,-3.710668996565389176e-07,-8.702622563564708412e-08,-2.484120784944976423e-08
+2.821489759999999933e+03,1.459418027667835522e-06,-1.166275036799863026e-05,1.646324087217821554e-06,-1.083466886664910605e-05
+2.823418320000000222e+03,-1.103929585246975950e-06,1.644399462377772712e-06,-6.154873301256754069e-07,3.808427728327185568e-06
+2.825346889999999803e+03,-1.835400298875349318e-06,-5.252735046838593945e-06,-1.614911477758993624e-07,2.163467543395961450e-06
+2.827275450000000092e+03,-2.209714346672288721e-06,-5.928948678112627295e-06,-3.302459123979645367e-07,2.397977942351983253e-06
+2.829204020000000128e+03,-1.827017779515134788e-06,-9.212352899527674014e-06,-1.760417661777723969e-07,-1.897754865049141174e-06
+2.831132579999999962e+03,-8.360243330829078886e-07,-8.491939679978950287e-06,4.983799032506324024e-07,-2.579903087421474636e-06
+2.833061149999999998e+03,-1.291724927510241167e-06,-5.565833366219364855e-06,3.100385720776250080e-07,1.530730152048268085e-06
+2.834989709999999832e+03,-5.535364631661718762e-07,-5.006611742656915644e-06,1.372829742804345672e-07,-1.945957645622518047e-06
+2.836918279999999868e+03,4.678815052559147374e-07,-8.138297073298956407e-06,7.322574619884005443e-07,-6.966987594628980467e-06
+2.838846840000000157e+03,3.489891228615339346e-07,-6.502657773107469466e-06,5.525697543542591276e-07,-5.600700097802165022e-06
+2.840775399999999991e+03,-6.843148378138123031e-07,-6.621374305298871026e-07,-2.937542806874682001e-07,1.068229007518075501e-06
+2.842703970000000027e+03,-4.322720957276639507e-07,-4.511097244715439235e-06,1.696618881574727338e-07,-1.844247393570836606e-06
+2.844632529999999861e+03,2.411808475693834832e-07,-5.450757024171179784e-06,4.020419398034134089e-07,-4.738066942926086684e-06
+2.846561099999999897e+03,-1.548341264386721983e-07,-3.111569021402184112e-06,-8.185435547930192154e-08,-2.788234409085787953e-06
+2.848489660000000185e+03,7.043469659918767254e-07,-9.107057753005148238e-06,7.861992159460945062e-07,-8.744413897615331733e-06
+2.850418230000000221e+03,5.356420171384334088e-07,-6.724519597262984664e-06,6.076113396127190297e-07,-6.405661745628290041e-06
+2.852346790000000055e+03,-7.888869502349746348e-07,2.794369298134342174e-07,-7.543090286744540644e-07,4.326333391129643033e-07
+2.854275360000000092e+03,4.235100938191441013e-07,-5.484083561698086137e-06,5.098358114234647676e-07,-5.101620146595468839e-06
+2.856203919999999925e+03,-1.166929216252101221e-07,-2.193666231926418849e-06,-5.138953940640100582e-09,-1.699429837107821903e-06
+2.858132480000000214e+03,-1.592859055182356556e-07,-6.005469823211871575e-06,6.815050365485382043e-08,-4.997819864601362778e-06
+2.860061049999999796e+03,-1.690219735289651223e-06,-4.911460019323034044e-06,-8.982579538583933372e-07,-1.402697903434272148e-06
+2.861989610000000084e+03,-2.608534150425729445e-06,-7.977669920645707636e-06,-7.011895112198353515e-07,4.727613613972395726e-07
+2.863918180000000120e+03,-1.373777606960061826e-06,-9.899839825603489382e-06,1.797545117853490536e-07,-3.016963944624575994e-06
+2.865846739999999954e+03,-1.714897688311420095e-06,-6.906250823179463696e-06,-8.069905636000663626e-08,3.340155432930107205e-07
+2.867775309999999990e+03,-1.262406218367043601e-06,-7.665465271742190215e-06,-2.562189642425326921e-07,-3.207583841678930090e-06
+2.869703869999999824e+03,-1.399902385109686112e-06,2.121157225098905353e-06,-1.840578424405588262e-06,1.687556972537369963e-07
+2.871632439999999860e+03,3.467020972483779967e-07,-2.493412901787516415e-06,-8.300500601864596959e-07,-7.706976847178635483e-06
+2.873561000000000149e+03,3.412444399864605650e-07,-3.913900815072365425e-06,-7.634971992192315867e-07,-8.808424392314260858e-06
+2.875489559999999983e+03,3.441124681523421394e-07,-4.048444731109979409e-06,-1.142839671080475018e-06,-1.063634007733601175e-05
+2.877418130000000019e+03,-1.189874833131108321e-06,2.667198560688714785e-06,-1.823745464211563808e-06,-1.411456155796655070e-07
+2.879346689999999853e+03,-1.039331754577976253e-06,-2.181920489226485512e-06,-1.989020626164688881e-07,1.541577201398577470e-06
+2.881275259999999889e+03,-6.503551571747707594e-07,1.020586488373715517e-06,-4.023289744945124598e-07,2.119458800070658472e-06
+2.883203820000000178e+03,-4.384879762059236300e-07,1.700278489530249243e-06,-4.426643814976650809e-07,1.681775055385010327e-06
+2.885132390000000214e+03,3.813184576361268293e-08,-9.778246904281586077e-07,-1.206587654584583594e-08,-1.200224142615132982e-06
+2.887060950000000048e+03,1.311563245217122330e-07,-1.339926144839644540e-06,9.678777254790304982e-09,-1.878128651292614229e-06
+2.888989520000000084e+03,4.760333019212442881e-08,-2.308655830357966118e-07,-3.942273113480603866e-07,-2.188382540322948107e-06
+2.890918079999999918e+03,1.196127628357743018e-07,-4.896701893744500924e-07,-5.081437329066694479e-07,-3.270925878611722487e-06
+2.892846640000000207e+03,5.216250647052850353e-07,-2.731189469551709848e-06,-6.612649999744213113e-07,-7.971947222670156639e-06
+2.894775209999999788e+03,8.753300153990942558e-08,-4.623148088505409943e-06,-7.293851680580312233e-07,-8.242478708331848575e-06
+2.896703770000000077e+03,8.647859513236377694e-08,-4.241670256513637470e-06,-1.136951476981988623e-06,-9.662039255527644541e-06
+2.898632340000000113e+03,-3.620668105236751363e-07,-1.806636407046485829e-06,-1.560141091485246733e-06,-7.114667359577388171e-06
+2.900560899999999947e+03,1.558906257241406880e-06,-9.181238969533809993e-06,-8.577386170798478527e-07,-1.988810915113636813e-05
+2.902489469999999983e+03,-7.653886767119468770e-07,3.758923279453052064e-06,-2.072569544994957428e-06,-2.032501025084706505e-06
+2.904418029999999817e+03,-1.157156842257207483e-07,1.779370070027591589e-06,-1.766810739551781677e-06,-5.535755376290678330e-06
+2.906346590000000106e+03,-4.376184539035117512e-08,9.586805036098030042e-08,-1.730974037195285750e-06,-7.379273249225401888e-06
+2.908275160000000142e+03,-5.054518674009234175e-07,1.668892529926873346e-06,-2.202851296228475754e-06,-5.851383007407624738e-06
+2.910203719999999976e+03,-4.802888037581908580e-07,-1.259623565917897432e-06,-2.249020706510639237e-06,-9.095935417136089037e-06
+2.912132290000000012e+03,-2.012607677202758099e-07,-1.811910034934127569e-06,-2.352891410869691000e-06,-1.134464288275443880e-05
+2.914060849999999846e+03,-1.999888785648892442e-06,6.645769438945654116e-06,-3.560876113122633148e-06,-2.701365131368584609e-07
+2.915989419999999882e+03,-1.826296189862478204e-06,-5.945353309653030218e-07,-1.055527649565128230e-06,2.820330787228769940e-06
+2.917917980000000171e+03,-1.062938436633992202e-06,6.756328638459625408e-07,-7.615633027153170064e-07,2.010866049787949085e-06
+2.919846550000000207e+03,8.911266832818667281e-08,-3.439063587698259843e-07,-4.928950011250952762e-07,-2.922473291688976351e-06
+2.921775110000000041e+03,-3.834210593013512459e-07,3.958259975606476481e-06,-1.421727535746612021e-06,-6.419246730125860402e-07
+2.923703669999999875e+03,7.792132951941104531e-07,-5.617660477840350819e-06,-5.170223025659357391e-07,-1.136059210071141519e-05
+2.925632239999999911e+03,-5.365359299522971874e-07,-1.404740642595319019e-06,-1.671978178274556706e-06,-6.435282316579511826e-06
+2.927560800000000199e+03,-2.120586794689366899e-07,-8.869691791061717727e-06,2.717161394080237354e-07,-6.726342456667395192e-06
+2.929489369999999781e+03,-9.510721136822481344e-07,-3.358573784697118385e-06,-4.106252200875005581e-07,-9.641405805241042194e-07
+2.931417930000000069e+03,-4.612001998398303162e-07,-1.228475954551572596e-06,-3.609034290667721964e-07,-7.841142215920741876e-07
+2.933346500000000106e+03,-7.134477079113726895e-07,-1.806759187992067569e-07,-4.987884106836139123e-07,7.703654415236115893e-07
+2.935275059999999939e+03,-1.032431045812116469e-06,-3.584729568755307604e-06,-2.572202770230504353e-07,-1.501822949710180257e-07
+2.937203629999999976e+03,-7.530787260208338888e-07,3.706611258241961082e-06,-1.188705619185353571e-06,1.776579815770562821e-06
+2.939132189999999810e+03,-1.403484086463112634e-07,-1.244681916311529997e-06,-5.039516582600811905e-07,-2.855614839303320344e-06
+2.941060750000000098e+03,-4.801452458740752991e-07,4.315925705287345034e-07,-5.650528633444279520e-07,5.541200409794419458e-08
+2.942989320000000134e+03,3.021890247286977210e-07,-3.226646917119526081e-06,2.822591279959700299e-07,-3.314945706617917955e-06
+2.944917879999999968e+03,7.867628341946854363e-07,-6.427857391775114794e-06,8.084244626809995293e-07,-6.331886218439102808e-06
+2.946846450000000004e+03,-8.601009227005504460e-07,2.999083884874160653e-06,-7.961075265627021702e-07,3.282604642188677254e-06
+2.948775009999999838e+03,-9.973349800585098698e-07,-1.871073866340646403e-06,-5.615760522981953043e-07,5.954255131336034012e-08
+2.950703579999999874e+03,-1.373014083358021529e-06,-5.570191738472565547e-06,-1.805921426077039392e-07,-2.872033039827745248e-07
+2.952632140000000163e+03,-1.760586771398549229e-06,-1.237137758719810994e-05,-3.269289170033037119e-07,-6.019600917423246880e-06
+2.954560710000000199e+03,-1.347012600625463261e-06,-1.783600170924386052e-06,-2.592879093517698550e-06,-7.303373036497842184e-06
+2.956489270000000033e+03,-9.913736443767789421e-07,4.650605827684954948e-06,-3.565795878494247004e-06,-6.755292054215735601e-06
+2.958417829999999867e+03,-1.008636708977777916e-06,5.820083372635410881e-06,-3.231068125614547141e-06,-4.026330106766755866e-06
+2.960346399999999903e+03,6.185131820064551847e-07,7.614150026013412204e-07,-1.822628441914561238e-06,-1.005398726852038463e-05
+2.962274960000000192e+03,-1.298157072590491488e-06,1.075057406380367722e-05,-3.485536691422769949e-06,1.059456487706241672e-06
+2.964203529999999773e+03,4.876565352861637197e-07,-4.332049823989790381e-06,-9.105789793711460086e-07,-1.052688891591336969e-05
+2.966132090000000062e+03,-2.031168399745526489e-07,-4.838160312944546484e-06,-7.561313102816042783e-07,-7.288273776052487151e-06
+2.968060660000000098e+03,2.591521356074030947e-07,-3.195034178240104199e-06,-5.812578535795484646e-07,-6.918444576333430741e-06
+2.969989219999999932e+03,-2.112688098323755511e-07,-3.214713014019570160e-06,-1.345054311323378344e-06,-8.237914522539432395e-06
+2.971917789999999968e+03,-1.748665903496432632e-06,6.086033911738658181e-06,-2.780046657693465674e-06,1.516533460791144277e-06
+2.973846349999999802e+03,-6.730102370897636039e-07,9.562798225261827168e-07,-2.630386428093572309e-06,-7.715814698404873753e-06
+2.975774910000000091e+03,-5.492570889084328380e-07,6.321012073323613367e-06,-3.739346061946018529e-06,-7.812578205085978915e-06
+2.977703480000000127e+03,1.006483234165418099e-06,-4.422326423018214090e-07,-2.185279646724218388e-06,-1.458323911754624975e-05
+2.979632039999999961e+03,-1.959904164863546289e-09,5.060059816554453344e-06,-1.789038820013845752e-06,-2.857537907293211606e-06
+2.981560609999999997e+03,-1.617324548336142391e-07,1.369893766370049685e-06,-6.053623350618939834e-07,-5.955946621348414765e-07
+2.983489169999999831e+03,-3.949598604099629995e-07,9.047359790515860658e-07,-5.794907001962900994e-07,8.717781521536314825e-08
+2.985417739999999867e+03,3.925417642344669118e-07,-5.761920093021135789e-06,3.035446133135261568e-07,-6.156219210598613051e-06
+2.987346300000000156e+03,4.064660839126005682e-08,-2.930042034486598528e-06,3.825083672928117667e-08,-2.940656426548144006e-06
+2.989274870000000192e+03,-6.262185979952911866e-07,-9.444496229407683878e-07,-4.409457100779591557e-07,-1.236038378691741144e-07
+2.991203430000000026e+03,-7.916696741674843306e-07,-3.038772771482785525e-06,2.478693998554686798e-08,5.785129412566555205e-07
+2.993131989999999860e+03,-1.236438867688935087e-06,-3.488891656635504231e-06,-6.561132206603148019e-08,1.698423479830147191e-06
+2.995060559999999896e+03,-1.092381031640258255e-06,-8.376186269098648431e-06,3.268966744478933416e-07,-2.088120400506143963e-06
+2.996989120000000185e+03,-8.628982136196507712e-07,-2.641373428981633671e-06,-5.512756771473341670e-07,-1.260739443771912020e-06
+2.998917690000000221e+03,-1.393096386864756126e-06,5.907048277932376223e-07,-1.462588072797505571e-06,2.828240680305454643e-07
+3.000846250000000055e+03,4.252454869399222429e-07,-3.860371341945959233e-06,-3.277432679392921872e-07,-7.196464672151397195e-06
+3.002774820000000091e+03,1.108616522327681333e-08,-8.333123431071946841e-07,-1.159273687793763771e-07,-1.396041867135800553e-06
+3.004703379999999925e+03,-2.298216243414827132e-08,-3.628520610479553611e-07,-6.509201813309981645e-08,-5.494184710014747552e-07
+3.006631949999999961e+03,-2.479599882119090031e-08,-2.180087918086043725e-07,-4.550862133229436936e-08,-3.097754235977330773e-07
+3.008560509999999795e+03,-2.257921480973014758e-08,-1.524974105854675029e-07,-3.546096467011316643e-08,-2.095696039112391885e-07
+3.010489070000000083e+03,-2.036345609674616585e-08,-1.164151388953090456e-07,-2.951600204275682528e-08,-1.569652099116855362e-07
+3.012417640000000119e+03,-1.836268617766706606e-08,-9.417902281587963085e-08,-2.550212239369167411e-08,-1.258100735950209914e-07
+3.014346199999999953e+03,-1.683870878122174535e-08,-7.919335531447621881e-08,-2.265077949353805148e-08,-1.049435543877028221e-07
+3.016274769999999990e+03,-1.552681593777920458e-08,-6.869069055160346241e-08,-2.045684221127043690e-08,-9.053301908859457422e-08
+3.018203329999999823e+03,-1.452157940367079515e-08,-6.083000552515009187e-08,-1.874536214599906525e-08,-7.954334399615881487e-08
+3.020131899999999860e+03,-1.363158983825844420e-08,-5.492736130699007699e-08,-1.733202387180853854e-08,-7.132201955148391945e-08
+3.022060460000000148e+03,-1.293479813234854214e-08,-5.019722041320874449e-08,-1.616860618110852915e-08,-6.452450670098788228e-08
+3.023989030000000184e+03,-1.229715222231069868e-08,-4.649366182539811155e-08,-1.516673144865346644e-08,-5.920724360927722127e-08
+3.025917590000000018e+03,-1.178852181967210394e-08,-4.337061495447727114e-08,-1.431359097368547920e-08,-5.455785554529162907e-08
+3.027846149999999852e+03,-1.130904473795722711e-08,-4.085928028505787275e-08,-1.355892999771690048e-08,-5.082732716514147826e-08
+3.029774719999999888e+03,-1.092106737747989926e-08,-3.865212598447649475e-08,-1.290124588888904844e-08,-4.742524547892083072e-08
+3.031703280000000177e+03,-1.054589688624951611e-08,-3.684671470180325940e-08,-1.230872926271316561e-08,-4.465688888472839312e-08
+3.033631850000000213e+03,-1.023906246351631397e-08,-3.520283268141998711e-08,-1.178354958479026631e-08,-4.204563498156422621e-08
+3.035560410000000047e+03,-9.935854474862146992e-09,-3.384395246779075319e-08,-1.130414188940671851e-08,-3.990610743078010324e-08
+3.037488980000000083e+03,-9.685894923880202443e-09,-3.256738377263426764e-08,-1.087364220902038015e-08,-3.782966129039264278e-08
+3.039417539999999917e+03,-9.434283387016006966e-09,-3.150598765736923748e-08,-1.047677730301382290e-08,-3.612472462708392724e-08
+3.041346100000000206e+03,-9.225619534976306995e-09,-3.048046664571150163e-08,-1.011664154800101011e-08,-3.442811204606644761e-08
+3.043274669999999787e+03,-9.012228949844327180e-09,-2.962577690885861475e-08,-9.782110944946890263e-09,-3.303671521605672895e-08
+3.045203230000000076e+03,-8.834460371946221882e-09,-2.877861145353823715e-08,-9.475874936650587664e-09,-3.162037879380891995e-08
+3.047131800000000112e+03,-8.650182729792939700e-09,-2.807268717349766806e-08,-9.189703060022196773e-09,-3.046301526741027447e-08
+3.049060359999999946e+03,-8.496130537977550051e-09,-2.735644756494237237e-08,-8.925764701477233160e-09,-2.925992840445319197e-08
+3.050988929999999982e+03,-8.334562615758228469e-09,-2.676082561589058744e-08,-8.677930107905223736e-09,-2.828210464288576946e-08
+3.052917489999999816e+03,-8.199123997609063542e-09,-2.614342957344623761e-08,-8.447845035726331838e-09,-2.724538042061113951e-08
+3.054846059999999852e+03,-8.055639859506099870e-09,-2.563172179316274160e-08,-8.230951891431967863e-09,-2.640843631462524053e-08
+3.056774620000000141e+03,-7.935094224141173368e-09,-2.509079094079099643e-08,-8.028410525621961809e-09,-2.550422592099788603e-08
+3.058703179999999975e+03,-7.806271776061337987e-09,-2.464437353990352077e-08,-7.836870014300623561e-09,-2.477993808564828667e-08
+3.060631750000000011e+03,-7.697844602276105516e-09,-2.416387428865163967e-08,-7.657052871302827153e-09,-2.398314778942347799e-08
+3.062560309999999845e+03,-7.581097064943355774e-09,-2.376926778925646103e-08,-7.486553852995352053e-09,-2.335039702026797456e-08
+3.064488879999999881e+03,-7.482679943941649410e-09,-2.333744589570319772e-08,-7.325713689350129299e-09,-2.264201177186411881e-08
+3.066417440000000170e+03,-7.376016840710624162e-09,-2.298468334294718793e-08,-7.172875804136693903e-09,-2.208467327929886448e-08
+3.068346010000000206e+03,-7.285977990808161705e-09,-2.259273598835788065e-08,-7.028050296965257590e-09,-2.144999533847579036e-08
+3.070274570000000040e+03,-7.187841862320145127e-09,-2.227430144533871725e-08,-6.890183084524206408e-09,-2.095553345996366198e-08
+3.072203140000000076e+03,-7.104899041611602610e-09,-2.191551386376536127e-08,-6.758998716851928031e-09,-2.038301320041646444e-08
+3.074131699999999910e+03,-7.014053188554083050e-09,-2.162563985786275843e-08,-6.633933145232366111e-09,-1.994152979249212147e-08
+3.076060260000000198e+03,-6.937185113516307189e-09,-2.129480487973845122e-08,-6.514465699404567290e-09,-1.942195962298194327e-08
+3.077988829999999780e+03,-6.852634039670658399e-09,-2.102899393188729872e-08,-6.400432567532855722e-09,-1.902552933121077019e-08
+3.079917390000000069e+03,-6.781015846983557414e-09,-2.072200799680771921e-08,-6.291103627465127510e-09,-1.855146709917671722e-08
+3.081845960000000105e+03,-6.701949735703823334e-09,-2.047670605987755735e-08,-6.186646893355684321e-09,-1.819367279509888431e-08
+3.083774519999999939e+03,-6.634908600526077111e-09,-2.019029348861978154e-08,-6.086150770963469823e-09,-1.775903894034238055e-08
+3.085703089999999975e+03,-6.560660460780401842e-09,-1.996265181577656072e-08,-5.990059684378022668e-09,-1.743462276882038549e-08
+3.087631649999999809e+03,-6.497641540460278599e-09,-1.969416344843137524e-08,-5.897306479006096391e-09,-1.703439757353855496e-08
+3.089560219999999845e+03,-6.427656871574219031e-09,-1.948187208969344465e-08,-5.808566443662978465e-09,-1.673901114526935866e-08
+3.091488780000000133e+03,-6.368198253391049929e-09,-1.922914035296683934e-08,-5.722639236081323174e-09,-1.636901114393711877e-08
+3.093417339999999967e+03,-6.302012203330340520e-09,-1.903030651427370864e-08,-5.640394095530340586e-09,-1.609902800277884023e-08
+3.095345910000000003e+03,-6.245725648801101335e-09,-1.879153772221992777e-08,-5.560515544220836862e-09,-1.575573560051856352e-08
+3.097274469999999837e+03,-6.182944376299662768e-09,-1.860459183986690508e-08,-5.484036721023318666e-09,-1.550810314453313811e-08
+3.099203039999999874e+03,-6.129501824601794159e-09,-1.837828966772399042e-08,-5.409544668262278237e-09,-1.518854181062191962e-08
+3.101131600000000162e+03,-6.069789895287674426e-09,-1.820192042251762072e-08,-5.338209346270559546e-09,-1.496067548456960565e-08
+3.103060170000000198e+03,-6.018911252276124598e-09,-1.798682257270524064e-08,-5.268535246304106381e-09,-1.466230494551836320e-08
+3.104988730000000032e+03,-5.961980690511123684e-09,-1.781992405500598775e-08,-5.201807592981139145e-09,-1.445200071745469994e-08
+3.106917300000000068e+03,-5.913425409725491371e-09,-1.761495731747457147e-08,-5.136460886197782731e-09,-1.417264008770025444e-08
+3.108845859999999902e+03,-5.859027348829677742e-09,-1.745658927633700157e-08,-5.073877426410847385e-09,-1.397800689058418990e-08
+3.110774420000000191e+03,-5.812587777276204382e-09,-1.726083475112747458e-08,-5.012432959459102649e-09,-1.371577364157667425e-08
+3.112702990000000227e+03,-5.760505563853990465e-09,-1.711019094628894634e-08,-4.953590484844287843e-09,-1.353517870914302500e-08
+3.114631550000000061e+03,-5.716000640447231811e-09,-1.692285383246672500e-08,-4.895677122731893619e-09,-1.328843592339743022e-08
+3.116560120000000097e+03,-5.666045311279514700e-09,-1.677924027971185004e-08,-4.840224105136368217e-09,-1.312046503253265319e-08
+3.118488679999999931e+03,-5.623316949462334499e-09,-1.659963043922984893e-08,-4.785517230659626183e-09,-1.288778476313600139e-08
+3.120417249999999967e+03,-5.575322129968474402e-09,-1.646244382024664968e-08,-4.733145032354089358e-09,-1.273120430305917092e-08
+3.122345809999999801e+03,-5.534231365452588570e-09,-1.628995751649462030e-08,-4.681359253798785007e-09,-1.251133407123097688e-08
+3.124274379999999837e+03,-5.488050045713615725e-09,-1.615867075822116884e-08,-4.631796044642685408e-09,-1.236506395675882984e-08
+3.126202940000000126e+03,-5.448474118506439847e-09,-1.599277667993237960e-08,-4.582679456453077464e-09,-1.215690027581926796e-08
+3.128131499999999960e+03,-5.403976005726950801e-09,-1.586692734327646578e-08,-4.535685148481389643e-09,-1.201999162376504796e-08
+3.130060069999999996e+03,-5.365805746376779337e-09,-1.570715464781142250e-08,-4.489014321742722108e-09,-1.182255742806647368e-08
+3.131988629999999830e+03,-5.322874235740113018e-09,-1.558633298470853903e-08,-4.444375398054184677e-09,-1.169417112437986342e-08
+3.133917199999999866e+03,-5.286012751354575334e-09,-1.543226409343483817e-08,-4.399952155526814866e-09,-1.150660009812986704e-08
+3.135845760000000155e+03,-5.244543634530352002e-09,-1.531610696008343074e-08,-4.357478734437492762e-09,-1.138599342587288746e-08
+3.137774330000000191e+03,-5.208903992866126915e-09,-1.516736798439265456e-08,-4.315126051842801809e-09,-1.120751253049419720e-08
+3.139702890000000025e+03,-5.168803591323673694e-09,-1.505555148784252644e-08,-4.274648516484447182e-09,-1.109402515426668745e-08
+3.141631460000000061e+03,-5.134307674191067725e-09,-1.491180668152524962e-08,-4.234207969800102557e-09,-1.092394285104844139e-08
+3.143560019999999895e+03,-5.095491462333357021e-09,-1.480404066592738450e-08,-4.195574338955883948e-09,-1.081698575496947755e-08
+3.145488580000000184e+03,-5.062069000058850351e-09,-1.466498780487257891e-08,-4.156903921395778853e-09,-1.065468199074771982e-08
+3.147417150000000220e+03,-5.024460254619850368e-09,-1.456101070637889322e-08,-4.119977418852967420e-09,-1.055372754825095778e-08
+3.149345710000000054e+03,-4.992047280696298951e-09,-1.442637506649456628e-08,-4.082948909844901312e-09,-1.039864292329081168e-08
+3.151274280000000090e+03,-4.955576666057214056e-09,-1.432595176630866057e-08,-4.047606666527057484e-09,-1.030321883725571512e-08
+3.153202839999999924e+03,-4.924115267403993708e-09,-1.419548419825322406e-08,-4.012104514482456027e-09,-1.015484883659336557e-08
+3.155131409999999960e+03,-4.888719418558105440e-09,-1.409840108077672331e-08,-3.978235325997436990e-09,-1.006452954050779233e-08
+3.157059969999999794e+03,-4.858156836495503843e-09,-1.397187435641103501e-08,-3.944154955873794846e-09,-9.922417365215425847e-09
+3.158988539999999830e+03,-4.823777834529226322e-09,-1.387793715480201266e-08,-3.911658091019677210e-09,-9.836818913721491219e-09
+3.160917100000000119e+03,-4.794065861667999710e-09,-1.375514335478489238e-08,-3.878904626311724136e-09,-9.700549878386459570e-09
+3.162845659999999953e+03,-4.760650780856295153e-09,-1.366417531275243548e-08,-3.847688785328243715e-09,-9.619325500220056022e-09
+3.164774229999999989e+03,-4.731745077574747726e-09,-1.354492311272143579e-08,-3.816175778898197252e-09,-9.488521724435545142e-09
+3.166702789999999823e+03,-4.699244952262884836e-09,-1.345676153412782870e-08,-3.786157547812097072e-09,-9.411356101251883319e-09
+3.168631359999999859e+03,-4.671105099226950606e-09,-1.334087575763126004e-08,-3.755806526172275203e-09,-9.285673810818561043e-09
+3.170559920000000147e+03,-4.639474966190092041e-09,-1.325537178707671043e-08,-3.726909977951629302e-09,-9.212280903030659312e-09
+3.172488490000000183e+03,-4.612063572443510839e-09,-1.314269027666469014e-08,-3.697649100983724614e-09,-9.091405314554380491e-09
+3.174417050000000017e+03,-4.581261899374225194e-09,-1.305970693370435089e-08,-3.669804834150319676e-09,-9.021524668220386266e-09
+3.176345620000000054e+03,-4.554544435357097053e-09,-1.295007962417839076e-08,-3.641568340673729838e-09,-8.905167345775561059e-09
+3.178274179999999888e+03,-4.524532770333378212e-09,-1.286949053478076280e-08,-3.614712789369461768e-09,-8.838561320348811535e-09
+3.180202740000000176e+03,-4.498477420903682871e-09,-1.276277863949653630e-08,-3.587440501877132881e-09,-8.726457818712279842e-09
+3.182131310000000212e+03,-4.469219938720861282e-09,-1.268446650961483752e-08,-3.561515191350691020e-09,-8.662908772031907055e-09
+3.184059870000000046e+03,-4.443796902187712129e-09,-1.258054015375169267e-08,-3.535151533875356194e-09,-8.554815024250705578e-09
+3.185988440000000082e+03,-4.415260578800135655e-09,-1.250439709405013934e-08,-3.510102974181030214e-09,-8.494124393445316378e-09
+3.187916999999999916e+03,-4.390442288878714964e-09,-1.240313566753592262e-08,-3.484596911571729842e-09,-8.389815811363554336e-09
+3.189845569999999952e+03,-4.362596216284745498e-09,-1.232906105508657631e-08,-3.460375700034095838e-09,-8.331801033426478591e-09
+3.191774129999999786e+03,-4.338356992868063001e-09,-1.223035194455384105e-08,-3.435680160415500017e-09,-8.231070228110383420e-09
+3.193702690000000075e+03,-4.311172454672692065e-09,-1.215825250910473548e-08,-3.412240838206990292e-09,-8.175563855961339125e-09
+3.195631260000000111e+03,-4.287488193504483893e-09,-1.206198997817999704e-08,-3.388312205710229740e-09,-8.078218645442788033e-09
+3.197559819999999945e+03,-4.260938071523205800e-09,-1.199177797861986385e-08,-3.365612514017365327e-09,-8.025065857883315167e-09
+3.199488389999999981e+03,-4.237786496338593612e-09,-1.189786369245078375e-08,-3.342410667811178901e-09,-7.930928847511924756e-09
+3.201416949999999815e+03,-4.211845516153258587e-09,-1.182945752547217315e-08,-3.320411605355492582e-09,-7.879987224805579204e-09
+3.203345519999999851e+03,-4.189205629906132397e-09,-1.173779879335671663e-08,-3.297899236258573045e-09,-7.788893453470123004e-09
+3.205274080000000140e+03,-4.163850075722609961e-09,-1.167112208565068943e-08,-3.276564641817065269e-09,-7.740031483221243732e-09
+3.207202650000000176e+03,-4.141702175744578096e-09,-1.158163174738761968e-08,-3.254707112859133628e-09,-7.651827624759055214e-09
+3.209131210000000010e+03,-4.116909758996250003e-09,-1.151661290254857541e-08,-3.234003407944234794e-09,-7.604923690917351504e-09
+3.211059769999999844e+03,-4.095235449179836580e-09,-1.142920921841537456e-08,-3.212768623870880511e-09,-7.519467311960195642e-09
+3.212988339999999880e+03,-4.070985069015330383e-09,-1.136578066675027114e-08,-3.192664473993249018e-09,-7.474408505016912431e-09
+3.214916900000000169e+03,-4.049766793518471606e-09,-1.128038586121549096e-08,-3.172022337520565047e-09,-7.391566265564112107e-09
+3.216845470000000205e+03,-4.026038799443681247e-09,-1.121848474555523740e-08,-3.152488776186775630e-09,-7.348248454104067007e-09
+3.218774030000000039e+03,-4.005260125527004957e-09,-1.113502569692644669e-08,-3.132411329092181966e-09,-7.267896169167230744e-09
+3.220702600000000075e+03,-3.982035851572136529e-09,-1.107459249324888011e-08,-3.113421240400423173e-09,-7.226222392006442783e-09
+3.222631159999999909e+03,-3.961681265949112890e-09,-1.099300004862809159e-08,-3.093882379259539684e-09,-7.148243989410206067e-09
+3.224559729999999945e+03,-3.938943069642994921e-09,-1.093397862995087686e-08,-3.075410444226893889e-09,-7.108124109019081629e-09
+3.226488289999999779e+03,-3.918997907215189976e-09,-1.085418730769563109e-08,-3.056385765549791057e-09,-7.032410961479436361e-09
+3.228416850000000068e+03,-3.896729203108098683e-09,-1.079652499455170024e-08,-3.038408409113812257e-09,-6.993761331128477822e-09
+3.230345420000000104e+03,-3.877179471781796217e-09,-1.071847240295527691e-08,-3.019874973577675519e-09,-6.920211406517599716e-09
+3.232273979999999938e+03,-3.855364326759781615e-09,-1.066211878206038937e-08,-3.002369938918025410e-09,-6.882953595937494749e-09
+3.234202549999999974e+03,-3.836196983988191598e-09,-1.058574631969285741e-08,-2.984306436560424472e-09,-6.811471664296826299e-09
+3.236131109999999808e+03,-3.814820390790926678e-09,-1.053065398179605165e-08,-2.967252957256046712e-09,-6.775532748453567355e-09
+3.238059679999999844e+03,-3.796022953798324449e-09,-1.045590566475010435e-08,-2.949639299866997986e-09,-6.706029130235142947e-09
+3.239988240000000133e+03,-3.775070660230813910e-09,-1.040202969056949976e-08,-2.933017891122579817e-09,-6.671341006973402379e-09
+3.241916810000000169e+03,-3.756631271230502872e-09,-1.032885227061520807e-08,-2.915835207916684516e-09,-6.603731383073985808e-09
+3.243845370000000003e+03,-3.736089727655104580e-09,-1.027615005440736176e-08,-2.899627566896934064e-09,-6.570230387755519281e-09
+3.245773929999999837e+03,-3.717997211698588052e-09,-1.020449311835545868e-08,-2.882858196818050790e-09,-6.504435608487047384e-09
+3.247702499999999873e+03,-3.697853421690353032e-09,-1.015292392438007046e-08,-2.867047026312430219e-09,-6.472061950874359566e-09
+3.249631060000000161e+03,-3.680096940694092376e-09,-1.008273887088173648e-08,-2.850674173411728983e-09,-6.408007018750575576e-09
+3.251559630000000197e+03,-3.660338723552351421e-09,-1.003226454166213115e-08,-2.835243359239678637e-09,-6.376705114206305985e-09
+3.253488190000000031e+03,-3.642908048214895419e-09,-9.963505289038167996e-09,-2.819251277082486907e-09,-6.314319504060347986e-09
+3.255416760000000068e+03,-3.623523690685856404e-09,-9.914089250405265359e-09,-2.804185551459109212e-09,-6.284037030175571514e-09
+3.257345319999999901e+03,-3.606409063886821308e-09,-9.846711806325906295e-09,-2.788559384670831525e-09,-6.223254162020474170e-09
+3.259273889999999938e+03,-3.587387386877329196e-09,-9.798319233938315892e-09,-2.773844345938328693e-09,-6.193942016981065511e-09
+3.261202450000000226e+03,-3.570579493266123364e-09,-9.732281565923402462e-09,-2.758570065901241917e-09,-6.134698976352781519e-09
+3.263131010000000060e+03,-3.551909911371672047e-09,-9.684879531044152914e-09,-2.744192193498886566e-09,-6.106311227303155951e-09
+3.265059580000000096e+03,-3.535399756214402735e-09,-9.620141189220266426e-09,-2.729256462295580564e-09,-6.048548321988372338e-09
+3.266988139999999930e+03,-3.517071965359001039e-09,-9.573697775440358957e-09,-2.715202826201993067e-09,-6.021041418349899831e-09
+3.268916709999999966e+03,-3.500851130277572274e-09,-9.510220562208453408e-09,-2.700593176451250600e-09,-5.964702511766791721e-09
+3.270845269999999800e+03,-3.482855362248272475e-09,-9.464705555716883763e-09,-2.686851620378075163e-09,-5.938035659434423944e-09
+3.272773839999999836e+03,-3.466915698499091668e-09,-9.402452639423298059e-09,-2.672556170609966521e-09,-5.883067382201039872e-09
+3.274702400000000125e+03,-3.449242599670646845e-09,-9.357837177730806871e-09,-2.659115185130656249e-09,-5.857202167474699840e-09
+3.276630970000000161e+03,-3.433576301331571058e-09,-9.296773262361081166e-09,-2.645122673671806520e-09,-5.803553912977895832e-09
+3.278559529999999995e+03,-3.416216908349330176e-09,-9.253029753445935759e-09,-2.631971352346010339e-09,-5.778454135054912334e-09
+3.280488089999999829e+03,-3.400816578304158473e-09,-9.193121227956086433e-09,-2.618271165875787002e-09,-5.726078042956698055e-09
+3.282416659999999865e+03,-3.383762209497413775e-09,-9.150223039519884689e-09,-2.605399094868023250e-09,-5.701709395236351603e-09
+3.284345220000000154e+03,-3.368620581125827549e-09,-9.091437184225310574e-09,-2.591981018627406655e-09,-5.650559684215020611e-09
+3.286273790000000190e+03,-3.351863075427167847e-09,-9.049359287231227353e-09,-2.579378451257878008e-09,-5.626890112653965226e-09
+3.288202350000000024e+03,-3.336973256634587917e-09,-8.991664916791294382e-09,-2.566232847033674713e-09,-5.576923430775524825e-09
+3.290130920000000060e+03,-3.320504693004625903e-09,-8.950383103968753454e-09,-2.553890456481232962e-09,-5.553922499830692422e-09
+3.292059479999999894e+03,-3.305860062678262609e-09,-8.893750256954500216e-09,-2.541008158659333135e-09,-5.505097612331960955e-09
+3.293988049999999930e+03,-3.289672829773085195e-09,-8.853241324052265602e-09,-2.528917078027925536e-09,-5.482736555067285031e-09
+3.295916610000000219e+03,-3.275267022976408805e-09,-8.797641198218112547e-09,-2.516289363705616370e-09,-5.435014212806645914e-09
+3.297845170000000053e+03,-3.259353882198595440e-09,-8.757883105951626246e-09,-2.504441220862697415e-09,-5.413265967845349497e-09
+3.299773740000000089e+03,-3.245180696676916838e-09,-8.703287780813844471e-09,-2.492059718320738331e-09,-5.366608638593632155e-09
+3.301702299999999923e+03,-3.229534526174342844e-09,-8.664258947753762610e-09,-2.480446416049150296e-09,-5.345447303181839924e-09
+3.303630869999999959e+03,-3.215588150052139145e-09,-8.610641983639560455e-09,-2.468303272213050317e-09,-5.299819503797523173e-09
+3.305559429999999793e+03,-3.200202172072989187e-09,-8.572321898136807736e-09,-2.456917157621873518e-09,-5.279220689009484167e-09
+3.307487999999999829e+03,-3.186476930085729118e-09,-8.519657624085952180e-09,-2.445004820148755302e-09,-5.234588432194921326e-09
+3.309416560000000118e+03,-3.171344616423696445e-09,-8.482026578226577692e-09,-2.433838596464109674e-09,-5.214529025001887505e-09
+3.311345130000000154e+03,-3.157835039862678254e-09,-8.430290264022818138e-09,-2.422149857040926125e-09,-5.170859873277730586e-09
+3.313273689999999988e+03,-3.142950099255239890e-09,-8.393329311940426786e-09,-2.411196562274741811e-09,-5.151317956184565280e-09
+3.315202249999999822e+03,-3.129650989679838408e-09,-8.342497322161180310e-09,-2.399724594902745023e-09,-5.108581063282421332e-09
+3.317130819999999858e+03,-3.115007281916555002e-09,-8.306188041073480042e-09,-2.388977523454380137e-09,-5.089535708563079227e-09
+3.319059380000000147e+03,-3.101913477969765305e-09,-8.256237187955227012e-09,-2.377715688699503297e-09,-5.047701338144840707e-09
+3.320987950000000183e+03,-3.087505226356241971e-09,-8.220562245375489504e-09,-2.367168549871198216e-09,-5.029132936036617292e-09
+3.322916510000000017e+03,-3.074611819342544685e-09,-8.171470355880380051e-09,-2.356110555324749180e-09,-4.988172784566129345e-09
+3.324845080000000053e+03,-3.060433375684586450e-09,-8.136412868187123460e-09,-2.345757278231354938e-09,-4.970062578728378982e-09
+3.326773639999999887e+03,-3.047735625761351837e-09,-8.088158542120045325e-09,-2.334897102487971697e-09,-4.929949568086582627e-09
+3.328702200000000175e+03,-3.033781606090630458e-09,-8.053702434707727521e-09,-2.324731934848042922e-09,-4.912279852113919066e-09
+3.330630770000000211e+03,-3.021274864166084804e-09,-8.006264820603600708e-09,-2.314063757344093834e-09,-4.872987940665991718e-09
+3.332559330000000045e+03,-3.007539928241880585e-09,-7.972394229251283709e-09,-2.304081084794599001e-09,-4.855741635847080478e-09
+3.334487900000000081e+03,-2.995219839901711539e-09,-7.925753559071220921e-09,-2.293599437546914424e-09,-4.817246121921829839e-09
+3.336416459999999915e+03,-2.981698895166273117e-09,-7.892453373713025064e-09,-2.283793936724545725e-09,-4.800407095613925960e-09
+3.338345029999999952e+03,-2.969561181115643012e-09,-7.846590359438124171e-09,-2.273493524240872427e-09,-4.762684188961326458e-09
+3.340273589999999786e+03,-2.956249303451536202e-09,-7.813846005858768311e-09,-2.263860093942391463e-09,-4.746237082375974319e-09
+3.342202159999999822e+03,-2.944289824107917886e-09,-7.768742001305655393e-09,-2.253735836870884716e-09,-4.709263973193831648e-09
+3.344130720000000110e+03,-2.931182250273401492e-09,-7.736539416221745169e-09,-2.244269586035913703e-09,-4.693194156751138879e-09
+3.346059279999999944e+03,-2.919397065007242923e-09,-7.692176563393590543e-09,-2.234316660454796933e-09,-4.656949073643799177e-09
+3.347987849999999980e+03,-2.906489120030621574e-09,-7.660501996543597668e-09,-2.225012846129922626e-09,-4.641242495891347123e-09
+3.349916409999999814e+03,-2.894874283907350156e-09,-7.616862672459662293e-09,-2.215226519517929704e-09,-4.605704326499651631e-09
+3.351844979999999850e+03,-2.882161571768621406e-09,-7.585703190814676039e-09,-2.206080689628022533e-09,-4.590347806058026060e-09
+3.353773540000000139e+03,-2.870713328386977593e-09,-7.542770511883248302e-09,-2.196456464928034824e-09,-4.555496385337445602e-09
+3.355702110000000175e+03,-2.858191527287504810e-09,-7.512113449500710771e-09,-2.187464294301422829e-09,-4.540477241319954984e-09
+3.357630670000000009e+03,-2.846906237093798779e-09,-7.469871070182820960e-09,-2.177997848804964997e-09,-4.506293197035428467e-09
+3.359559240000000045e+03,-2.834571159934824229e-09,-7.439704185979946182e-09,-2.169155181652278402e-09,-4.491599327074560571e-09
+3.361487799999999879e+03,-2.823445295287983380e-09,-7.398136276281992953e-09,-2.159842358155103538e-09,-4.458064039972361429e-09
+3.363416360000000168e+03,-2.811292945268774458e-09,-7.368447897794020850e-09,-2.151145246582130754e-09,-4.443683988282183572e-09
+3.365344930000000204e+03,-2.800323024511574494e-09,-7.327538959693514310e-09,-2.141981997944942040e-09,-4.410779454989025479e-09
+3.367273490000000038e+03,-2.788349405125284289e-09,-7.298317475865246744e-09,-2.133426551684470889e-09,-4.396702081205753972e-09
+3.369202060000000074e+03,-2.777532172835673959e-09,-7.258052812549831058e-09,-2.124409075229792659e-09,-4.364411180311104397e-09
+3.371130619999999908e+03,-2.765733468345492025e-09,-7.229287149446082105e-09,-2.115991596995845393e-09,-4.350625935292283944e-09
+3.373059189999999944e+03,-2.755065705600836985e-09,-7.189652354037735964e-09,-2.107116184234426065e-09,-4.318932090908397857e-09
+3.374987749999999778e+03,-2.743438214087897509e-09,-7.161331794078423558e-09,-2.098833114672073552e-09,-4.305428888699052423e-09
+3.376916319999999814e+03,-2.732916796664906538e-09,-7.122312896406421859e-09,-2.090096192345415035e-09,-4.274316141218649577e-09
+3.378844880000000103e+03,-2.721456925477210505e-09,-7.094427063474303339e-09,-2.081944103323237415e-09,-4.261085334604852738e-09
+3.380773439999999937e+03,-2.711078877557522681e-09,-7.056010663923064901e-09,-2.073342270811416801e-09,-4.230538402342197535e-09
+3.382702009999999973e+03,-2.699783081529546730e-09,-7.028549358217780365e-09,-2.065317815233004314e-09,-4.217570669062673084e-09
+3.384630569999999807e+03,-2.689545398968628886e-09,-6.990722155632133299e-09,-2.056847706164361349e-09,-4.187574646026539575e-09
+3.386559139999999843e+03,-2.678410349506934352e-09,-6.963675795794218779e-09,-2.048947744338475774e-09,-4.174861241647149800e-09
+3.388487700000000132e+03,-2.668310170437713782e-09,-6.926425029992797350e-09,-2.040606153845930826e-09,-4.145401848005279539e-09
+3.390416270000000168e+03,-2.657332577632813690e-09,-6.899784182479035417e-09,-2.032827614894302577e-09,-4.132934309393826418e-09
+3.392344830000000002e+03,-2.647367120984141568e-09,-6.863097465876087033e-09,-2.024611449643630066e-09,-4.103997774088590489e-09
+3.394273400000000038e+03,-2.636543788186458831e-09,-6.836852986361890821e-09,-2.016951370797748545e-09,-4.091767993123305124e-09
+3.396201959999999872e+03,-2.626710350630411745e-09,-6.800718289850342033e-09,-2.008857643889098694e-09,-4.063341030690996480e-09
+3.398130520000000161e+03,-2.616038224910382681e-09,-6.774861452946433016e-09,-2.001313206488679944e-09,-4.051341319905373307e-09
+3.400059090000000197e+03,-2.606334123974999254e-09,-6.739266951343458664e-09,-1.993338991671309653e-09,-4.023411025108841854e-09
+3.401987650000000031e+03,-2.595810130112937775e-09,-6.713789014037838495e-09,-1.985907392956712407e-09,-4.011633848616670829e-09
+3.403916220000000067e+03,-2.586232864090975982e-09,-6.678723498772317715e-09,-1.978049943606715455e-09,-3.984187927789101063e-09
+3.405844779999999901e+03,-2.575854064791127140e-09,-6.653616117922780849e-09,-1.970728516421253849e-09,-3.972626139290937813e-09
+3.407773349999999937e+03,-2.566401146693812138e-09,-6.619068557130213260e-09,-1.962985137108171122e-09,-3.945652637073414821e-09
+3.409701910000000225e+03,-2.556164684828552834e-09,-6.594323636225532797e-09,-1.955771304124033186e-09,-3.934299379702423924e-09
+3.411630479999999807e+03,-2.546833694599911352e-09,-6.560283306400477733e-09,-1.948139388141961501e-09,-3.907786745642782287e-09
+3.413559040000000095e+03,-2.536736790313664035e-09,-6.535892986172813708e-09,-1.941030657902346388e-09,-3.896635437872959496e-09
+3.415487599999999929e+03,-2.527525423256072948e-09,-6.502349593007431034e-09,-1.933507721780871523e-09,-3.870572585616047767e-09
+3.417416169999999966e+03,-2.517565320381196114e-09,-6.478306110591717838e-09,-1.926501646602284935e-09,-3.859616831311777859e-09
+3.419344729999999799e+03,-2.508471231753733764e-09,-6.445249380526692757e-09,-1.919085210871341512e-09,-3.833992890384984088e-09
+3.421273299999999836e+03,-2.498645348303713556e-09,-6.421545458612052204e-09,-1.912179498905440031e-09,-3.823226697683561782e-09
+3.423201860000000124e+03,-2.489666304939776420e-09,-6.388965528504102856e-09,-1.904867200806830104e-09,-3.798031230792064173e-09
+3.425130430000000160e+03,-2.479972076785783172e-09,-6.365593967542298171e-09,-1.898059596524266305e-09,-3.787448767385689767e-09
+3.427058989999999994e+03,-2.471105903516831265e-09,-6.333481241003576127e-09,-1.890849147840729878e-09,-3.762671677282795473e-09
+3.428987560000000030e+03,-2.461540833482465882e-09,-6.310435045347365119e-09,-1.884137467761652746e-09,-3.752267337347042816e-09
+3.430916119999999864e+03,-2.452785411149102960e-09,-6.278780183475727817e-09,-1.877026651722608844e-09,-3.727898852667282313e-09
+3.432844680000000153e+03,-2.443347114619298721e-09,-6.256052677726933803e-09,-1.870408817400170169e-09,-3.717667317272783141e-09
+3.434773250000000189e+03,-2.434700330259339631e-09,-6.224846466535957698e-09,-1.863395449746775400e-09,-3.693697908152101021e-09
+3.436701810000000023e+03,-2.425386388652205438e-09,-6.202430915439666861e-09,-1.856869376424205899e-09,-3.683633921045788851e-09
+3.438630380000000059e+03,-2.416846278020716809e-09,-6.171664630270868474e-09,-1.849951411111897711e-09,-3.660054500414977259e-09
+3.440558939999999893e+03,-2.407654381636580279e-09,-6.149554606805326512e-09,-1.843515113995637210e-09,-3.650153074061556153e-09
+3.442487509999999929e+03,-2.399218982504616370e-09,-6.119219629486611278e-09,-1.836690531556481436e-09,-3.626954770152954094e-09
+3.444416070000000218e+03,-2.390146879985813667e-09,-6.097408882827755712e-09,-1.830342086740387380e-09,-3.617211104492178957e-09
+3.446344639999999799e+03,-2.381814279004933267e-09,-6.067496819404172587e-09,-1.823608928270741978e-09,-3.594385321519931833e-09
+3.448273200000000088e+03,-2.372859775408467932e-09,-6.045979268751054569e-09,-1.817346470288695264e-09,-3.584794795487933932e-09
+3.450201759999999922e+03,-2.364628151759704497e-09,-6.016482058122393032e-09,-1.810702868913661559e-09,-3.562333268302456152e-09
+3.452130329999999958e+03,-2.355789061461514136e-09,-5.995251670741639950e-09,-1.804524554556678562e-09,-3.552891366225254564e-09
+3.454058889999999792e+03,-2.347656549026132424e-09,-5.966161227591704904e-09,-1.797968631145098634e-09,-3.530785951859212417e-09
+3.455987459999999828e+03,-2.338930830258453082e-09,-5.945212362958527426e-09,-1.791872739265687928e-09,-3.521488453710191178e-09
+3.457916020000000117e+03,-2.330895653021248385e-09,-5.916520922462355507e-09,-1.785402702734795889e-09,-3.499731320582266451e-09
+3.459844590000000153e+03,-2.322281269296565235e-09,-5.895847975399366357e-09,-1.779387529670032021e-09,-3.490574095753064005e-09
+3.461773149999999987e+03,-2.314341694121767346e-09,-5.867547968873997416e-09,-1.773001640615003248e-09,-3.469157647405436461e-09
+3.463701709999999821e+03,-2.305836701737311469e-09,-5.847145592803181524e-09,-1.767065564826508971e-09,-3.460136776657389752e-09
+3.465630279999999857e+03,-2.297990993702655127e-09,-5.819229530714626715e-09,-1.760762101226924820e-09,-3.439053580717301924e-09
+3.467558840000000146e+03,-2.289593409715646574e-09,-5.799092298988821320e-09,-1.754903483987624529e-09,-3.430165162440243504e-09
+3.469487410000000182e+03,-2.281839961285502240e-09,-5.771553098474641050e-09,-1.748680836748282518e-09,-3.409408129135619276e-09
+3.471415970000000016e+03,-2.273547893011787132e-09,-5.751675834858824558e-09,-1.742898118155535661e-09,-3.400648461472714020e-09
+3.473344540000000052e+03,-2.265885091785694517e-09,-5.724506478769215787e-09,-1.736754691489768652e-09,-3.380210647260642152e-09
+3.475273099999999886e+03,-2.257696691511570526e-09,-5.704884140588576319e-09,-1.731046355979263072e-09,-3.371576159114643682e-09
+3.477201669999999922e+03,-2.250122962878487237e-09,-5.678077784125615351e-09,-1.724980598465286478e-09,-3.351450821936496376e-09
+3.479130230000000211e+03,-2.242036426476541322e-09,-5.658705457884173565e-09,-1.719345173159613067e-09,-3.342938067404300540e-09
+3.481058790000000045e+03,-2.234550273473471667e-09,-5.632255527393501250e-09,-1.713355606632115165e-09,-3.323118716888272353e-09
+3.482987360000000081e+03,-2.226563798060500708e-09,-5.613128320438966961e-09,-1.707791629250181016e-09,-3.314724312344671027e-09
+3.484915919999999915e+03,-2.219163676753722935e-09,-5.587028194327451511e-09,-1.701876755331058402e-09,-3.295204528730381645e-09
+3.486844489999999951e+03,-2.211275582931547939e-09,-5.568141544623777084e-09,-1.696382864609502852e-09,-3.286925321625784388e-09
+3.488773049999999785e+03,-2.203960025361259464e-09,-5.542384863713494372e-09,-1.690541255538022200e-09,-3.267698923836037625e-09
+3.490701619999999821e+03,-2.196168631970561120e-09,-5.523734220737001064e-09,-1.685116097483106806e-09,-3.259531813143722056e-09
+3.492630180000000109e+03,-2.188936203624079392e-09,-5.498314777876660872e-09,-1.679346363802150279e-09,-3.240592793644511968e-09
+3.494558750000000146e+03,-2.181239868067270834e-09,-5.479895704449645165e-09,-1.673988621221378063e-09,-3.232534783883942190e-09
+3.496487309999999979e+03,-2.174089166893322319e-09,-5.454807439910007584e-09,-1.668289410427301955e-09,-3.213877302465261722e-09
+3.498415869999999813e+03,-2.166486322863862005e-09,-5.436615706892032533e-09,-1.662997830476234966e-09,-3.205925553280126548e-09
+3.500344439999999850e+03,-2.159415939452759726e-09,-5.411852605699624403e-09,-1.657367796869246035e-09,-3.187543877233215943e-09
+3.502273000000000138e+03,-2.151904978779714042e-09,-5.393883892452840892e-09,-1.652141102879320363e-09,-3.179695536696634036e-09
+3.504201570000000174e+03,-2.144913612513442412e-09,-5.369440276121913444e-09,-1.646578993251993539e-09,-3.161584197586898931e-09
+3.506130130000000008e+03,-2.137493001621192888e-09,-5.351690464603787163e-09,-1.641415970808175250e-09,-3.153836561687408247e-09
+3.508058700000000044e+03,-2.130579342270396805e-09,-5.327560689715282497e-09,-1.635920535984614670e-09,-3.135990186591246042e-09
+3.509987259999999878e+03,-2.123247581832895399e-09,-5.310025761711942764e-09,-1.630820002567378948e-09,-3.128340640716454145e-09
+3.511915829999999914e+03,-2.116410348037966302e-09,-5.286204315493106037e-09,-1.625390025485857888e-09,-3.110754001730886050e-09
+3.513844390000000203e+03,-2.109165971997411331e-09,-5.268880349557623617e-09,-1.620350829374658973e-09,-3.103200017095331996e-09
+3.515772950000000037e+03,-2.102403947345028700e-09,-5.245361938782000255e-09,-1.614985151332916490e-09,-3.085868076680953036e-09
+3.517701520000000073e+03,-2.095245485068202515e-09,-5.228245014607654832e-09,-1.610006143225836550e-09,-3.078407156626276959e-09
+3.519630079999999907e+03,-2.088557406199127744e-09,-5.205024282574372101e-09,-1.604703580535111694e-09,-3.061324911059802915e-09
+3.521558649999999943e+03,-2.081483492673492168e-09,-5.188110757406613686e-09,-1.599783694855132189e-09,-3.053954739471241137e-09
+3.523487209999999777e+03,-2.074868160049512099e-09,-5.165182560928602440e-09,-1.594543120480418640e-09,-3.037117366788810438e-09
+3.525415779999999813e+03,-2.067877423468767612e-09,-5.148468786380111118e-09,-1.589681291773467988e-09,-3.029835652563083867e-09
+3.527344340000000102e+03,-2.061333663318109009e-09,-5.125828098427828768e-09,-1.584501606723917471e-09,-3.013238457049725922e-09
+3.529272910000000138e+03,-2.054424761554653424e-09,-5.109310511739303582e-09,-1.579696796392857097e-09,-3.006042982209844989e-09
+3.531201469999999972e+03,-2.047951425162778169e-09,-5.086952418134766988e-09,-1.574576928807170328e-09,-2.989681390183465090e-09
+3.533130029999999806e+03,-2.041123080002311296e-09,-5.070627627332657974e-09,-1.569828150154019971e-09,-2.982570054309897594e-09
+3.535058599999999842e+03,-2.034719007970024036e-09,-5.048547235898140396e-09,-1.564767028494135241e-09,-2.966439562858794150e-09
+3.536987160000000131e+03,-2.027969898767475604e-09,-5.032411753178327906e-09,-1.560073267792252938e-09,-2.959410237939996489e-09
+3.538915730000000167e+03,-2.021634025907025687e-09,-5.010604454750632900e-09,-1.555069898082804469e-09,-2.943506553405244955e-09
+3.540844290000000001e+03,-2.014962894769052012e-09,-4.994654959406527775e-09,-1.550430192142628580e-09,-2.936557224410596161e-09
+3.542772860000000037e+03,-2.008694143512216175e-09,-4.973116159655445922e-09,-1.545483578778997401e-09,-2.920876115599187830e-09
+3.544701419999999871e+03,-2.002099759109172916e-09,-4.957349406992715924e-09,-1.540896987937410001e-09,-2.914004830053860084e-09
+3.546629989999999907e+03,-1.995897074341141546e-09,-4.936074612326112074e-09,-1.536006159139380414e-09,-2.898542172584995818e-09
+3.548558550000000196e+03,-1.989378231193458446e-09,-4.920487431471220709e-09,-1.531471766508976778e-09,-2.891747038214094015e-09
+3.550487110000000030e+03,-1.983240613004493172e-09,-4.899472329206302083e-09,-1.526635798202195439e-09,-2.876498855391303693e-09
+3.552415680000000066e+03,-1.976796097441151553e-09,-4.884061538075792629e-09,-1.522152684321728678e-09,-2.869777993598637188e-09
+3.554344239999999900e+03,-1.970722500139813340e-09,-4.863301743903384913e-09,-1.517370625263915796e-09,-2.854740319566818114e-09
+3.556272809999999936e+03,-1.964351190045868686e-09,-4.848064396942968410e-09,-1.512937941565284910e-09,-2.848091996738914107e-09
+3.558201370000000225e+03,-1.958340622377970918e-09,-4.827555703217243822e-09,-1.508208887092514248e-09,-2.833261007487698569e-09
+3.560129939999999806e+03,-1.952041385766915624e-09,-4.812488838621371984e-09,-1.503825780796875802e-09,-2.826683498839897267e-09
+3.562058500000000095e+03,-1.946092876658574815e-09,-4.792227127869217421e-09,-1.499148847254675211e-09,-2.812055464205171112e-09
+3.563987070000000131e+03,-1.939864604766996559e-09,-4.777327849630413863e-09,-1.494814485639973462e-09,-2.805547096722673191e-09
+3.565915629999999965e+03,-1.933977202801707379e-09,-4.757309092128020833e-09,-1.490188809745682362e-09,-2.791118377454885191e-09
+3.567844189999999799e+03,-1.927818841240275717e-09,-4.742574646834027340e-09,-1.485902402960472740e-09,-2.784677569752337239e-09
+3.569772759999999835e+03,-1.921991582396390113e-09,-4.722794819654895234e-09,-1.481327117759596287e-09,-2.770444572978005806e-09
+3.571701320000000123e+03,-1.915902034963541641e-09,-4.708222357868971262e-09,-1.477087847689744986e-09,-2.764069707676395583e-09
+3.573629890000000159e+03,-1.910134037730837307e-09,-4.688677679392756775e-09,-1.472562152509605587e-09,-2.750029009923407004e-09
+3.575558449999999993e+03,-1.904112261791731617e-09,-4.674264491740159181e-09,-1.468369243008659470e-09,-2.743718558316525645e-09
+3.577487020000000030e+03,-1.898402630747580103e-09,-4.654951181724678838e-09,-1.463892332087336547e-09,-2.729866776581690110e-09
+3.579415579999999864e+03,-1.892447604589418973e-09,-4.640694617635451210e-09,-1.459745024741217492e-09,-2.723619254636401429e-09
+3.581344149999999900e+03,-1.886795462038563644e-09,-4.621608974658659590e-09,-1.455316110368546534e-09,-2.709953086173826494e-09
+3.583272710000000188e+03,-1.880906184339872374e-09,-4.607506440767496024e-09,-1.451213663967683234e-09,-2.703767052942548568e-09
+3.585201270000000022e+03,-1.875310700140962770e-09,-4.588644914720955234e-09,-1.446831998269955754e-09,-2.690283312128038758e-09
+3.587129840000000058e+03,-1.869486159184548167e-09,-4.574693798793221676e-09,-1.442773665988045179e-09,-2.684157328967004713e-09
+3.589058399999999892e+03,-1.863946459188258619e-09,-4.556052764367055883e-09,-1.438438473246915159e-09,-2.670852826586085537e-09
+3.590986969999999928e+03,-1.858185723498052855e-09,-4.542250658260943492e-09,-1.434423569326571456e-09,-2.664785574002494724e-09
+3.592915530000000217e+03,-1.852700980579804645e-09,-4.523826638425634590e-09,-1.430134112901937162e-09,-2.651657233914314392e-09
+3.594844099999999798e+03,-1.847003106983499502e-09,-4.510171111293694069e-09,-1.426161944767795766e-09,-2.645647391322705655e-09
+3.596772660000000087e+03,-1.841572510046514325e-09,-4.491960699988084961e-09,-1.421917504073325626e-09,-2.632692208469839588e-09
+3.598701230000000123e+03,-1.835936573801375086e-09,-4.478449372291102800e-09,-1.417987394430536666e-09,-2.626738492641181144e-09
+3.600629789999999957e+03,-1.830559327383759294e-09,-4.460449232611598123e-09,-1.413787264478183504e-09,-2.613953530961599802e-09
+3.602558349999999791e+03,-1.824984450604761476e-09,-4.447079845584462602e-09,-1.409898572152007248e-09,-2.608054731868352935e-09
+3.604486919999999827e+03,-1.819659745615088300e-09,-4.429286637232496074e-09,-1.405742041833357874e-09,-2.595437085174200954e-09
+3.606415480000000116e+03,-1.814145009895703782e-09,-4.416056838286868973e-09,-1.401894097292390806e-09,-2.589591952861551247e-09
+3.608344050000000152e+03,-1.808872110187108327e-09,-4.398467429092921535e-09,-1.397780513011244007e-09,-2.577138854721457705e-09
+3.610272609999999986e+03,-1.803416643412079792e-09,-4.385374984654886085e-09,-1.393972682237150542e-09,-2.571346210496517736e-09
+3.612201180000000022e+03,-1.798194798180324094e-09,-4.367986234878648270e-09,-1.389901383220188558e-09,-2.559054920049380785e-09
+3.614129739999999856e+03,-1.792797744931508863e-09,-4.355028957498995351e-09,-1.386133045813043133e-09,-2.553313617703866707e-09
+3.616058300000000145e+03,-1.787626245414854322e-09,-4.337837857900590754e-09,-1.382103405736391113e-09,-2.541181490948204918e-09
+3.617986870000000181e+03,-1.782286738702931385e-09,-4.325013537046636192e-09,-1.378373934014843525e-09,-2.535490380195971842e-09
+3.619915430000000015e+03,-1.777164833967303080e-09,-4.308017002446542227e-09,-1.374385298856123568e-09,-2.523514761316531370e-09
+3.621844000000000051e+03,-1.771882078722697319e-09,-4.295323608183907763e-09,-1.370694119258912448e-09,-2.517872793608923181e-09
+3.623772559999999885e+03,-1.766809059495241954e-09,-4.278518681630517475e-09,-1.366745868906369072e-09,-2.506051120679578577e-09
+3.625701129999999921e+03,-1.761582248025062782e-09,-4.265954157884736281e-09,-1.363092399658699318e-09,-2.500457240865241236e-09
+3.627629690000000210e+03,-1.756557418225998748e-09,-4.249337940369489229e-09,-1.359183926824459818e-09,-2.488787008267228012e-09
+3.629558259999999791e+03,-1.751385757998432836e-09,-4.236900272642547873e-09,-1.355567598327717042e-09,-2.483240189546775766e-09
+3.631486820000000080e+03,-1.746408434431688174e-09,-4.220469921684097190e-09,-1.351698308203476945e-09,-2.471718946398010070e-09
+3.633415379999999914e+03,-1.741291174348583536e-09,-4.208157200754088463e-09,-1.348118582311184379e-09,-2.466218223025330083e-09
+3.635343949999999950e+03,-1.736360659771169202e-09,-4.191909864295854616e-09,-1.344287872628618625e-09,-2.454843538051535768e-09
+3.637272509999999784e+03,-1.731297009672154126e-09,-4.179720090229357646e-09,-1.340744183313918874e-09,-2.449387903109788935e-09
+3.639201079999999820e+03,-1.726412672655445126e-09,-4.163653100224040571e-09,-1.336951503038121565e-09,-2.438157464445551551e-09
+3.641129640000000109e+03,-1.721401883398385489e-09,-4.151584377084895496e-09,-1.333443315296204569e-09,-2.432745970727353910e-09
+3.643058210000000145e+03,-1.716563077624703292e-09,-4.135695052551383356e-09,-1.329688105101938142e-09,-2.421657482808871303e-09
+3.644986769999999979e+03,-1.711604413863723587e-09,-4.123745521956646782e-09,-1.326214894848148771e-09,-2.416289207917565088e-09
+3.646915340000000015e+03,-1.706810504747746824e-09,-4.108031233185683293e-09,-1.322496606623473067e-09,-2.405340424153213987e-09
+3.648843899999999849e+03,-1.701903244615936905e-09,-4.096199073376296668e-09,-1.319057860404980155e-09,-2.400014469701856527e-09
+3.650772460000000137e+03,-1.697153634507968195e-09,-4.080657302326393585e-09,-1.315375975708839005e-09,-2.389203222981576089e-09
+3.652701030000000173e+03,-1.692297043836350653e-09,-4.068940665668344334e-09,-1.311971171676003382e-09,-2.383918682010398876e-09
+3.654629590000000007e+03,-1.687591095101205112e-09,-4.053568819259504410e-09,-1.308325145027759512e-09,-2.373242787542059886e-09
+3.656558160000000044e+03,-1.682784503783135390e-09,-4.041966016841467394e-09,-1.304953809095026919e-09,-2.367998839605100557e-09
+3.658486719999999877e+03,-1.678121615458193797e-09,-4.026761612005859421e-09,-1.301343124315239147e-09,-2.357456189950108219e-09
+3.660415289999999914e+03,-1.673364340243423742e-09,-4.015270926633388698e-09,-1.298004773284584509e-09,-2.352252004178094481e-09
+3.662343850000000202e+03,-1.668743922071069855e-09,-4.000231526892553693e-09,-1.294428924297510573e-09,-2.341840535823179391e-09
+3.664272419999999784e+03,-1.664035292005353483e-09,-3.988851274546779808e-09,-1.291123084540149179e-09,-2.336675302441572875e-09
+3.666200980000000072e+03,-1.659456764193303418e-09,-3.973974488925803428e-09,-1.287581575117893606e-09,-2.326392994641249360e-09
+3.668129539999999906e+03,-1.654796144725014564e-09,-3.962703076697682042e-09,-1.284307800279561203e-09,-2.321265954543587444e-09
+3.670058109999999942e+03,-1.650258913330286998e-09,-3.947986499946656624e-09,-1.280800125843977550e-09,-2.311110797976079025e-09
+3.671986669999999776e+03,-1.645645632663888811e-09,-3.936822248419209409e-09,-1.277557942587541524e-09,-2.306021151009184976e-09
+3.673915239999999812e+03,-1.641149162747331145e-09,-3.922263636788036320e-09,-1.274083643992226227e-09,-2.295991237721815337e-09
+3.675843800000000101e+03,-1.636582585196504184e-09,-3.911204956761680615e-09,-1.270872605961875291e-09,-2.290938233509060347e-09
+3.677772370000000137e+03,-1.632126326985799567e-09,-3.896802049559020769e-09,-1.267431215064669364e-09,-2.281031664470372595e-09
+3.679700929999999971e+03,-1.627605828102679039e-09,-3.885847381938289822e-09,-1.264250884540807811e-09,-2.276014571210092207e-09
+3.681629500000000007e+03,-1.623189241396022154e-09,-3.871597959924956273e-09,-1.260841942101956016e-09,-2.266229485880755882e-09
+3.683558059999999841e+03,-1.618714207724268789e-09,-3.860745775005585360e-09,-1.257691889785802996e-09,-2.261247589773032021e-09
+3.685486620000000130e+03,-1.614336785040764577e-09,-3.846647715439968686e-09,-1.254314962446878579e-09,-2.251582193808732688e-09
+3.687415190000000166e+03,-1.609906590515209843e-09,-3.835896456240675365e-09,-1.251194750054087647e-09,-2.246634769829400695e-09
+3.689343750000000000e+03,-1.605567786595286080e-09,-3.821947563393467009e-09,-1.247849378374214470e-09,-2.237087247717900639e-09
+3.691272320000000036e+03,-1.601181862606922214e-09,-3.811295813512757311e-09,-1.244758610186016751e-09,-2.232173645450303642e-09
+3.693200879999999870e+03,-1.596881164731889350e-09,-3.797493986939037659e-09,-1.241444360350804806e-09,-2.222742246329738423e-09
+3.695129449999999906e+03,-1.592538929380051864e-09,-3.786940300772781335e-09,-1.238382631102190816e-09,-2.217861802748541042e-09
+3.697058010000000195e+03,-1.588275833598867480e-09,-3.773283477847601409e-09,-1.235099077365018890e-09,-2.208544810476226520e-09
+3.698986579999999776e+03,-1.583976715051226976e-09,-3.762826436532397438e-09,-1.232065989414800725e-09,-2.203696878466476533e-09
+3.700915140000000065e+03,-1.579750725992699735e-09,-3.749312591604783235e-09,-1.228812713903554537e-09,-2.194492610748689219e-09
+3.702843699999999899e+03,-1.575494184664612833e-09,-3.738950855863748180e-09,-1.225807893543583881e-09,-2.189676585944175610e-09
+3.704772269999999935e+03,-1.571304792958296047e-09,-3.725577945983681652e-09,-1.222584469578998351e-09,-2.180583366191620600e-09
+3.706700830000000224e+03,-1.567090253911605482e-09,-3.715310094580068707e-09,-1.219607517224176257e-09,-2.175798604251880238e-09
+3.708629399999999805e+03,-1.562937003403241750e-09,-3.702076219607005886e-09,-1.216413558770454830e-09,-2.166814842981677920e-09
+3.710557960000000094e+03,-1.558763923741144547e-09,-3.691900910267623286e-09,-1.213464098568969195e-09,-2.162060741721175773e-09
+3.712486530000000130e+03,-1.554646343716908201e-09,-3.678804150618215179e-09,-1.210299210271953043e-09,-2.153184853228643197e-09
+3.714415089999999964e+03,-1.550514189781180439e-09,-3.668720065436336846e-09,-1.207376873290930143e-09,-2.148460824551203333e-09
+3.716343660000000000e+03,-1.546431817403001373e-09,-3.655758535338342500e-09,-1.204240666953274039e-09,-2.139691253757517218e-09
+3.718272219999999834e+03,-1.542340064579699037e-09,-3.645764380220649707e-09,-1.201345091015311510e-09,-2.134996723239884519e-09
+3.720200780000000123e+03,-1.538292466207391068e-09,-3.632936278019917427e-09,-1.198237201258677236e-09,-2.126331970922894844e-09
+3.722129350000000159e+03,-1.534240577249619052e-09,-3.623030731116748208e-09,-1.195368014954080440e-09,-2.121666351451985956e-09
+3.724057909999999993e+03,-1.530227283624772528e-09,-3.610334184894791530e-09,-1.192288051429409069e-09,-2.113104895298638321e-09
+3.725986480000000029e+03,-1.526214773125829298e-09,-3.600516049703905606e-09,-1.189444921591368088e-09,-2.108467664866324821e-09
+3.727915039999999863e+03,-1.522235344067189409e-09,-3.587949270766437077e-09,-1.186392516593351495e-09,-2.100008037284764363e-09
+3.729843609999999899e+03,-1.518261713426407767e-09,-3.578217321468890508e-09,-1.183575100375592783e-09,-2.095398660137121160e-09
+3.731772170000000187e+03,-1.514315715993621591e-09,-3.565778552082225379e-09,-1.180549892717849708e-09,-2.087039421297411039e-09
+3.733700740000000224e+03,-1.510380474925657407e-09,-3.556131584610647875e-09,-1.177757853422216399e-09,-2.082457373830335030e-09
+3.735629300000000057e+03,-1.506467483270271800e-09,-3.543819097337383356e-09,-1.174759488288941321e-09,-2.074197111003013446e-09
+3.737557859999999891e+03,-1.502570170264377931e-09,-3.534255977705544533e-09,-1.171992510430017717e-09,-2.069641906190978376e-09
+3.739486429999999928e+03,-1.498689744853534979e-09,-3.522068025955051371e-09,-1.169020624025638680e-09,-2.061479208337113227e-09
+3.741414990000000216e+03,-1.494829864933259982e-09,-3.512587542859751527e-09,-1.166278367443035013e-09,-2.056950320784675724e-09
+3.743343559999999798e+03,-1.490981614483886046e-09,-3.500522507153586766e-09,-1.163332632604014493e-09,-2.048883852505444512e-09
+3.745272120000000086e+03,-1.487158701303920224e-09,-3.491123518943222382e-09,-1.160614778215102003e-09,-2.044380793003749158e-09
+3.747200690000000122e+03,-1.483342220383106770e-09,-3.479179758903741815e-09,-1.157694858386567774e-09,-2.036409219083507292e-09
+3.749129249999999956e+03,-1.479555815255356111e-09,-3.469861143818670986e-09,-1.155001092716252619e-09,-2.031931509234603925e-09
+3.751057809999999790e+03,-1.475770724958661634e-09,-3.458037094003791406e-09,-1.152106671904342980e-09,-2.024053542954643556e-09
+3.752986379999999826e+03,-1.472020356699989624e-09,-3.448797702621809349e-09,-1.149436672215212600e-09,-2.019600691020505034e-09
+3.754914940000000115e+03,-1.468266244354625062e-09,-3.437091730063564096e-09,-1.146567410500644596e-09,-2.011815021745012705e-09
+3.756843510000000151e+03,-1.464551489303692485e-09,-3.427930526720964497e-09,-1.143920889029670561e-09,-2.007386594155182101e-09
+3.758772069999999985e+03,-1.460827968682981914e-09,-3.416341072703834449e-09,-1.141076466929315878e-09,-1.999691958873855834e-09
+3.760700640000000021e+03,-1.457148390208077844e-09,-3.407256992765762451e-09,-1.138453126280768923e-09,-1.995287507874180480e-09
+3.762629199999999855e+03,-1.453455081232326301e-09,-3.395782524655787411e-09,-1.135633229753433643e-09,-1.987682666534592594e-09
+3.764557769999999891e+03,-1.449810249762692282e-09,-3.386774521716772161e-09,-1.133032777656079863e-09,-1.983301754020888671e-09
+3.766486330000000180e+03,-1.446146778376850308e-09,-3.375413532418518780e-09,-1.130237097983888419e-09,-1.975785489001925349e-09
+3.768414890000000014e+03,-1.442536290484997376e-09,-3.366480623036731829e-09,-1.127659261360357272e-09,-1.971427709044519972e-09
+3.770343460000000050e+03,-1.438902269316260823e-09,-3.355231585349452926e-09,-1.124887480851123328e-09,-1.963998801863254802e-09
+3.772272019999999884e+03,-1.435325689748838680e-09,-3.346372712844027034e-09,-1.122331963042839754e-09,-1.959663711821137398e-09
+3.774200589999999920e+03,-1.431720775824712237e-09,-3.335234214736852474e-09,-1.119583797584764491e-09,-1.952321011227185601e-09
+3.776129150000000209e+03,-1.428177695369317422e-09,-3.326448385086862203e-09,-1.117050321032943613e-09,-1.948008200366702010e-09
+3.778057719999999790e+03,-1.424601532001487790e-09,-3.315418992955147780e-09,-1.114325477196375274e-09,-1.940750553020964216e-09
+3.779986280000000079e+03,-1.421091547966668850e-09,-3.306705228860141496e-09,-1.111813769034953559e-09,-1.936459619229021878e-09
+3.781914850000000115e+03,-1.417543784030797496e-09,-3.295783532596769105e-09,-1.109111958270250106e-09,-1.929285892259627639e-09
+3.783843409999999949e+03,-1.414066500118886926e-09,-3.287140873124653083e-09,-1.106621750224961683e-09,-1.925016441807842416e-09
+3.785771969999999783e+03,-1.410546808435160304e-09,-3.276325528843532164e-09,-1.103942702407356194e-09,-1.917925544109318924e-09
+3.787700539999999819e+03,-1.407101816128283817e-09,-3.267752985894852643e-09,-1.101473717048546523e-09,-1.913677169680531226e-09
+3.789629100000000108e+03,-1.403609837731467909e-09,-3.257042585435247540e-09,-1.098817139317896542e-09,-1.906667985968699647e-09
+3.791557670000000144e+03,-1.400196771796382830e-09,-3.248539273407108023e-09,-1.096369131025598971e-09,-1.902440331902918990e-09
+3.793486229999999978e+03,-1.396732171615381107e-09,-3.237932474323119106e-09,-1.093734748862945919e-09,-1.895511788006252892e-09
+3.795414800000000014e+03,-1.393350654200285789e-09,-3.229497479361527417e-09,-1.091307462557970106e-09,-1.891304484389740365e-09
+3.797343359999999848e+03,-1.389913102309224986e-09,-3.218992960848973326e-09,-1.088695005926022651e-09,-1.884455524838559309e-09
+3.799271929999999884e+03,-1.386562761476709204e-09,-3.210625384145621817e-09,-1.086288190743511274e-09,-1.880268209271195822e-09
+3.801200490000000173e+03,-1.383151932996434514e-09,-3.200221846604326504e-09,-1.083697393993652860e-09,-1.873497796884390220e-09
+3.803129050000000007e+03,-1.379832420406151064e-09,-3.191920845500456075e-09,-1.081310816341494503e-09,-1.869330135095917876e-09
+3.805057620000000043e+03,-1.376447977611272620e-09,-3.181616968704390694e-09,-1.078741404975718829e-09,-1.862637229774417049e-09
+3.806986179999999877e+03,-1.373158914874139576e-09,-3.173381631749079690e-09,-1.076374808900772091e-09,-1.858488852762551951e-09
+3.808914749999999913e+03,-1.369800560636204232e-09,-3.163176199042513479e-09,-1.073826539032187822e-09,-1.851872473735716988e-09
+3.810843310000000201e+03,-1.366541592892845370e-09,-3.155005670732085645e-09,-1.071479685793669094e-09,-1.847743040456607594e-09
+3.812771879999999783e+03,-1.363209016900326634e-09,-3.144897443612287331e-09,-1.068952304402149366e-09,-1.841202203049476487e-09
+3.814700440000000071e+03,-1.359979794769633414e-09,-3.136790882286739224e-09,-1.066624959134103150e-09,-1.837091379198954011e-09
+3.816629010000000108e+03,-1.356672691384916466e-09,-3.126778641809708197e-09,-1.064118217238684972e-09,-1.830625115483064140e-09
+3.818557569999999942e+03,-1.353472870861323987e-09,-3.118735219369856841e-09,-1.061810148870605149e-09,-1.826532573317223769e-09
+3.820486129999999775e+03,-1.350190956169906027e-09,-3.108817805463482187e-09,-1.059323814116540246e-09,-1.820139951654356746e-09
+3.822414699999999812e+03,-1.347020181384692014e-09,-3.100836667405959603e-09,-1.057034782626275710e-09,-1.816065349924466708e-09
+3.824343260000000100e+03,-1.343763141556127787e-09,-3.091012859016779190e-09,-1.054568601095683209e-09,-1.809745414701924047e-09
+3.826271830000000136e+03,-1.340621096234227182e-09,-3.083093243612898174e-09,-1.052298395544609264e-09,-1.805688458369133353e-09
+3.828200389999999970e+03,-1.337388639133966105e-09,-3.073361878182756080e-09,-1.049852129891638539e-09,-1.799440289768391488e-09
+3.830128960000000006e+03,-1.334274994800259048e-09,-3.065502996392682241e-09,-1.047600530136984899e-09,-1.795400669755981213e-09
+3.832057519999999840e+03,-1.331066832627600405e-09,-3.055862929417148125e-09,-1.045173946739508423e-09,-1.789223363309099879e-09
+3.833986089999999876e+03,-1.327981265793710351e-09,-3.048064004700703589e-09,-1.042940736135526853e-09,-1.785200776439841484e-09
+3.835914650000000165e+03,-1.324797115001430077e-09,-3.038514109373315552e-09,-1.040533605021178879e-09,-1.779093442702107817e-09
+3.837843209999999999e+03,-1.321739323588386940e-09,-3.030774415542184828e-09,-1.038318582567869788e-09,-1.775087610614931467e-09
+3.839771780000000035e+03,-1.318578888289303255e-09,-3.021313544314002735e-09,-1.035930665122737188e-09,-1.769049355784843987e-09
+3.841700339999999869e+03,-1.315548541861066196e-09,-3.013632290630655455e-09,-1.033733608644442116e-09,-1.765059967386492015e-09
+3.843628909999999905e+03,-1.312411563429550729e-09,-3.004259389503879916e-09,-1.031364694296936568e-09,-1.759089950368185697e-09
+3.845557470000000194e+03,-1.309408352917500577e-09,-2.996635835454448748e-09,-1.029185397227007713e-09,-1.755116719276591370e-09
+3.847486039999999775e+03,-1.306294560100614000e-09,-2.987349828658452318e-09,-1.026835266527072235e-09,-1.749214093810505949e-09
+3.849414600000000064e+03,-1.303318181068164135e-09,-2.979783245260040048e-09,-1.024673525526262879e-09,-1.745256738951399665e-09
+3.851343170000000100e+03,-1.300227306562665417e-09,-2.970583073374468543e-09,-1.022341962395620780e-09,-1.739420672567797816e-09
+3.853271729999999934e+03,-1.297277459121486780e-09,-2.963072742947349977e-09,-1.020197577288739794e-09,-1.735478918037419734e-09
+3.855200290000000223e+03,-1.294209255423259335e-09,-2.953957399148128461e-09,-1.017884380745144019e-09,-1.729708610025921801e-09
+3.857128859999999804e+03,-1.291285628229245123e-09,-2.946502578534326143e-09,-1.015757142669481092e-09,-1.725782166706955269e-09
+3.859057420000000093e+03,-1.288239819671756446e-09,-2.937470998245198058e-09,-1.013462091302830080e-09,-1.720076792872741491e-09
+3.860985990000000129e+03,-1.285342137737693956e-09,-2.930071028603752454e-09,-1.011351818108990331e-09,-1.716165413239288190e-09
+3.862914549999999963e+03,-1.282318468443337058e-09,-2.921122199557435023e-09,-1.009074705572683279e-09,-1.710524180760661862e-09
+3.864843119999999999e+03,-1.279446445039061481e-09,-2.913776395802101335e-09,-1.006981206211670149e-09,-1.706627603638933974e-09
+3.866771679999999833e+03,-1.276444662802063640e-09,-2.904909320830780008e-09,-1.004721829279721423e-09,-1.701049732351509739e-09
+3.868700249999999869e+03,-1.273598015428154035e-09,-2.897617008317654724e-09,-1.002644915628237305e-09,-1.697167701228084588e-09
+3.870628810000000158e+03,-1.270617871648905479e-09,-2.888830705054774223e-09,-1.000403074136383040e-09,-1.691652423356608630e-09
+3.872557369999999992e+03,-1.267796337321474754e-09,-2.881591254511590877e-09,-9.983425723246314245e-10,-1.687784703776438478e-09
+3.874485940000000028e+03,-1.264837571581987759e-09,-2.872884719972564533e-09,-9.961180577288007944e-10,-1.682331246162101684e-09
+3.876414499999999862e+03,-1.262040860559251872e-09,-2.865697441586459944e-09,-9.940737738470750675e-10,-1.678477572893369742e-09
+3.878343069999999898e+03,-1.259103246761741889e-09,-2.857069757571373428e-09,-9.918664034070675027e-10,-1.673085209430686142e-09
+3.880271630000000187e+03,-1.256331088794359276e-09,-2.849934006825646192e-09,-9.898381577794204509e-10,-1.669245339239307672e-09
+3.882200200000000223e+03,-1.253414388776310806e-09,-2.841384233619836234e-09,-9.876477401764542300e-10,-1.663913337753328948e-09
+3.884128760000000057e+03,-1.250666517555311531e-09,-2.834299375649730758e-09,-9.856353558365639511e-10,-1.660087031604380498e-09
+3.886057330000000093e+03,-1.247770496511765582e-09,-2.825826587184609990e-09,-9.834617025928068920e-10,-1.654814671277414726e-09
+3.887985889999999927e+03,-1.245046649599885008e-09,-2.818791996589905076e-09,-9.814650052330851276e-10,-1.651001694226471758e-09
+3.889914450000000215e+03,-1.242171090848790043e-09,-2.810395313913922247e-09,-9.793079416564590867e-10,-1.645788282142245327e-09
+3.891843019999999797e+03,-1.239470994788559450e-09,-2.803410340829413385e-09,-9.773267485817498014e-10,-1.641988386443716348e-09
+3.893771580000000085e+03,-1.236615655126631422e-09,-2.795088830264452611e-09,-9.751860806438477464e-10,-1.636833206791880137e-09
+3.895700150000000122e+03,-1.233939069962901130e-09,-2.788152901723916183e-09,-9.732202337957066999e-10,-1.633046182320353911e-09
+3.897628709999999955e+03,-1.231103724312633143e-09,-2.779905676447877128e-09,-9.710957812393437280e-10,-1.627948546853857522e-09
+3.899557279999999992e+03,-1.228450398823638901e-09,-2.773018194362192802e-09,-9.691451139919213591e-10,-1.624174170319791284e-09
+3.901485839999999826e+03,-1.225634825238818337e-09,-2.764844380064809403e-09,-9.670366992039246716e-10,-1.619133401144520617e-09
+3.903414400000000114e+03,-1.223004526240964904e-09,-2.758004787845134767e-09,-9.651010581080223278e-10,-1.615371469219846786e-09
+3.905342970000000150e+03,-1.220208491425573782e-09,-2.749903489703578403e-09,-9.630084953638591561e-10,-1.610386882276965821e-09
+3.907271529999999984e+03,-1.217600960320094443e-09,-2.743111173566970401e-09,-9.610877078926899445e-10,-1.606637162517977190e-09
+3.909200100000000020e+03,-1.214824262969572094e-09,-2.735081574458909434e-09,-9.590108355226543570e-10,-1.601708116286150277e-09
+3.911128659999999854e+03,-1.212239259185756653e-09,-2.728335962076902354e-09,-9.571047423177176367e-10,-1.597970396172555211e-09
+3.913057229999999890e+03,-1.209481686431653396e-09,-2.720377223480266155e-09,-9.550433903745246830e-10,-1.593096242290602713e-09
+3.914985790000000179e+03,-1.206918972829094767e-09,-2.713677750775814545e-09,-9.531518344121291156e-10,-1.589370312699983899e-09
+3.916914360000000215e+03,-1.204180314729405574e-09,-2.705789045483980281e-09,-9.511058354219595051e-10,-1.584550412115258652e-09
+3.918842920000000049e+03,-1.201639657540385825e-09,-2.699135156469957721e-09,-9.492286619711743628e-10,-1.580836067230522754e-09
+3.920771479999999883e+03,-1.198919720968303235e-09,-2.691315699747896486e-09,-9.471978612513914803e-10,-1.576069805533706007e-09
+3.922700049999999919e+03,-1.196400875804790068e-09,-2.684706814883189178e-09,-9.453349074778370136e-10,-1.572366827134669480e-09
+3.924628610000000208e+03,-1.193699442489093284e-09,-2.676955769365918294e-09,-9.433191319609009777e-10,-1.567653567234286095e-09
+3.926557179999999789e+03,-1.191202196202680842e-09,-2.670391380123518604e-09,-9.414702580286474238e-10,-1.563961771602590752e-09
+3.928485740000000078e+03,-1.188519064704400616e-09,-2.662707950440406228e-09,-9.394693474489047457e-10,-1.559300900545105675e-09
+3.930414310000000114e+03,-1.186043193310879649e-09,-2.656187524146890318e-09,-9.376344052627469687e-10,-1.555620091231209578e-09
+3.932342869999999948e+03,-1.183378164938998217e-09,-2.648570924712567942e-09,-9.356482016969318843e-10,-1.551011004051514832e-09
+3.934271439999999984e+03,-1.180923447609062724e-09,-2.642093936150644810e-09,-9.338270452965833744e-10,-1.547340987542996495e-09
+3.936199999999999818e+03,-1.178276326381651209e-09,-2.634543390655057860e-09,-9.318553931412951639e-10,-1.542783086826855589e-09
+3.938128560000000107e+03,-1.175842558860485474e-09,-2.628109352215106275e-09,-9.300478886834365052e-10,-1.539123687470043129e-09
+3.940057130000000143e+03,-1.173213137997384625e-09,-2.620624062715673124e-09,-9.280906246200509639e-10,-1.534616367829857316e-09
+3.941985689999999977e+03,-1.170800092042173190e-09,-2.614232433045127128e-09,-9.262966202132367543e-10,-1.530967382544563746e-09
+3.943914260000000013e+03,-1.168188194447323615e-09,-2.606811670400200539e-09,-9.243536033307630165e-10,-1.526510075155510325e-09
+3.945842819999999847e+03,-1.165795658392983024e-09,-2.600461945690832930e-09,-9.225729592033188833e-10,-1.522871318655026887e-09
+3.947771389999999883e+03,-1.163201096012776463e-09,-2.593104957185076085e-09,-9.206440408007282480e-10,-1.518463445152155209e-09
+3.949699950000000172e+03,-1.160828861153200513e-09,-2.586796640427612387e-09,-9.188766191749555536e-10,-1.514834734673319627e-09
+3.951628520000000208e+03,-1.158251448530384037e-09,-2.579502679108661999e-09,-9.169616528769757510e-10,-1.510475721255763050e-09
+3.953557080000000042e+03,-1.155899309073468934e-09,-2.573235279910310629e-09,-9.152073179371273991e-10,-1.506856876433862524e-09
+3.955485639999999876e+03,-1.153338876364322465e-09,-2.566003632084533059e-09,-9.133061694414272889e-10,-1.502546166873014141e-09
+3.957414209999999912e+03,-1.151006616363961123e-09,-2.559776637302500690e-09,-9.115647776060175021e-10,-1.498936995174464126e-09
+3.959342770000000201e+03,-1.148462970177036274e-09,-2.552606532379200972e-09,-9.096772956154620307e-10,-1.494674005377179391e-09
+3.961271339999999782e+03,-1.146150402664150375e-09,-2.546419493655162218e-09,-9.079487246689744780e-10,-1.491074345332302358e-09
+3.963199900000000071e+03,-1.143623365362799787e-09,-2.539310188639040370e-09,-9.060747702805763608e-10,-1.486858503911558973e-09
+3.965128470000000107e+03,-1.141330293040770605e-09,-2.533162634126592627e-09,-9.043588901173610940e-10,-1.483268181361460237e-09
+3.967057029999999941e+03,-1.138819689701632093e-09,-2.526113378704715230e-09,-9.024983273290201960e-10,-1.479098910443768434e-09
+3.968985599999999977e+03,-1.136545918036747191e-09,-2.520004842162056185e-09,-9.007950096979058163e-10,-1.475517752809383287e-09
+3.970914159999999811e+03,-1.134051576608051015e-09,-2.513014869703763225e-09,-8.989477058862787332e-10,-1.471394460450508243e-09
+3.972842720000000099e+03,-1.131796926407652759e-09,-2.506944918158011078e-09,-8.972568337653155026e-10,-1.467822310204353064e-09
+3.974771290000000135e+03,-1.129318665415209029e-09,-2.500013401869555345e-09,-8.954226511638596784e-10,-1.463744363255918898e-09
+3.976699849999999969e+03,-1.127082934920222715e-09,-2.493981550425043224e-09,-8.937440905138051793e-10,-1.460181035532941277e-09
+3.978628420000000006e+03,-1.124620601982729775e-09,-2.487107658075132956e-09,-8.919229161389572028e-10,-1.456147776314114641e-09
+3.980556979999999839e+03,-1.122403604870760063e-09,-2.481113453686482798e-09,-8.902565442201971906e-10,-1.452593099770480543e-09
+3.982485549999999876e+03,-1.119957040043004681e-09,-2.474296200261148421e-09,-8.884482651511257872e-10,-1.448603751607358649e-09
+3.984414110000000164e+03,-1.117758592798794761e-09,-2.468339191560092505e-09,-8.867939611131906717e-10,-1.445057552509192021e-09
+3.986342680000000200e+03,-1.115327644528034594e-09,-2.461577316360895561e-09,-8.849984826834422485e-10,-1.441111106736276157e-09
+3.988271240000000034e+03,-1.113147566629616775e-09,-2.455657049861639636e-09,-8.833561277003988797e-10,-1.437573204940152591e-09
+3.990199799999999868e+03,-1.110732113718761091e-09,-2.448948591603598424e-09,-8.815734087934826076e-10,-1.433668055067074415e-09
+3.992128369999999904e+03,-1.108570215992372153e-09,-2.443064574922914056e-09,-8.799428773640905137e-10,-1.430138240288903792e-09
+3.994056930000000193e+03,-1.106170172980796466e-09,-2.436404838456383820e-09,-8.781730163971008867e-10,-1.426270505830551946e-09
+3.995985499999999774e+03,-1.104026296406228031e-09,-2.430556586392240012e-09,-8.765542052389269364e-10,-1.422748539812785849e-09
+3.997914060000000063e+03,-1.101642108970170088e-09,-2.423916824932671491e-09,-8.747987115015089606e-10,-1.418894186290831660e-09
```

### Comparing `simulateIRAS-0.1.0.post5/examples/simpleSimulation/simpleSimulation.py` & `simulateIRAS-0.1.0.post6/examples/simpleSimulation/simpleSimulation.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,30 +32,16 @@
 
 # Simulates the 4 polarization- and azimuth-resolved IRAS spectra
 simulatedSpectra = iras.SimulatePolarizationAzimuthSpectra_3Layer(simulationWavenumber,
                         nVacuum, nSubstrate, nAdsorbate,
                         filmThickness, angle)
 simulatedSpectra = simulatedSpectra.real
 
-# Plots the k parameters IRAS spectra
-plt.figure(0); plt.clf()
-plt.xlabel("$\mathregular{Wavenumber\ (cm^{-1})}$")
-plt.ylabel("$\mathregular{\Delta R / R}$")
-plt.plot(simulationWavenumber, dataK[0],label="k(x))")
-plt.plot(simulationWavenumber, dataK[1],label="k(y)")
-plt.plot(simulationWavenumber, dataK[2],label="k(z)")
-plt.xlim(1900, 3000)
-plt.legend()
-plt.tight_layout()
-plt.ion()
-plt.show()
-plt.savefig("Figure0.png", dpi=300, format='png')
-
 # Plots the 4 polarization- and azimuth-resolved IRAS spectra
-plt.figure(1); plt.clf()
+plt.figure(0); plt.clf()
 plt.xlabel("$\mathregular{Wavenumber\ (cm^{-1})}$")
 plt.ylabel("$\mathregular{\Delta R / R}$")
 plt.plot(simulatedSpectra[0], simulatedSpectra[1],label="s(y)")
 plt.plot(simulatedSpectra[0], simulatedSpectra[2],label="p(xz)")
 plt.plot(simulatedSpectra[0], simulatedSpectra[3],label="s(x)")
 plt.plot(simulatedSpectra[0], simulatedSpectra[4],label="p(yz)")
 plt.xlim(1900, 3000)
```

### Comparing `simulateIRAS-0.1.0.post5/setup.py` & `simulateIRAS-0.1.0.post6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="simulateIRAS",
-    version = '0.1.0-5',
+    version = '0.1.0-6',
     description="A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements",
     py_modules = ["simulateIRAS"],
     package_dir = {'':'src'},
     
     author="coconnor24",
     author_email="coconnor@g.harvard.edu",
```

### Comparing `simulateIRAS-0.1.0.post5/src/simulateIRAS.egg-info/PKG-INFO` & `simulateIRAS-0.1.0.post6/src/simulateIRAS.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulateIRAS
-Version: 0.1.0.post5
+Version: 0.1.0.post6
 Summary: A python package for simulating Infrared Reflection Absorption Spectroscopy(IRAS) measurements
 Home-page: https://github.com/coconnor24/simulateIRAS
 Author: coconnor24
 Author-email: coconnor@g.harvard.edu
 License: GPLv3
 Keywords: IRAS,Surface Science,FTIR,doi:
 Classifier: Development Status :: 4 - Beta
@@ -53,16 +53,25 @@
 We recommend importing in python as iras. 
 <br><br>
 `import simulateIRAS as iras`
 <br>
 
 ## Examples
 ### Example 1: Simulating polarization- and azimuth-resolved IRAS spectra
+This example simulates the 4 polarization- and azimuth-resolved IRAS spectra with given k parameters k(x), k(y), k(z) for an isotropic, dielectric substrate. The python code, input files and output files are provided in "simulateIRAS/examples/simpleSimulation". The simulation requires the following inputs: 
+1) incident angle of light relative to the surface normal
+2) complex index of refraction of the subtrate layer which here is wavelength independent for an isotropic substrate modelling anatase TiO<sub>2</sub>(101) as $n = 2.3 + 0.0i$.
+3) k parameters of the adsorbate layer (imaginary part of the complex index of refraction) which here is for a water film.
+4) real index of refraction of the adsorbate layer in the infinite wavenumber simulation limit which here is taken as $Real(n) = 1.37$ for a water film.
+5) adsobate film thickness
+The Kramersâ€“Kronig relations aure use on the adsorbate k parameters (imaginary part of the complex index of refraction) to get the real part of the complex index of refraction for the adsorbate layer. The simulation then applies the three-layer (substrate-adsorbate-vacuum) model to simulate the 4 polarization- and azimuth-resolved IRAS spectra.
+<br>
+The input adsorbate k parameters and 4 polarization- and azimuth-resolved simulated IRAS spectra are plotted below:
 <p align="center">
-<img src='./examples/simpleSimulation/Solutions/Figure1.png' width='50%'>
+<img src='./examples/simpleSimulation/Solutions/Figure0.png' width='40%'><img src='./examples/simpleSimulation/Solutions/Figure1.png' width='40%'>
 </p>
 
 ### Example 2: Determining extinction coefficients from polarization- and azimuth-resolved IRAS spectra
 <p align="center">
 <img src='./examples/simpleSimulation/Solutions/Figure1.png' width='50%'>
 </p>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `simulateIRAS-0.1.0.post5/src/simulateIRAS.py` & `simulateIRAS-0.1.0.post6/src/simulateIRAS.py`

 * *Files identical despite different names*

