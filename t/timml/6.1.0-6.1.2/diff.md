# Comparing `tmp/timml-6.1.0.tar.gz` & `tmp/timml-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timml-6.1.0.tar", last modified: Mon Mar 20 14:10:53 2023, max compression
+gzip compressed data, was "timml-6.1.2.tar", last modified: Wed May  3 16:16:49 2023, max compression
```

## Comparing `timml-6.1.0.tar` & `timml-6.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:10:53.076647 timml-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-20 14:10:38.000000 timml-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-20 14:10:38.000000 timml-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-20 14:10:53.076647 timml-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-20 14:10:38.000000 timml-6.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 14:10:53.076647 timml-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-20 14:10:38.000000 timml-6.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:10:53.072647 timml-6.1.0/timml/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-20 14:10:38.000000 timml-6.1.0/timml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-03-20 14:10:38.000000 timml-6.1.0/timml/aquifer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-20 14:10:38.000000 timml-6.1.0/timml/aquifer_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:10:53.076647 timml-6.1.0/timml/besselaesnumba/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 14:10:38.000000 timml-6.1.0/timml/besselaesnumba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25134 2023-03-20 14:10:38.000000 timml-6.1.0/timml/besselaesnumba/besselaesnumba.py
--rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-03-20 14:10:38.000000 timml-6.1.0/timml/besselaesnumba/besselaesnumba_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-03-20 14:10:38.000000 timml-6.1.0/timml/circareasink.py
--rw-r--r--   0 runner    (1001) docker     (123)    25025 2023-03-20 14:10:38.000000 timml-6.1.0/timml/circinhom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-03-20 14:10:38.000000 timml-6.1.0/timml/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-20 14:10:38.000000 timml-6.1.0/timml/controlpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-03-20 14:10:38.000000 timml-6.1.0/timml/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-03-20 14:10:38.000000 timml-6.1.0/timml/equation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-03-20 14:10:38.000000 timml-6.1.0/timml/inhomogeneity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-03-20 14:10:38.000000 timml-6.1.0/timml/inhomogeneity1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-03-20 14:10:38.000000 timml-6.1.0/timml/intlinesink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-03-20 14:10:38.000000 timml-6.1.0/timml/linedoublet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-20 14:10:38.000000 timml-6.1.0/timml/linedoublet1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    48454 2023-03-20 14:10:38.000000 timml-6.1.0/timml/linesink.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-03-20 14:10:38.000000 timml-6.1.0/timml/linesink1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-03-20 14:10:38.000000 timml-6.1.0/timml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:10:53.076647 timml-6.1.0/timml/src/
--rw-r--r--   0 runner    (1001) docker     (123)    34734 2023-03-20 14:10:38.000000 timml-6.1.0/timml/src/besselaesnew.f95
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-03-20 14:10:38.000000 timml-6.1.0/timml/stripareasink.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-03-20 14:10:38.000000 timml-6.1.0/timml/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-20 14:10:38.000000 timml-6.1.0/timml/uflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-03-20 14:10:38.000000 timml-6.1.0/timml/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-20 14:10:38.000000 timml-6.1.0/timml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-03-20 14:10:38.000000 timml-6.1.0/timml/well.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:10:53.072647 timml-6.1.0/timml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-20 14:10:52.000000 timml-6.1.0/timml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-20 14:10:53.000000 timml-6.1.0/timml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 14:10:52.000000 timml-6.1.0/timml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-20 14:10:52.000000 timml-6.1.0/timml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-20 14:10:52.000000 timml-6.1.0/timml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:16:49.640273 timml-6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 16:16:36.000000 timml-6.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 16:16:36.000000 timml-6.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-03 16:16:49.640273 timml-6.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-03 16:16:36.000000 timml-6.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:16:49.640273 timml-6.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-03 16:16:36.000000 timml-6.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:16:49.640273 timml-6.1.2/timml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-03 16:16:36.000000 timml-6.1.2/timml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-03 16:16:36.000000 timml-6.1.2/timml/aquifer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-03 16:16:36.000000 timml-6.1.2/timml/aquifer_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:16:49.640273 timml-6.1.2/timml/besselaesnumba/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:16:36.000000 timml-6.1.2/timml/besselaesnumba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24960 2023-05-03 16:16:36.000000 timml-6.1.2/timml/besselaesnumba/besselaesnumba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-05-03 16:16:36.000000 timml-6.1.2/timml/besselaesnumba/besselaesnumba_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-03 16:16:36.000000 timml-6.1.2/timml/circareasink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25025 2023-05-03 16:16:36.000000 timml-6.1.2/timml/circinhom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-03 16:16:36.000000 timml-6.1.2/timml/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-03 16:16:36.000000 timml-6.1.2/timml/controlpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-03 16:16:36.000000 timml-6.1.2/timml/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-05-03 16:16:36.000000 timml-6.1.2/timml/equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-05-03 16:16:36.000000 timml-6.1.2/timml/inhomogeneity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-03 16:16:36.000000 timml-6.1.2/timml/inhomogeneity1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-05-03 16:16:36.000000 timml-6.1.2/timml/intlinesink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-05-03 16:16:36.000000 timml-6.1.2/timml/linedoublet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-03 16:16:36.000000 timml-6.1.2/timml/linedoublet1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48454 2023-05-03 16:16:36.000000 timml-6.1.2/timml/linesink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-05-03 16:16:36.000000 timml-6.1.2/timml/linesink1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-05-03 16:16:36.000000 timml-6.1.2/timml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:16:49.640273 timml-6.1.2/timml/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    34734 2023-05-03 16:16:36.000000 timml-6.1.2/timml/src/besselaesnew.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-03 16:16:36.000000 timml-6.1.2/timml/stripareasink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-05-03 16:16:36.000000 timml-6.1.2/timml/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-03 16:16:36.000000 timml-6.1.2/timml/uflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-05-03 16:16:36.000000 timml-6.1.2/timml/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 16:16:36.000000 timml-6.1.2/timml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-05-03 16:16:36.000000 timml-6.1.2/timml/well.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:16:49.640273 timml-6.1.2/timml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-03 16:16:49.000000 timml-6.1.2/timml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 16:16:49.000000 timml-6.1.2/timml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:16:49.000000 timml-6.1.2/timml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 16:16:49.000000 timml-6.1.2/timml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 16:16:49.000000 timml-6.1.2/timml.egg-info/top_level.txt
```

### Comparing `timml-6.1.0/LICENSE` & `timml-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/PKG-INFO` & `timml-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timml
-Version: 6.1.0
+Version: 6.1.2
 Summary: Steady multi-layer AEM Model
 Home-page: https://github.com/mbakker7/timml
 Author: Mark Bakker
 Author-email: markbak@gmail.com
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >3.5
```

### Comparing `timml-6.1.0/README.md` & `timml-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/setup.py` & `timml-6.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/__init__.py` & `timml-6.1.2/timml/__init__.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/aquifer.py` & `timml-6.1.2/timml/aquifer.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/aquifer_parameters.py` & `timml-6.1.2/timml/aquifer_parameters.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/besselaesnumba/besselaesnumba.py` & `timml-6.1.2/timml/besselaesnumba/besselaesnumba.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 BC1[7] = -0.159531523882074e-12
 AC1[8] = 0.573031034976631e-15
 BC1[8] = -0.340195779923156e-14
 
 
 @numba.njit(nogil=True, cache=True)
 def prepare_z(x, y, z1, z2):
-    zin = np.complex(x, y)
+    zin = complex(x, y)
     z1in = z1
     z2in = z2
     Lin = abs(z2in - z1in)
     z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in)
     zplus1 = z + 1.0
     zmin1 = z - 1.0
     # If at cornerpoint, move slightly
@@ -127,15 +127,15 @@
     #    istart = 1
     # else:
     #    istart = 0
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
     # Laplace linesink
     if ilap == 1:
         power = order + 1
-        pcor = np.complex(0.0, 0.0)
+        pcor = complex(0.0, 0.0)
         for n in range(1, int((power + 1) / 2) + 1):
             pcor = pcor + z ** (power - 2 * n + 1) / (2 * n - 1)
         pcor = 2.0 * pcor
         comega = (
             z ** power * np.log((zmin1) / (zplus1))
             + pcor
             - np.log(zmin1)
@@ -189,15 +189,15 @@
     lstype = 1
 
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
 
     pcor = 0.0
     # Laplace linesink
     if ilap == 1:
-        pcor = np.complex(0.0, 0.0)
+        pcor = complex(0.0, 0.0)
         for n in range(1, int((order + 1) / 2) + 1):
             pcor = pcor + float(order - 2 * n + 2) * z ** (order + 1 - 2 * n) / float(
                 2 * n - 1
             )
 
         pcor = 2.0 * pcor
 
@@ -214,15 +214,15 @@
 
         wdis = wdis * Lin / 2.0 / (z2in - z1in) / np.pi * cdum
 
         rv[0, 0] = np.real(wdis)
         rv[1, 0] = -np.imag(wdis)
 
     for i in range(ilap, naq):
-        wdis = np.complex(0.0, 0.0)
+        wdis = complex(0.0, 0.0)
 
         # Check whether entire linesink is outside radius of convergence
         # Outside if |z-zc|>L/2+7lab, and thus |Z|>1+7lab*2/L, or |zeta|>1/biglab+7 (zeta is called z here)
         biglab = 2.0 * labda[i] / Lin
         z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
 
         if abs(z) < (Rconv + 1.0 / biglab):
@@ -273,42 +273,42 @@
     # lstype=2 means line-doublet
     lstype = 2
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
 
     # Laplace line-doublet
     if ilap == 1:
         comega = z ** order * np.log(zmin1 / zplus1)
-        qm = np.complex(0.0, 0.0)
+        qm = complex(0.0, 0.0)
         for n in range(1, int((order + 1) / 2) + 1):
             qm = qm + z ** (order - 2.0 * float(n) + 1.0) / (2.0 * float(n) - 1.0)
 
-        comega = 1.0 / (2.0 * np.pi * np.complex(0.0, 1.0)) * (comega + 2.0 * qm)
+        comega = 1.0 / (2.0 * np.pi * complex(0.0, 1.0)) * (comega + 2.0 * qm)
         rv[0] = np.real(comega)
 
     # N-1 leakage factors
     for i in range(ilap, naq):
         pot = 0.0
         # Check whether entire linedoublet is outside radius of convergence
         # Outside if |z-zc|>L/2+7lab, and thus |Z|>1+7lab*2/L, or |zeta|>1/biglab+7 (zeta is called z here)
         biglab = 2.0 * labda[i] / Lin
         z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
 
         if abs(z) < (Rconv + 1.0 / biglab):
             m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda[i], Rconv)
-            comega = np.complex(0.0, 0.0)
+            comega = complex(0.0, 0.0)
             if m1 > 0:  # Otherwise outside radius of convergence
                 z1new = z1in + float(m1 - 1) / float(NLS) * (z2in - z1in)
                 z2new = z1in + float(m2) / float(NLS) * (z2in - z1in)
                 del0 = float(1 - m1 - m2 + NLS) / float(1 - m1 + m2)
                 ra = float(NLS) / float(1 + m2 - m1)
                 comega = IntegralLapLineDipole(zin, z1new, z2new, del0, ra, order)
 
             pot = IntegralF(zin, z1in, z2in, Lin, labda[i], order, Rconv, lstype)
             rv[i] = (
-                np.real(comega / np.complex(0.0, 1.0)) + np.imag(z) / biglab * pot
+                np.real(comega / complex(0.0, 1.0)) + np.imag(z) / biglab * pot
             )  # Note that z is really zeta in analysis
         else:
             rv[i] = 0.0
 
     return rv
 
 
@@ -339,58 +339,58 @@
 
     # lstype=2 means line-doublet
     lstype = 2
 
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
 
     # Laplace line-doublet
-    qm = np.complex(0.0, 0.0)
+    qm = complex(0.0, 0.0)
     if ilap == 1:
         if order == 0:
             wdis = -(1.0 / zmin1 - 1.0 / zplus1) / (
-                np.pi * np.complex(0.0, 1.0) * (z2in - z1in)
+                np.pi * complex(0.0, 1.0) * (z2in - z1in)
             )
         else:
             wdis = float(order) * z ** (order - 1) * np.log(zmin1 / zplus1)
             wdis = wdis + z ** order * (1.0 / zmin1 - 1.0 / zplus1)
-            qm = np.complex(0.0, 0.0)
+            qm = complex(0.0, 0.0)
             if order > 1:  # To avoid a possible problem of 0 * 0^(-1)
                 for n in range(1, int(order / 2) + 1):
                     qm = qm + float(order - 2 * n + 1) * z ** (order - 2 * n) / float(
                         2 * n - 1
                     )
 
-            wdis = -(wdis + 2.0 * qm) / (np.pi * np.complex(0.0, 1.0) * (z2in - z1in))
+            wdis = -(wdis + 2.0 * qm) / (np.pi * complex(0.0, 1.0) * (z2in - z1in))
 
         rv[0, 0] = np.real(wdis)
         rv[1, 0] = -np.imag(wdis)
 
     # N-1 or N leakage factors
     for i in range(ilap, naq):
-        wdis = np.complex(0.0, 0.0)
+        wdis = complex(0.0, 0.0)
 
         # Check whether entire line-doublet is outside radius of convergence
         # Outside if |z-zc|>L/2+7lab, and thus |Z|>1+7lab*2/L, or |zeta|>1/biglab+7 (zeta is called z here)
         biglab = 2.0 * labda[i] / Lin
         z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
 
         if abs(z) < (Rconv + 1.0 / biglab):
             m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda[i], Rconv)
-            wdis1 = np.complex(0.0, 0.0)
+            wdis1 = complex(0.0, 0.0)
             if m1 > 0:
                 z1new = z1in + float(m1 - 1) / float(NLS) * (z2in - z1in)
                 z2new = z1in + float(m2) / float(NLS) * (z2in - z1in)
                 del0 = float(1 - m1 - m2 + NLS) / float(1 - m1 + m2)
                 ra = float(NLS) / float(1 + m2 - m1)
                 wdis1 = IntegralLapLineDipoleDis(zin, z1new, z2new, del0, ra, order)
-                wdis1 = -2.0 * wdis1 / (np.complex(0.0, 1.0) * (z2new - z1new))
+                wdis1 = -2.0 * wdis1 / (complex(0.0, 1.0) * (z2new - z1new))
 
             pot = IntegralF(zin, z1in, z2in, Lin, labda[i], order, Rconv, lstype)
             wdis2 = IntegralG(zin, z1in, z2in, Lin, labda[i], order, Rconv, lstype)
-            wdis3 = pot / (2.0 * np.complex(0.0, 1.0)) + wdis2 * np.imag(z)
+            wdis3 = pot / (2.0 * complex(0.0, 1.0)) + wdis2 * np.imag(z)
 
             wdis = wdis1 - 4.0 * wdis3 / (biglab ** 2 * (z2in - z1in))
         rv[0, i] = np.real(wdis)
         rv[1, i] = -1.0 * np.imag(wdis)
     return rv
 
 
@@ -403,21 +403,21 @@
         qxqy[n, 0 : naq + 1] = rv[0, 0:naq]
         qxqy[n + order + 1, 0 : naq + 1] = rv[1, 0 : naq + 1]
     return qxqy
 
 
 @numba.njit(nogil=True, cache=True)
 def IntegralF(zin, z1in, z2in, Lin, labda, order, Rconv, lstype):
-    czmzbarp = np.full(NTERMS + 1, np.complex(0.0, 0.0))
-    cgamma = np.full((NTERMS + 1, NTERMS + 1), np.complex(0.0, 0.0))
-    calphat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cbetat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cc = np.full(order + 2, np.complex(0.0, 0.0))
-    calpha = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
-    cbeta = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
+    czmzbarp = np.full(NTERMS + 1, complex(0.0, 0.0))
+    cgamma = np.full((NTERMS + 1, NTERMS + 1), complex(0.0, 0.0))
+    calphat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cbetat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cc = np.full(order + 2, complex(0.0, 0.0))
+    calpha = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
+    cbeta = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
 
     m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda, Rconv)
     if m1 == 0:
         # pot = 0.0
         return 0.0
 
     # Compute zeta (called z here). This is the regular value of the entire element
@@ -433,40 +433,40 @@
 
     for n in range(0, NTERMS + 1):
         for m in range(0, n + 1):
             cgamma[n, m] = RBINOM[n, m] * czmzbarp[n - m]
 
     # Eq. 23 These coefficients should be modified for a higher order linesink
     for n in range(0, 2 * NTERMS + 1):
-        calphat[n] = np.complex(0.0, 0.0)
-        cbetat[n] = np.complex(0.0, 0.0)
+        calphat[n] = complex(0.0, 0.0)
+        cbetat[n] = complex(0.0, 0.0)
         for m in range(max(0, n - NTERMS), int(n / 2) + 1):
             if lstype == 1:
                 calphat[n] = calphat[n] + AC[n - m] * cgamma[n - m, m]
                 cbetat[n] = cbetat[n] + BC[n - m] * cgamma[n - m, m]
             else:
                 calphat[n] = calphat[n] + AC1[n - m] * cgamma[n - m, m]
                 cbetat[n] = cbetat[n] + BC1[n - m] * cgamma[n - m, m]
 
     # Compute coefficients of delta^p
     for m in range(0, order + 1):
         cc[m] = RBINOM[order, m] * z ** (order - m) * biglab ** order
     if order > 0:
         for n in range(0, 2 * NTERMS + order + 1):
-            calpha[n] = np.complex(0.0, 0.0)
-            cbeta[n] = np.complex(0.0, 0.0)
+            calpha[n] = complex(0.0, 0.0)
+            cbeta[n] = complex(0.0, 0.0)
             for m in range(max(0, n - 2 * NTERMS), min(n, order) + 1):
                 calpha[n] = calpha[n] + cc[m] * calphat[n - m]
                 cbeta[n] = cbeta[n] + cc[m] * cbetat[n - m]
     else:
         calpha = calphat
         cbeta = cbetat
 
     # Evaluation of integral, Eq. 25
-    cInt = np.complex(0.0, 0.0)
+    cInt = complex(0.0, 0.0)
     del1 = -1.0 + 2.0 * (float(m1) - 1.0) / float(NLS)
     del2 = -1.0 + 2.0 * float(m2) / float(NLS)
     cd1minz = del1 / biglab - z
     cd2minz = del2 / biglab - z
     if abs(cd1minz) < 1.0e-8 / labda:
         cd1minz = cd1minz + 1.0e-8
     if abs(cd2minz) < 1.0e-8 / labda:
@@ -482,30 +482,30 @@
         ) * (cd1minz) ** (n + 1) / float(n + 1)
     pot = np.real(cInt) * biglab / (2.0 * np.pi)
     return pot
 
 
 @numba.njit(nogil=True, cache=True)
 def IntegralG(zin, z1in, z2in, Lin, labda, order, Rconv, lstype):
-    czmzbarp = np.full(NTERMS + 1, np.complex(0.0, 0.0))
-    cgamma = np.full((NTERMS + 1, NTERMS + 1), np.complex(0.0, 0.0))
-    cahat = np.full(2 * (NTERMS - 1) + 1, np.complex(0.0, 0.0))
-    cbhat = np.full(2 * (NTERMS - 1) + 1, np.complex(0.0, 0.0))
-    calphat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cbetat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cc = np.full(order + 2, np.complex(0.0, 0.0))
-    calpha = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
-    cbeta = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
+    czmzbarp = np.full(NTERMS + 1, complex(0.0, 0.0))
+    cgamma = np.full((NTERMS + 1, NTERMS + 1), complex(0.0, 0.0))
+    cahat = np.full(2 * (NTERMS - 1) + 1, complex(0.0, 0.0))
+    cbhat = np.full(2 * (NTERMS - 1) + 1, complex(0.0, 0.0))
+    calphat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cbetat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cc = np.full(order + 2, complex(0.0, 0.0))
+    calpha = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
+    cbeta = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
 
     biglabin = 2.0 * labda / Lin
 
     m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda, Rconv)
     if m1 == 0:
-        # wdis = np.complex(0.0, 0.0)
-        return np.complex(0.0, 0.0)
+        # wdis = complex(0.0, 0.0)
+        return complex(0.0, 0.0)
 
     # Compute zeta (called z here). This is the regular value of the entire element
     L = abs(z2in - z1in)
     biglab = 2.0 * labda / L
     z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
     zbar = np.conj(z)
 
@@ -520,15 +520,15 @@
 
     # Integral g1
     # Implemented with different z, rather than Delta1 and Delta2
     z1 = z1in + float(m1 - 1) / float(NLS) * (z2in - z1in)
     z2 = z1in + float(m2) / float(NLS) * (z2in - z1in)
     del0 = float(1 - m1 - m2 + NLS) / float(1 - m1 + m2)
     ra = float(NLS) / float(1 + m2 - m1)
-    # comega = np.complex(0.0, 0.0)
+    # comega = complex(0.0, 0.0)
     comega = IntegralLapLineDipole(zin, z1, z2, del0, ra, order)
 
     if lstype == 1:
         g1 = -AC[0] * biglabin * comega
         # Integral g2
         # Compute hat coefficients
         for n in range(0, NTERMS):
@@ -540,36 +540,36 @@
         # Compute hat coefficients
         for n in range(0, NTERMS):
             cahat[n] = float(n + 1) * AC1[n + 1]
             cbhat[n] = AC1[n + 1] + float(n + 1) * BC1[n + 1]
 
     # Eq. 23
     for n in range(0, 2 * NTERMS):
-        calphat[n] = np.complex(0.0, 0.0)
-        cbetat[n] = np.complex(0.0, 0.0)
+        calphat[n] = complex(0.0, 0.0)
+        cbetat[n] = complex(0.0, 0.0)
         for m in range(max(0, n - NTERMS + 1), int((n + 1) / 2) + 1):
             calphat[n] = calphat[n] + cahat[n - m] * cgamma[n - m + 1, m]
             cbetat[n] = cbetat[n] + cbhat[n - m] * cgamma[n - m + 1, m]
 
     # Compute coefficients of delta^p
     for m in range(0, order + 1):
         cc[m] = RBINOM[order, m] * z ** (order - m) * biglab ** order
     if order > 0:
         for n in range(0, 2 * NTERMS + order):
-            calpha[n] = np.complex(0.0, 0.0)
-            cbeta[n] = np.complex(0.0, 0.0)
+            calpha[n] = complex(0.0, 0.0)
+            cbeta[n] = complex(0.0, 0.0)
             for m in range(max(0, n - 2 * NTERMS + 1), min(n, order) + 1):
                 calpha[n] = calpha[n] + cc[m] * calphat[n - m]
                 cbeta[n] = cbeta[n] + cc[m] * cbetat[n - m]
     else:
         calpha = calphat
         cbeta = cbetat
 
     # Computation of integral
-    g2 = np.complex(0.0, 0.0)
+    g2 = complex(0.0, 0.0)
     del1 = -1.0 + 2.0 * (float(m1) - 1.0) / float(NLS)
     del2 = -1.0 + 2.0 * float(m2) / float(NLS)
     cd1minz = del1 / biglab - z
     cd2minz = del2 / biglab - z
     if abs(cd1minz) < 1.0e-8 / labda:
         cd1minz = cd1minz + 1.0e-8
     if abs(cd2minz) < 1.0e-8 / labda:
@@ -583,36 +583,36 @@
         g2 = g2 + (calpha[n] * cln1 - calpha[n] / (n + 1) + cbeta[n]) * (cd1minz) ** (
             n + 1
         ) / float(n + 1)
     g2 = biglabin * g2 / (2 * np.pi)
 
     # Integral g3
     # Eq. 23
-    calphat[0] = np.complex(0.0, 0.0)
+    calphat[0] = complex(0.0, 0.0)
     for n in range(1, 2 * NTERMS):  # Loop start at 1, because of bug in Digital Fortran
-        calphat[n] = np.complex(0.0, 0.0)
+        calphat[n] = complex(0.0, 0.0)
         for m in range(max(0, n - NTERMS), int((n - 1) / 2) + 1):
             calphat[n] = calphat[n] + cahat[n - m - 1] * cgamma[n - m - 1, m] * (
                 -1.0
             ) ** (n - 1 - 2 * m)
 
     # Compute coefficients of delta^p
     for m in range(0, order + 1):
         cc[m] = RBINOM[order, m] * zbar ** (order - m) * biglab ** order
 
     if order > 0:
         for n in range(0, 2 * NTERMS + order):
-            calpha[n] = np.complex(0.0, 0.0)
+            calpha[n] = complex(0.0, 0.0)
             for m in range(max(0, n - 2 * NTERMS + 1), min(n, order) + 1):
                 calpha[n] = calpha[n] + cc[m] * calphat[n - m]
     else:
         calpha = calphat
 
     # Computation of integral
-    g3 = np.complex(0.0, 0.0)
+    g3 = complex(0.0, 0.0)
     # cd1minz = del1 / biglab - zbar  cd2minz = del2 / biglab - zbar
     # if ( abs(cd1minz) < 1.0e-8) cd1minz = cd1minz + 1.0e-8
     # if ( abs(cd2minz) < 1.0e-8) cd2minz = cd2minz + 1.0e-8
     # By definition log is conjugate of previous log this avoids problems with signs along the line (and saves logs).
     cd1minz = np.conj(cd1minz)
     cd2minz = np.conj(cd2minz)
     cln1 = np.conj(cln1)
@@ -627,61 +627,61 @@
     g3 = biglabin * g3 / (2.0 * np.pi)
     wdis = g1 + g2 + g3
     return wdis
 
 
 @numba.njit(nogil=True, cache=True)
 def IntegralLapLineDipole(zin, z1, z2, del0, ra, order):
-    cg = np.full(order + 2, np.complex(0.0, 0.0))
+    cg = np.full(order + 2, complex(0.0, 0.0))
     z = (2.0 * zin - (z1 + z2)) / (z2 - z1)
     zplus1 = z + 1.0
     zmin1 = z - 1.0
 
     # We don't always have to do this, so maybe put in condition?
     # Determine coefficients of powers of Delta
     for m in range(0, order + 1):
         cg[m] = RBINOM[order, m] * (-del0) ** (order - m) / ra ** order
 
-    zterm = np.complex(0.0, 0.0)
+    zterm = complex(0.0, 0.0)
     for n in range(0, order + 1):
         zterm = zterm + cg[n] * z ** n
 
-    qmtot = np.complex(0.0, 0.0)
+    qmtot = complex(0.0, 0.0)
     for m in range(1, order + 1):
-        qm = np.complex(0.0, 0.0)
+        qm = complex(0.0, 0.0)
         for n in range(1, int((m + 1) / 2) + 1):
             qm = qm + z ** (m - 2 * n + 1) / float(2 * n - 1)
         qmtot = qmtot + 2.0 * cg[m] * qm
 
     comega = (zterm * np.log(zmin1 / zplus1) + qmtot) / (2.0 * np.pi)
     return comega
 
 
 @numba.njit(nogil=True, cache=True)
 def IntegralLapLineDipoleDis(zin, z1, z2, del0, ra, order):
-    cg = np.full(order + 2, np.complex(0.0, 0.0))
+    cg = np.full(order + 2, complex(0.0, 0.0))
 
     z = (2.0 * zin - (z1 + z2)) / (z2 - z1)
     zplus1 = z + 1.0
     zmin1 = z - 1.0
 
     # Determine coefficients of powers of Delta for [ (Delta-Delta_0)/a ] ^ p
     for m in range(0, order + 1):
         cg[m] = RBINOM[order, m] * (-del0) ** (order - m) / ra ** order
 
-    zterm1 = np.complex(0.0, 0.0)
-    zterm2 = np.complex(0.0, 0.0)
+    zterm1 = complex(0.0, 0.0)
+    zterm2 = complex(0.0, 0.0)
     for n in range(1, order + 1):
         zterm1 = zterm1 + cg[n] * float(n) * z ** (n - 1)
     for n in range(0, order + 1):
         zterm2 = zterm2 + cg[n] * z ** n
 
-    qmtot = np.complex(0.0, 0.0)
+    qmtot = complex(0.0, 0.0)
     for m in range(2, order + 1):
-        qm = np.complex(0.0, 0.0)
+        qm = complex(0.0, 0.0)
         for n in range(1, int(m / 2) + 1):
             qm = qm + float(m - 2 * n + 1) * z ** (m - 2 * n) / float(2 * n - 1)
         qmtot = qmtot + 2.0 * cg[m] * qm
 
     wdis = (
         zterm1 * np.log(zmin1 / zplus1) + zterm2 * (1.0 / zmin1 - 1.0 / zplus1) + qmtot
     ) / (2.0 * np.pi)
```

### Comparing `timml-6.1.0/timml/besselaesnumba/besselaesnumba_old.py` & `timml-6.1.2/timml/besselaesnumba/besselaesnumba_old.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 BC1[7] = -0.159531523882074e-12
 AC1[8] = 0.573031034976631e-15
 BC1[8] = -0.340195779923156e-14
 
 
 @numba.njit
 def prepare_z(x, y, z1, z2):
-    zin = np.complex(x, y)
+    zin = complex(x, y)
     z1in = z1
     z2in = z2
     Lin = abs(z2in - z1in)
     z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in)
     zplus1 = z + 1.0
     zmin1 = z - 1.0
     # If at cornerpoint, move slightly
@@ -116,15 +116,15 @@
     #    istart = 1
     # else:
     #    istart = 0
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
     # Laplace linesink
     if ilap == 1:
         power = order + 1
-        pcor = np.complex(0.0, 0.0)
+        pcor = complex(0.0, 0.0)
         for n in range(1, int((power + 1) / 2) + 1):
             pcor = pcor + z ** (power - 2 * n + 1) / (2 * n - 1)
         pcor = 2.0 * pcor
         comega = (
             z ** power * np.log((zmin1) / (zplus1))
             + pcor
             - np.log(zmin1)
@@ -177,15 +177,15 @@
     lstype = 1
 
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
 
     pcor = 0.0
     # Laplace linesink
     if ilap == 1:
-        pcor = np.complex(0.0, 0.0)
+        pcor = complex(0.0, 0.0)
         for n in range(1, int((order + 1) / 2) + 1):
             pcor = pcor + float(order - 2 * n + 2) * z ** (order + 1 - 2 * n) / float(
                 2 * n - 1
             )
 
         pcor = 2.0 * pcor
 
@@ -202,15 +202,15 @@
 
         wdis = wdis * Lin / 2.0 / (z2in - z1in) / np.pi * cdum
 
         rv[0, 0] = np.real(wdis)
         rv[1, 0] = -np.imag(wdis)
 
     for i in range(ilap, naq):
-        wdis = np.complex(0.0, 0.0)
+        wdis = complex(0.0, 0.0)
 
         # Check whether entire linesink is outside radius of convergence
         # Outside if |z-zc|>L/2+7lab, and thus |Z|>1+7lab*2/L, or |zeta|>1/biglab+7 (zeta is called z here)
         biglab = 2.0 * labda[i] / Lin
         z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
 
         if abs(z) < (Rconv + 1.0 / biglab):
@@ -261,42 +261,42 @@
     # lstype=2 means line-doublet
     lstype = 2
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
 
     # Laplace line-doublet
     if ilap == 1:
         comega = z ** order * np.log(zmin1 / zplus1)
-        qm = np.complex(0.0, 0.0)
+        qm = complex(0.0, 0.0)
         for n in range(1, int((order + 1) / 2) + 1):
             qm = qm + z ** (order - 2.0 * float(n) + 1.0) / (2.0 * float(n) - 1.0)
 
-        comega = 1.0 / (2.0 * np.pi * np.complex(0.0, 1.0)) * (comega + 2.0 * qm)
+        comega = 1.0 / (2.0 * np.pi * complex(0.0, 1.0)) * (comega + 2.0 * qm)
         rv[0] = np.real(comega)
 
     # N-1 leakage factors
     for i in range(ilap, naq):
         pot = 0.0
         # Check whether entire linedoublet is outside radius of convergence
         # Outside if |z-zc|>L/2+7lab, and thus |Z|>1+7lab*2/L, or |zeta|>1/biglab+7 (zeta is called z here)
         biglab = 2.0 * labda[i] / Lin
         z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
 
         if abs(z) < (Rconv + 1.0 / biglab):
             m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda[i], Rconv)
-            comega = np.complex(0.0, 0.0)
+            comega = complex(0.0, 0.0)
             if m1 > 0:  # Otherwise outside radius of convergence
                 z1new = z1in + float(m1 - 1) / float(NLS) * (z2in - z1in)
                 z2new = z1in + float(m2) / float(NLS) * (z2in - z1in)
                 del0 = float(1 - m1 - m2 + NLS) / float(1 - m1 + m2)
                 ra = float(NLS) / float(1 + m2 - m1)
                 comega = IntegralLapLineDipole(zin, z1new, z2new, del0, ra, order)
 
             pot = IntegralF(zin, z1in, z2in, Lin, labda[i], order, Rconv, lstype)
             rv[i] = (
-                np.real(comega / np.complex(0.0, 1.0)) + np.imag(z) / biglab * pot
+                np.real(comega / complex(0.0, 1.0)) + np.imag(z) / biglab * pot
             )  # Note that z is really zeta in analysis
         else:
             rv[i] = 0.0
 
     return rv
 
 
@@ -327,58 +327,58 @@
 
     # lstype=2 means line-doublet
     lstype = 2
 
     zin, z1in, z2in, Lin, z, zplus1, zmin1 = prepare_z(x, y, z1, z2)
 
     # Laplace line-doublet
-    qm = np.complex(0.0, 0.0)
+    qm = complex(0.0, 0.0)
     if ilap == 1:
         if order == 0:
             wdis = -(1.0 / zmin1 - 1.0 / zplus1) / (
-                np.pi * np.complex(0.0, 1.0) * (z2in - z1in)
+                np.pi * complex(0.0, 1.0) * (z2in - z1in)
             )
         else:
             wdis = float(order) * z ** (order - 1) * np.log(zmin1 / zplus1)
             wdis = wdis + z ** order * (1.0 / zmin1 - 1.0 / zplus1)
-            qm = np.complex(0.0, 0.0)
+            qm = complex(0.0, 0.0)
             if order > 1:  # To avoid a possible problem of 0 * 0^(-1)
                 for n in range(1, int(order / 2) + 1):
                     qm = qm + float(order - 2 * n + 1) * z ** (order - 2 * n) / float(
                         2 * n - 1
                     )
 
-            wdis = -(wdis + 2.0 * qm) / (np.pi * np.complex(0.0, 1.0) * (z2in - z1in))
+            wdis = -(wdis + 2.0 * qm) / (np.pi * complex(0.0, 1.0) * (z2in - z1in))
 
         rv[0, 0] = np.real(wdis)
         rv[1, 0] = -np.imag(wdis)
 
     # N-1 or N leakage factors
     for i in range(ilap, naq):
-        wdis = np.complex(0.0, 0.0)
+        wdis = complex(0.0, 0.0)
 
         # Check whether entire line-doublet is outside radius of convergence
         # Outside if |z-zc|>L/2+7lab, and thus |Z|>1+7lab*2/L, or |zeta|>1/biglab+7 (zeta is called z here)
         biglab = 2.0 * labda[i] / Lin
         z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
 
         if abs(z) < (Rconv + 1.0 / biglab):
             m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda[i], Rconv)
-            wdis1 = np.complex(0.0, 0.0)
+            wdis1 = complex(0.0, 0.0)
             if m1 > 0:
                 z1new = z1in + float(m1 - 1) / float(NLS) * (z2in - z1in)
                 z2new = z1in + float(m2) / float(NLS) * (z2in - z1in)
                 del0 = float(1 - m1 - m2 + NLS) / float(1 - m1 + m2)
                 ra = float(NLS) / float(1 + m2 - m1)
                 wdis1 = IntegralLapLineDipoleDis(zin, z1new, z2new, del0, ra, order)
-                wdis1 = -2.0 * wdis1 / (np.complex(0.0, 1.0) * (z2new - z1new))
+                wdis1 = -2.0 * wdis1 / (complex(0.0, 1.0) * (z2new - z1new))
 
             pot = IntegralF(zin, z1in, z2in, Lin, labda[i], order, Rconv, lstype)
             wdis2 = IntegralG(zin, z1in, z2in, Lin, labda[i], order, Rconv, lstype)
-            wdis3 = pot / (2.0 * np.complex(0.0, 1.0)) + wdis2 * np.imag(z)
+            wdis3 = pot / (2.0 * complex(0.0, 1.0)) + wdis2 * np.imag(z)
 
             wdis = wdis1 - 4.0 * wdis3 / (biglab ** 2 * (z2in - z1in))
         rv[0, i] = np.real(wdis)
         rv[1, i] = -1.0 * np.imag(wdis)
     return rv
 
 
@@ -391,21 +391,21 @@
         qxqy[n, 0 : naq + 1] = rv[0, 0:naq]
         qxqy[n + order + 1, 0 : naq + 1] = rv[1, 0 : naq + 1]
     return qxqy
 
 
 @numba.njit
 def IntegralF(zin, z1in, z2in, Lin, labda, order, Rconv, lstype):
-    czmzbarp = np.full(NTERMS + 1, np.complex(0.0, 0.0))
-    cgamma = np.full((NTERMS + 1, NTERMS + 1), np.complex(0.0, 0.0))
-    calphat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cbetat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cc = np.full(order + 2, np.complex(0.0, 0.0))
-    calpha = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
-    cbeta = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
+    czmzbarp = np.full(NTERMS + 1, complex(0.0, 0.0))
+    cgamma = np.full((NTERMS + 1, NTERMS + 1), complex(0.0, 0.0))
+    calphat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cbetat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cc = np.full(order + 2, complex(0.0, 0.0))
+    calpha = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
+    cbeta = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
 
     m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda, Rconv)
     if m1 == 0:
         # pot = 0.0
         return 0.0
 
     # Compute zeta (called z here). This is the regular value of the entire element
@@ -421,40 +421,40 @@
 
     for n in range(0, NTERMS + 1):
         for m in range(0, n + 1):
             cgamma[n, m] = RBINOM[n, m] * czmzbarp[n - m]
 
     # Eq. 23 These coefficients should be modified for a higher order linesink
     for n in range(0, 2 * NTERMS + 1):
-        calphat[n] = np.complex(0.0, 0.0)
-        cbetat[n] = np.complex(0.0, 0.0)
+        calphat[n] = complex(0.0, 0.0)
+        cbetat[n] = complex(0.0, 0.0)
         for m in range(max(0, n - NTERMS), int(n / 2) + 1):
             if lstype == 1:
                 calphat[n] = calphat[n] + AC[n - m] * cgamma[n - m, m]
                 cbetat[n] = cbetat[n] + BC[n - m] * cgamma[n - m, m]
             else:
                 calphat[n] = calphat[n] + AC1[n - m] * cgamma[n - m, m]
                 cbetat[n] = cbetat[n] + BC1[n - m] * cgamma[n - m, m]
 
     # Compute coefficients of delta^p
     for m in range(0, order + 1):
         cc[m] = RBINOM[order, m] * z ** (order - m) * biglab ** order
     if order > 0:
         for n in range(0, 2 * NTERMS + order + 1):
-            calpha[n] = np.complex(0.0, 0.0)
-            cbeta[n] = np.complex(0.0, 0.0)
+            calpha[n] = complex(0.0, 0.0)
+            cbeta[n] = complex(0.0, 0.0)
             for m in range(max(0, n - 2 * NTERMS), min(n, order) + 1):
                 calpha[n] = calpha[n] + cc[m] * calphat[n - m]
                 cbeta[n] = cbeta[n] + cc[m] * cbetat[n - m]
     else:
         calpha = calphat
         cbeta = cbetat
 
     # Evaluation of integral, Eq. 25
-    cInt = np.complex(0.0, 0.0)
+    cInt = complex(0.0, 0.0)
     del1 = -1.0 + 2.0 * (float(m1) - 1.0) / float(NLS)
     del2 = -1.0 + 2.0 * float(m2) / float(NLS)
     cd1minz = del1 / biglab - z
     cd2minz = del2 / biglab - z
     if abs(cd1minz) < 1.0e-8 / labda:
         cd1minz = cd1minz + 1.0e-8
     if abs(cd2minz) < 1.0e-8 / labda:
@@ -470,30 +470,30 @@
         ) * (cd1minz) ** (n + 1) / float(n + 1)
     pot = np.real(cInt) * biglab / (2.0 * np.pi)
     return pot
 
 
 @numba.njit
 def IntegralG(zin, z1in, z2in, Lin, labda, order, Rconv, lstype):
-    czmzbarp = np.full(NTERMS + 1, np.complex(0.0, 0.0))
-    cgamma = np.full((NTERMS + 1, NTERMS + 1), np.complex(0.0, 0.0))
-    cahat = np.full(2 * (NTERMS - 1) + 1, np.complex(0.0, 0.0))
-    cbhat = np.full(2 * (NTERMS - 1) + 1, np.complex(0.0, 0.0))
-    calphat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cbetat = np.full(2 * NTERMS + 1, np.complex(0.0, 0.0))
-    cc = np.full(order + 2, np.complex(0.0, 0.0))
-    calpha = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
-    cbeta = np.full(2 * NTERMS + order + 1, np.complex(0.0, 0.0))
+    czmzbarp = np.full(NTERMS + 1, complex(0.0, 0.0))
+    cgamma = np.full((NTERMS + 1, NTERMS + 1), complex(0.0, 0.0))
+    cahat = np.full(2 * (NTERMS - 1) + 1, complex(0.0, 0.0))
+    cbhat = np.full(2 * (NTERMS - 1) + 1, complex(0.0, 0.0))
+    calphat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cbetat = np.full(2 * NTERMS + 1, complex(0.0, 0.0))
+    cc = np.full(order + 2, complex(0.0, 0.0))
+    calpha = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
+    cbeta = np.full(2 * NTERMS + order + 1, complex(0.0, 0.0))
 
     biglabin = 2.0 * labda / Lin
 
     m1, m2, NLS = findm1m2(zin, z1in, z2in, Lin, labda, Rconv)
     if m1 == 0:
-        # wdis = np.complex(0.0, 0.0)
-        return np.complex(0.0, 0.0)
+        # wdis = complex(0.0, 0.0)
+        return complex(0.0, 0.0)
 
     # Compute zeta (called z here). This is the regular value of the entire element
     L = abs(z2in - z1in)
     biglab = 2.0 * labda / L
     z = (2.0 * zin - (z1in + z2in)) / (z2in - z1in) / biglab
     zbar = np.conj(z)
 
@@ -508,15 +508,15 @@
 
     # Integral g1
     # Implemented with different z, rather than Delta1 and Delta2
     z1 = z1in + float(m1 - 1) / float(NLS) * (z2in - z1in)
     z2 = z1in + float(m2) / float(NLS) * (z2in - z1in)
     del0 = float(1 - m1 - m2 + NLS) / float(1 - m1 + m2)
     ra = float(NLS) / float(1 + m2 - m1)
-    # comega = np.complex(0.0, 0.0)
+    # comega = complex(0.0, 0.0)
     comega = IntegralLapLineDipole(zin, z1, z2, del0, ra, order)
 
     if lstype == 1:
         g1 = -AC[0] * biglabin * comega
         # Integral g2
         # Compute hat coefficients
         for n in range(0, NTERMS):
@@ -528,36 +528,36 @@
         # Compute hat coefficients
         for n in range(0, NTERMS):
             cahat[n] = float(n + 1) * AC1[n + 1]
             cbhat[n] = AC1[n + 1] + float(n + 1) * BC1[n + 1]
 
     # Eq. 23
     for n in range(0, 2 * NTERMS):
-        calphat[n] = np.complex(0.0, 0.0)
-        cbetat[n] = np.complex(0.0, 0.0)
+        calphat[n] = complex(0.0, 0.0)
+        cbetat[n] = complex(0.0, 0.0)
         for m in range(max(0, n - NTERMS + 1), int((n + 1) / 2) + 1):
             calphat[n] = calphat[n] + cahat[n - m] * cgamma[n - m + 1, m]
             cbetat[n] = cbetat[n] + cbhat[n - m] * cgamma[n - m + 1, m]
 
     # Compute coefficients of delta^p
     for m in range(0, order + 1):
         cc[m] = RBINOM[order, m] * z ** (order - m) * biglab ** order
     if order > 0:
         for n in range(0, 2 * NTERMS + order):
-            calpha[n] = np.complex(0.0, 0.0)
-            cbeta[n] = np.complex(0.0, 0.0)
+            calpha[n] = complex(0.0, 0.0)
+            cbeta[n] = complex(0.0, 0.0)
             for m in range(max(0, n - 2 * NTERMS + 1), min(n, order) + 1):
                 calpha[n] = calpha[n] + cc[m] * calphat[n - m]
                 cbeta[n] = cbeta[n] + cc[m] * cbetat[n - m]
     else:
         calpha = calphat
         cbeta = cbetat
 
     # Computation of integral
-    g2 = np.complex(0.0, 0.0)
+    g2 = complex(0.0, 0.0)
     del1 = -1.0 + 2.0 * (float(m1) - 1.0) / float(NLS)
     del2 = -1.0 + 2.0 * float(m2) / float(NLS)
     cd1minz = del1 / biglab - z
     cd2minz = del2 / biglab - z
     if abs(cd1minz) < 1.0e-8 / labda:
         cd1minz = cd1minz + 1.0e-8
     if abs(cd2minz) < 1.0e-8 / labda:
@@ -571,36 +571,36 @@
         g2 = g2 + (calpha[n] * cln1 - calpha[n] / (n + 1) + cbeta[n]) * (cd1minz) ** (
             n + 1
         ) / float(n + 1)
     g2 = biglabin * g2 / (2 * np.pi)
 
     # Integral g3
     # Eq. 23
-    calphat[0] = np.complex(0.0, 0.0)
+    calphat[0] = complex(0.0, 0.0)
     for n in range(1, 2 * NTERMS):  # Loop start at 1, because of bug in Digital Fortran
-        calphat[n] = np.complex(0.0, 0.0)
+        calphat[n] = complex(0.0, 0.0)
         for m in range(max(0, n - NTERMS), int((n - 1) / 2) + 1):
             calphat[n] = calphat[n] + cahat[n - m - 1] * cgamma[n - m - 1, m] * (
                 -1.0
             ) ** (n - 1 - 2 * m)
 
     # Compute coefficients of delta^p
     for m in range(0, order + 1):
         cc[m] = RBINOM[order, m] * zbar ** (order - m) * biglab ** order
 
     if order > 0:
         for n in range(0, 2 * NTERMS + order):
-            calpha[n] = np.complex(0.0, 0.0)
+            calpha[n] = complex(0.0, 0.0)
             for m in range(max(0, n - 2 * NTERMS + 1), min(n, order) + 1):
                 calpha[n] = calpha[n] + cc[m] * calphat[n - m]
     else:
         calpha = calphat
 
     # Computation of integral
-    g3 = np.complex(0.0, 0.0)
+    g3 = complex(0.0, 0.0)
     # cd1minz = del1 / biglab - zbar  cd2minz = del2 / biglab - zbar
     # if ( abs(cd1minz) < 1.0e-8) cd1minz = cd1minz + 1.0e-8
     # if ( abs(cd2minz) < 1.0e-8) cd2minz = cd2minz + 1.0e-8
     # By definition log is conjugate of previous log this avoids problems with signs along the line (and saves logs).
     cd1minz = np.conj(cd1minz)
     cd2minz = np.conj(cd2minz)
     cln1 = np.conj(cln1)
@@ -615,61 +615,61 @@
     g3 = biglabin * g3 / (2.0 * np.pi)
     wdis = g1 + g2 + g3
     return wdis
 
 
 @numba.njit
 def IntegralLapLineDipole(zin, z1, z2, del0, ra, order):
-    cg = np.full(order + 2, np.complex(0.0, 0.0))
+    cg = np.full(order + 2, complex(0.0, 0.0))
     z = (2.0 * zin - (z1 + z2)) / (z2 - z1)
     zplus1 = z + 1.0
     zmin1 = z - 1.0
 
     # We don't always have to do this, so maybe put in condition?
     # Determine coefficients of powers of Delta
     for m in range(0, order + 1):
         cg[m] = RBINOM[order, m] * (-del0) ** (order - m) / ra ** order
 
-    zterm = np.complex(0.0, 0.0)
+    zterm = complex(0.0, 0.0)
     for n in range(0, order + 1):
         zterm = zterm + cg[n] * z ** n
 
-    qmtot = np.complex(0.0, 0.0)
+    qmtot = complex(0.0, 0.0)
     for m in range(1, order + 1):
-        qm = np.complex(0.0, 0.0)
+        qm = complex(0.0, 0.0)
         for n in range(1, int((m + 1) / 2) + 1):
             qm = qm + z ** (m - 2 * n + 1) / float(2 * n - 1)
         qmtot = qmtot + 2.0 * cg[m] * qm
 
     comega = (zterm * np.log(zmin1 / zplus1) + qmtot) / (2.0 * np.pi)
     return comega
 
 
 @numba.njit
 def IntegralLapLineDipoleDis(zin, z1, z2, del0, ra, order):
-    cg = np.full(order + 2, np.complex(0.0, 0.0))
+    cg = np.full(order + 2, complex(0.0, 0.0))
 
     z = (2.0 * zin - (z1 + z2)) / (z2 - z1)
     zplus1 = z + 1.0
     zmin1 = z - 1.0
 
     # Determine coefficients of powers of Delta for [ (Delta-Delta_0)/a ] ^ p
     for m in range(0, order + 1):
         cg[m] = RBINOM[order, m] * (-del0) ** (order - m) / ra ** order
 
-    zterm1 = np.complex(0.0, 0.0)
-    zterm2 = np.complex(0.0, 0.0)
+    zterm1 = complex(0.0, 0.0)
+    zterm2 = complex(0.0, 0.0)
     for n in range(1, order + 1):
         zterm1 = zterm1 + cg[n] * float(n) * z ** (n - 1)
     for n in range(0, order + 1):
         zterm2 = zterm2 + cg[n] * z ** n
 
-    qmtot = np.complex(0.0, 0.0)
+    qmtot = complex(0.0, 0.0)
     for m in range(2, order + 1):
-        qm = np.complex(0.0, 0.0)
+        qm = complex(0.0, 0.0)
         for n in range(1, int(m / 2) + 1):
             qm = qm + float(m - 2 * n + 1) * z ** (m - 2 * n) / float(2 * n - 1)
         qmtot = qmtot + 2.0 * cg[m] * qm
 
     wdis = (
         zterm1 * np.log(zmin1 / zplus1) + zterm2 * (1.0 / zmin1 - 1.0 / zplus1) + qmtot
     ) / (2.0 * np.pi)
```

### Comparing `timml-6.1.0/timml/circareasink.py` & `timml-6.1.2/timml/circareasink.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/circinhom.py` & `timml-6.1.2/timml/circinhom.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/constant.py` & `timml-6.1.2/timml/constant.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/controlpoints.py` & `timml-6.1.2/timml/controlpoints.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/element.py` & `timml-6.1.2/timml/element.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/equation.py` & `timml-6.1.2/timml/equation.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/inhomogeneity.py` & `timml-6.1.2/timml/inhomogeneity.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/inhomogeneity1d.py` & `timml-6.1.2/timml/inhomogeneity1d.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/intlinesink.py` & `timml-6.1.2/timml/intlinesink.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/linedoublet.py` & `timml-6.1.2/timml/linedoublet.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/linedoublet1d.py` & `timml-6.1.2/timml/linedoublet1d.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/linesink.py` & `timml-6.1.2/timml/linesink.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/linesink1d.py` & `timml-6.1.2/timml/linesink1d.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/model.py` & `timml-6.1.2/timml/model.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/src/besselaesnew.f95` & `timml-6.1.2/timml/src/besselaesnew.f95`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/stripareasink.py` & `timml-6.1.2/timml/stripareasink.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/trace.py` & `timml-6.1.2/timml/trace.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/uflow.py` & `timml-6.1.2/timml/uflow.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/util.py` & `timml-6.1.2/timml/util.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml/well.py` & `timml-6.1.2/timml/well.py`

 * *Files identical despite different names*

### Comparing `timml-6.1.0/timml.egg-info/PKG-INFO` & `timml-6.1.2/timml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timml
-Version: 6.1.0
+Version: 6.1.2
 Summary: Steady multi-layer AEM Model
 Home-page: https://github.com/mbakker7/timml
 Author: Mark Bakker
 Author-email: markbak@gmail.com
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >3.5
```

### Comparing `timml-6.1.0/timml.egg-info/SOURCES.txt` & `timml-6.1.2/timml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

