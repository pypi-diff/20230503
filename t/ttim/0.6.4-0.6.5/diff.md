# Comparing `tmp/ttim-0.6.4.tar.gz` & `tmp/ttim-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttim-0.6.4.tar", last modified: Mon Mar 20 16:21:28 2023, max compression
+gzip compressed data, was "ttim-0.6.5.tar", last modified: Wed May  3 19:41:00 2023, max compression
```

## Comparing `ttim-0.6.4.tar` & `ttim-0.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:21:28.302145 ttim-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-20 16:21:16.000000 ttim-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-20 16:21:16.000000 ttim-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-20 16:21:28.302145 ttim-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-20 16:21:16.000000 ttim-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 16:21:28.302145 ttim-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-20 16:21:16.000000 ttim-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:21:28.302145 ttim-0.6.4/ttim/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/aquifer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/aquifer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/aquifernew.py
--rw-r--r--   0 runner    (1001) docker     (123)    63596 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/besselnumba.py
--rw-r--r--   0 runner    (1001) docker     (123)    77989 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/besselnumba_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/circareasink.py
--rw-r--r--   0 runner    (1001) docker     (123)    32556 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/circinhom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/equation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/invlapnumba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/kuhlman_invlap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/linedoublet.py
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/linesink.py
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-03-20 16:21:16.000000 ttim-0.6.4/ttim/well.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 16:21:28.302145 ttim-0.6.4/ttim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-20 16:21:28.000000 ttim-0.6.4/ttim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-20 16:21:28.000000 ttim-0.6.4/ttim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 16:21:28.000000 ttim-0.6.4/ttim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-20 16:21:28.000000 ttim-0.6.4/ttim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-20 16:21:28.000000 ttim-0.6.4/ttim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:41:00.643050 ttim-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 19:40:48.000000 ttim-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 19:40:48.000000 ttim-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-03 19:41:00.643050 ttim-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-03 19:40:48.000000 ttim-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:41:00.643050 ttim-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 19:40:48.000000 ttim-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:41:00.643050 ttim-0.6.5/ttim/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/aquifer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/aquifer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/aquifernew.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63347 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/besselnumba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77683 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/besselnumba_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/circareasink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32556 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/circinhom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/invlapnumba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/kuhlman_invlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/linedoublet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/linesink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-05-03 19:40:48.000000 ttim-0.6.5/ttim/well.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:41:00.643050 ttim-0.6.5/ttim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-03 19:41:00.000000 ttim-0.6.5/ttim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 19:41:00.000000 ttim-0.6.5/ttim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:41:00.000000 ttim-0.6.5/ttim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 19:41:00.000000 ttim-0.6.5/ttim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 19:41:00.000000 ttim-0.6.5/ttim.egg-info/top_level.txt
```

### Comparing `ttim-0.6.4/LICENSE` & `ttim-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/PKG-INFO` & `ttim-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttim
-Version: 0.6.4
+Version: 0.6.5
 Summary: Transient multi-layer AEM Model
 Home-page: https://github.com/mbakker7/ttim
 Author: Mark Bakker
 Author-email: markbak@gmail.com
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.7
```

### Comparing `ttim-0.6.4/README.md` & `ttim-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/setup.py` & `ttim-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/__init__.py` & `ttim-0.6.5/ttim/__init__.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/aquifer.py` & `ttim-0.6.5/ttim/aquifer.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/aquifer_parameters.py` & `ttim-0.6.5/ttim/aquifer_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,19 +36,24 @@
         assert len(c) == naq - 1, 'Error: Length of c needs to be ' + \
                                   str(naq - 1)
         assert len(Sll) == naq - 1, 'Error: Length of Sll needs to be ' + \
                                   str(naq - 1)
         assert len(porll) == naq - 1, 'Error: Length of porll needs to be ' + \
                                   str(naq - 1)
         Haq = H[::2]
+        assert np.all(Haq > 0), 'Error: Some thicknesses of aquifer layers ' + \
+                                'are negative'
         Hll = H[1::2]
+        Hll = np.maximum(Hll, 1e-20) # make sure none are negative
+        assert np.all(Hll > 0), 'Error: Some thicknesses of leaky layers ' + \
+                                'are negative'
         c = np.hstack((1e100, c))  
-        Sll = np.hstack((1e-30, Sll)) 
-        Hll = np.hstack((1e-30, Hll))
-        porll = np.hstack((1e-30, porll))
+        Sll = np.hstack((1e-20, Sll)) 
+        Hll = np.hstack((1e-20, Hll))
+        porll = np.hstack((1e-20, porll))
         # layertype
         nlayers = len(z) - 1
         ltype = np.array(nlayers * ['a'])
         ltype[1::2] = 'l'
     else: # leaky layers on top
         naq = int(len(z - 1) / 2)
         if len(kaq) == 1:
```

### Comparing `ttim-0.6.4/ttim/aquifernew.py` & `ttim-0.6.5/ttim/aquifernew.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/besselnumba.py` & `ttim-0.6.5/ttim/besselnumba.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,17 @@
     complex(kind=8) :: omega
     integer :: n, n2, ts
     real(kind=8) :: a, b, c, A3, u
     complex(kind=8) :: A1, A2, cn, cnp1, cnp2, cnp3
     complex(kind=8) :: z1, z2, S, T
 
     """
-    cnp1 = np.complex(1., 0.)
-    cnp2 = np.complex(0., 0.)
-    cnp3 = np.complex(0., 0.)
+    cnp1 = complex(1., 0.)
+    cnp2 = complex(0., 0.)
+    cnp3 = complex(0., 0.)
     a = 0.5
     c = 1.
     b = 1. + a - c
 
     z1 = 2. * z
     z2 = 2. * z1
     ts = (-1)**(Nt+1)
@@ -196,17 +196,17 @@
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2 * biga / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a * exprange
-    bnew = (b - a * np.complex(0, 2) * ang) * exprange
+    bnew = (b - a * complex(0, 2) * ang) * exprange
 
 #zminzbar = np.zeros(21, dtype=np.complex_)
 exprange = np.zeros(21, dtype=np.complex_)
 anew = np.zeros(21, dtype=np.complex_)
 bnew = np.zeros(21, dtype=np.complex_)
 
 @numba.njit(nogil=True, cache=True)
@@ -254,19 +254,19 @@
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2 * biga / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a * exprange
-    bnew = (b - a * np.complex(0, 2) * ang) * exprange
+    bnew = (b - a * complex(0, 2) * ang) * exprange
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     # #for n in range(21):
     # #    zminzbar[n] = (zeta-zetabar)**(20-n)  # Ordered from high power to low power
     zminzbar[20] = 1
 
     for n in range(1, 21):
         # Ordered from high power to low power
@@ -292,17 +292,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     omega = 0
     d1minzeta = -1/biglab - zeta
     d2minzeta = 1/biglab - zeta
 
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
 
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
     term1 = 1
     term2 = 1
 
     # I tried to serialize this, but it didn't speed things up
@@ -332,16 +332,16 @@
     complex(kind=8) :: omega
     integer :: n
     real(kind=8) :: L, x0
     complex(kind=8) :: bigz, biglab
     """
     L = np.abs(z2-z1)
     biglab = 2 * lab / L
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
-    omega = np.complex(0, 0)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
+    omega = complex(0, 0)
     for n in range(1, 9):
         x0 = bigz.real - xg[n-1]
         omega = omega + wg[n-1] * besselk0(x0, bigz.imag, biglab)
 
     omega = -L/(4*np.pi) * omega
     return omega
 
@@ -358,16 +358,16 @@
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L
     complex(kind=8) :: z, delz, za, zb
     """
 
     Lnear = 3.
-    z = np.complex(x, y)
-    omega = np.complex(0., 0.)
+    z = complex(x, y)
+    omega = complex(0., 0.)
     L = np.abs(z2-z1)
     if (L < Lnear * np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5 * (z1 + z2)) < 0.5 * Lnear * L):  # Do integration
             omega = bessells_int(x, y, z1, z2, lab)
         else:
             omega = bessells_gauss(x, y, z1, z2, lab)
     else:  # Break integral up in parts
@@ -412,16 +412,16 @@
     real(kind=8), intent(in) :: R
     real(kind=8), intent(inout) :: xouta, youta, xoutb, youtb
     integer, intent(inout) :: N
     real(kind=8) :: Lover2, d, xa, xb
     complex(kind=8) :: bigz, za, zb
     """
     N = 0
-    za = np.complex(0, 0)
-    zb = np.complex(0, 0)
+    za = complex(0, 0)
+    zb = complex(0, 0)
     Lover2 = np.abs(z2-z1) / 2
     bigz = (2*zc - (z1+z2)) * Lover2 / (z2-z1)
     if (abs(bigz.imag) < R):
         d = np.sqrt(R ** 2 - bigz.imag ** 2)
         xa = bigz.real - d
         xb = bigz.real + d
         if ((xa < Lover2) and (xb > -Lover2)):
@@ -449,15 +449,15 @@
     complex(kind=8), dimension(order+1,nlab) :: omega
     integer :: n, nterms
     """
     nlab = len(lab)
     nterms = order+1
     omega = np.zeros((order+1, nlab), dtype=np.complex_)
     # Check if endpoints need to be adjusted using the largest lambda (the first one)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         omega[:nterms+1, n] = bessells(x, y, z1, z2, lab[n], order, d1, d2)
     return omega
 
 @numba.njit(nogil=True, cache=True)
 def find_d1d2(z1, z2, zc, R):
     """
@@ -499,15 +499,15 @@
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
     """
     omega = np.zeros(order + 1, dtype=np.complex_)
     Lnear = 3
-    z = np.complex(x, y)
+    z = complex(x, y)
     L = np.abs(z2-z1)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             omega = bessells_int_ho(x, y, z1, z2, lab, order, d1in, d2in)
         else:
             omega = bessells_gauss_ho_d1d2(
                 x, y, z1, z2, lab, order, d1in, d2in)
@@ -552,19 +552,19 @@
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2 * biga / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a * exprange
-    bnew = (b - a * np.complex(0, 2) * ang) * exprange
+    bnew = (b - a * complex(0, 2) * ang) * exprange
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
 
     # #for n in range(21):
     # #    zminzbar[n] = (zeta-zetabar)**(20-n)  # Ordered from high power to low power
     #
     zminzbar = np.zeros(21, dtype=np.complex_)
     zminzbar[20] = 1
@@ -591,17 +591,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
     # #d1minzeta = -1/biglab - zeta
     # #d2minzeta = 1/biglab - zeta
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(51, dtype=np.complex_)
     alphanew2 = np.zeros(51, dtype=np.complex_)
     betanew = np.zeros(51, dtype=np.complex_)
 
@@ -649,24 +649,24 @@
     integer :: n, p
     real(kind=8) :: L, x0
     complex(kind=8) :: bigz, biglab
     complex(kind=8), dimension(8) :: k0
     """
     L = np.abs(z2-z1)
     biglab = 2 * lab / L
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
 
     k0 = np.zeros(8, dtype=np.complex_)
     for n in range(8):
         x0 = bigz.real - xg[n]
         k0[n] = besselk0(x0, bigz.imag, biglab)
 
     omega = np.zeros(order+1, dtype=np.complex_)
     for p in range(order+1):
-        omega[p] = np.complex(0, 0)
+        omega[p] = complex(0, 0)
         for n in range(8):
             omega[p] = omega[p] + wg[n] * xg[n]**p * k0[n]
         omega[p] = -L/(4*np.pi) * omega[p]
 
     return omega
 
 @numba.njit(nogil=True, cache=True)
@@ -680,16 +680,16 @@
     complex(kind=8), intent(in) :: z1,z2,lab
     complex(kind=8), dimension(0:order) :: omega, omegac
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
     omega = np.zeros(order+1, dtype=np.complex_)
-    bigz1 = np.complex(d1, 0)
-    bigz2 = np.complex(d2, 0)
+    bigz1 = complex(d1, 0)
+    bigz2 = complex(d2, 0)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     omegac = bessells_gauss_ho(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             omega[n] = omega[n] + gam[n, m] * dc**(n-m) * omegac[m]
@@ -731,15 +731,15 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqylab
     integer :: n, nterms, nhalf
     """
     nlab = len(lab)
     qxqy = np.zeros((2*(order+1), nlab), dtype=np.complex_)
     nterms = order+1
     nhalf = nlab*(order+1)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         qxqylab = bessellsqxqy(x, y, z1, z2, lab[n], order, d1, d2)
         qxqy[:nterms, n] = qxqylab[0:order + 1]
         qxqy[nterms:2 * nterms, n] = qxqylab[order + 1:2 * (order + 1)]
     return qxqy
 
 @numba.njit(nogil=True, cache=True)
@@ -753,15 +753,15 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqy
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
     """
     Lnear = 3.
-    z = np.complex(x, y)
+    z = complex(x, y)
     qxqy = np.zeros(2 * order + 2, dtype=np.complex_)
     L = np.abs(z2-z1)
     # print *,'Lnear*np.abs(lab) ',Lnear*np.abs(lab)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             qxqy = bessells_int_ho_qxqy(x, y, z1, z2, lab, order, d1in, d2in)
         else:
@@ -812,30 +812,30 @@
     complex(kind=8), dimension(0:order) :: omegalap ! To store intermediate result
 
     integer :: m, n, p
     """
     zminzbar = np.zeros(21, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     bigx = bigz.real
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     angz = np.arctan2((z2-z1).imag, (z2-z1).real)
     biglab = 2 * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[20] = 1
 
     for n in range(1, 21):
         # Ordered from high power to low po
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -856,17 +856,17 @@
         beta[n:2*n+1] = beta[n:2*n+1] + bnew[n] * gamnew[n, 0:n+1]
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1 / biglab - zeta
     d2minzeta = d2 / biglab - zeta
 
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(52, dtype=np.complex_)
     alphanew2 = np.zeros(52, dtype=np.complex_)
     betanew = np.zeros(52, dtype=np.complex_)
 
@@ -924,16 +924,16 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqy, qxqyc
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     qxqyc = bessells_gauss_ho_qxqy(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             qxqy[n] = qxqy[n] + gam[n, m] * dc**(n-m) * qxqyc[m]
@@ -956,16 +956,16 @@
     complex(kind=8), dimension(0:order) :: omega, omegac
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
     omega = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     omegac = lapld_int_ho(x, y, z1p, z2p, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             omega[n] = omega[n] + gam[n, m] * dc**(n-m) * omegac[m]
@@ -987,15 +987,15 @@
     complex(kind=8) :: z, zplus1, zmin1
     """
 
     omega = np.zeros(order+1, dtype=np.complex_)
     qm = np.zeros(order+1, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    z = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    z = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     zplus1 = z + 1.
     zmin1 = z - 1.
     # Not sure if this gives correct answer at corner point (z also appears in qm); should really be caught in code that calls this function
     if np.abs(zplus1) < tiny:
         zplus1 = tiny
     if np.abs(zmin1) < tiny:
         zmin1 = tiny
@@ -1008,15 +1008,15 @@
         qm[1] = 2.
     for m in range(3, order+1, 2):
         qm[m] = qm[m-2] * z * z + 2. / m
 
     for m in range(2, order+1, 2):
         qm[m] = qm[m-1] * z
 
-    omega = 1. / (np.complex(0., 2.) * np.pi) * (omega + qm)
+    omega = 1. / (complex(0., 2.) * np.pi) * (omega + qm)
     return omega
 
 @numba.njit(nogil=True, cache=True)
 def bessells_gauss_ho_qxqy(x, y, z1, z2, lab, order):
     """
     implicit none
     integer, intent(in) :: order
@@ -1034,15 +1034,15 @@
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
     xmind = np.zeros(8, dtype=np.complex_)
     k1 = np.zeros(8, dtype=np.complex_)
     r = np.zeros(8, dtype=np.complex_)
 
     L = np.abs(z2-z1)
     biglab = 2 * lab / L
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     for n in range(8):
         xmind[n] = bigz.real - xg[n]
         r[n] = np.sqrt(xmind[n]**2 + bigz.imag**2)
         k1[n] = besselk1(xmind[n], bigz.imag, biglab)
 
     qx = np.zeros(order+1, dtype=np.complex_)
@@ -1163,15 +1163,15 @@
     integer :: n, nterms
     """
     nlab = len(lab)
     omega = np.zeros((order+1, nlab), dtype=np.complex_)
 
     nterms = order+1
     # Check if endpoints need to be adjusted using the largest lambda (the first one)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         omega[:nterms+1, n] = besselld(x, y, z1, z2, lab[n], order, d1, d2)
 
     return omega
 
 @numba.njit(nogil=True, cache=True)
 def besselld(x, y, z1, z2, lab, order, d1in, d2in):
@@ -1187,15 +1187,15 @@
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
     """
 
     omega = np.zeros(order+1, dtype=np.complex_)
 
     Lnear = 3.
-    z = np.complex(x, y)
+    z = complex(x, y)
     L = np.abs(z2-z1)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             omega = besselld_int_ho(x, y, z1, z2, lab, order, d1in, d2in)
         else:
             omega = besselld_gauss_ho_d1d2(
                 x, y, z1, z2, lab, order, d1in, d2in)
@@ -1240,28 +1240,28 @@
     integer :: m, n, p
     """
 
     zminzbar = np.zeros(21, dtype=np.complex_)
     omega = np.zeros(order+1, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2. * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
 
-    zeta = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2. * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[20] = 1.
     for n in range(1, 21):
         # Ordered from high power to low power
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
 
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -1283,17 +1283,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
     #d1minzeta = -1./biglab - zeta
     #d2minzeta = 1./biglab - zeta
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0.)
+        d1minzeta = d1minzeta + complex(tol, 0.)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0.)
+        d2minzeta = d2minzeta + complex(tol, 0.)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(51, dtype=np.complex_)
     alphanew2 = np.zeros(51, dtype=np.complex_)
     betanew = np.zeros(51, dtype=np.complex_)
 
@@ -1340,16 +1340,16 @@
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
 
     omega = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     omegac = besselld_gauss_ho(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     omega[0:order+1] = 0.
     for n in range(order+1):
         for m in range(n+1):
@@ -1373,21 +1373,21 @@
     """
 
     k1overr = np.zeros(8, dtype=np.complex_)
     omega = np.zeros(order+1, dtype=np.complex_)
 
     L = np.abs(z2-z1)
     biglab = 2. * lab / L
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     for n in range(8):
         x0 = bigz.real - xg[n]
         r = np.sqrt(x0**2 + bigz.imag**2)
         k1overr[n] = besselk1(x0, bigz.imag, biglab) / r
     for p in range(order+1):
-        omega[p] = np.complex(0., 0.)
+        omega[p] = complex(0., 0.)
         for n in range(8):
             omega[p] = omega[p] + wg[n] * xg[n]**p * k1overr[n]
         omega[p] = bigz.imag/(2.*np.pi*biglab) * omega[p]
     return omega
 
 @numba.njit(nogil=True, cache=True)
 def besselldqxqyv2(x, y, z1, z2, lab, order, R):
@@ -1403,15 +1403,15 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqylab
     integer :: n, nterms, nhalf
     """
     nlab = len(lab)
     qxqy = np.zeros((2*(order+1), nlab), dtype=np.complex_)
     nterms = order+1
     nhalf = nlab*(order+1)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         qxqylab = besselldqxqy(x, y, z1, z2, lab[n], order, d1, d2)
         qxqy[:nterms, n] = qxqylab[0:order+1]
         qxqy[nterms:2*nterms, n] = qxqylab[order+1:2*order+1+1]
     return qxqy
 
 @numba.njit(nogil=True, cache=True)
@@ -1426,15 +1426,15 @@
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
 
     """
     Lnear = 3
-    z = np.complex(x, y)
+    z = complex(x, y)
     qxqy = np.zeros(2 * order + 2, dtype=np.complex_)
     
     L = np.abs(z2-z1)
 
     # print *,'Lnear*np.abs(lab) ',Lnear*np.abs(lab)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
@@ -1489,37 +1489,37 @@
     """
 
     zminzbar = np.zeros(21, dtype=np.complex_)
     omega = np.zeros(order+2, dtype=np.complex_)
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     angz = np.arctan2((z2-z1).imag, (z2-z1).real)
     biglab = 2 * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
     azero = anew[0]
 
     for n in range(20):
         bnew[n] = (n+1)*bnew[n+1] + anew[n+1]
         anew[n] = (n+1)*anew[n+1]
 
     anew[20] = 0  # This is a bit lazy
     bnew[20] = 0
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[20] = 1
     for n in range(1, 21):
         # Ordered from high power to low power
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
 
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -1542,17 +1542,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
     # d1minzeta = -1/biglab - zeta
     # d2minzeta = 1/biglab - zeta
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
 
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(52, dtype=np.complex_)
     alphanew2 = np.zeros(52, dtype=np.complex_)
     betanew = np.zeros(52, dtype=np.complex_)
@@ -1581,40 +1581,40 @@
                                    alphanew[n] / (n+1) + betanew[n]) * term1 / (n+1)
             omega[p] = omega[p] + (alphanew2[n] * np.conj(log2) -
                                    alphanew2[n] / (n+1)) * np.conj(term2) / (n+1)
             omega[p] = omega[p] - (alphanew2[n] * np.conj(log1) -
                                    alphanew2[n] / (n+1)) * np.conj(term1) / (n+1)
 
     omegalap = lapld_int_ho_d1d2(
-        x, y, z1, z2, order, d1, d2) / np.complex(0, 1)
+        x, y, z1, z2, order, d1, d2) / complex(0, 1)
     omegaom = besselldpart(x, y, z1, z2, lab, order, d1, d2)
     wdis = lapld_int_ho_wdis_d1d2(x, y, z1, z2, order, d1, d2)
 
     rvz = -biglab * bigy / (2*np.pi*biglabcomplex**2) * (omega[1:order+1+1]/biglab - zetabar * omega[0:order+1]) + \
-        biglab * omegaom / np.complex(0, 2)
+        biglab * omegaom / complex(0, 2)
     rvzbar = -biglab * bigy / (2*np.pi*biglabcomplex**2) * (omega[1:order+1+1]/biglab - zeta * omega[0:order+1]) - \
-        biglab * omegaom / np.complex(0, 2)
+        biglab * omegaom / complex(0, 2)
     # qxqy[0:order+1] = -2.0 / L * ( rvz + rvzbar ) / biglab  # As we need to take derivative w.r.t. z not zeta
-    # qxqy[order+1:2*order+1+1] = -2.0 / L * np.complex(0,1) * (rvz-rvzbar) / biglab
+    # qxqy[order+1:2*order+1+1] = -2.0 / L * complex(0,1) * (rvz-rvzbar) / biglab
     #
     # qxqy[0:order+1] = qxqy[0:order+1] - 2.0 / L / biglabcomplex**2 * azero * ( omegalap + np.conj(omegalap) )
     # qxqy[order+1:2*order+1+1] = qxqy[order+1:2*order+1+1] -  \
-    #                          2.0 / L / biglabcomplex**2 * azero * np.complex(0,1) * (omegalap - np.conj(omegalap))
+    #                          2.0 / L / biglabcomplex**2 * azero * complex(0,1) * (omegalap - np.conj(omegalap))
     #
     # qxqy[0:order+1] = qxqy[0:order+1] + real(wdis)
     # qxqy[order+1:2*order+1+1] = qxqy[order+1:2*order+1+1] - aimag(wdis)
 
     # As we need to take derivative w.r.t. z not zeta
     qx = -2.0 / L * (rvz + rvzbar) / biglab
-    qy = -2.0 / L * np.complex(0, 1) * (rvz-rvzbar) / biglab
+    qy = -2.0 / L * complex(0, 1) * (rvz-rvzbar) / biglab
 
     qx = qx - 2.0 / L * bigy / biglabcomplex**2 * \
         azero * (omegalap + np.conj(omegalap))
     qy = qy - 2.0 / L * bigy / biglabcomplex**2 * azero * \
-        np.complex(0, 1) * (omegalap - np.conj(omegalap))
+        complex(0, 1) * (omegalap - np.conj(omegalap))
 
     # qx = qx + real(wdis * (z2-z1) / L)
     # qy = qy - aimag(wdis * (z2-z1) / L)
 
     # print *,'angz ',angz
     # wdis already includes the correct rotation
     qxqy[0:order+1] = qx * np.cos(angz) - qy * np.sin(angz) + wdis.real
@@ -1636,16 +1636,16 @@
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
 
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0)
-    bigz2 = np.complex(d2, 0)
+    bigz1 = complex(d1, 0)
+    bigz2 = complex(d2, 0)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     qxqyc = besselld_gauss_ho_qxqy(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             qxqy[n] = qxqy[n] + gam[n, m] * dc**(n-m) * qxqyc[m]
@@ -1678,15 +1678,15 @@
     r = np.zeros(8, dtype=np.float_)
     k0 = np.zeros(8, dtype=np.complex_)
     k1 = np.zeros(8, dtype=np.complex_)
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
     L = np.abs(z2-z1)
     biglab = 2. * lab / L
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     for n in range(8):
         xmind[n] = bigz.real - xg[n]
         r[n] = np.sqrt(xmind[n]**2 + bigz.imag**2)
         k0[n] = besselk0(xmind[n], bigz.imag, biglab)
         k1[n] = besselk1(xmind[n], bigz.imag, biglab)
 
@@ -1726,28 +1726,28 @@
     complex(kind=8), dimension(0:40) :: alpha, beta, alpha2
     complex(kind=8), dimension(0:50) :: alphanew, betanew, alphanew2 ! Order fixed to 10
     integer :: m, n, p
     """
     zminzbar = np.zeros(21, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2. * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
 
-    zeta = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2. * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[-1] = 1.
     for n in range(1, 21):
         # Ordered from high power to low power
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
 
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -1767,17 +1767,17 @@
         beta[n:2*n+1] = beta[n:2*n+1] + bnew[n] * gamnew[n, 0:n+1]
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
 
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0.)
+        d1minzeta = d1minzeta + complex(tol, 0.)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0.)
+        d2minzeta = d2minzeta + complex(tol, 0.)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(51, dtype=np.complex_)
     alphanew2 = np.zeros(51, dtype=np.complex_)
     betanew = np.zeros(51, dtype=np.complex_)
     omega = np.zeros(order+1, dtype=np.complex_)
@@ -1828,16 +1828,16 @@
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
 
     wdis = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     wdisc = lapld_int_ho_wdis(x, y, z1p, z2p, order)
     dc = (d1+d2) / (d2-d1)
     wdis[0:order+1] = 0.
     for n in range(order+1):
         for m in range(n+1):
@@ -1858,15 +1858,15 @@
     integer :: m, n
     complex(kind=8) :: z, zplus1, zmin1, term1, term2, zterm
     """
 
     qm = np.zeros(11, dtype=np.complex_)
     wdis = np.zeros(order+1, dtype=np.complex_)
 
-    z = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    z = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     zplus1 = z + 1.
     zmin1 = z - 1.
     # Not sure if this gives correct answer at corner point (z also appears in qm); should really be caught in code that calls this function
     if (np.abs(zplus1) < tiny):
         zplus1 = tiny
     if (np.abs(zmin1) < tiny):
         zmin1 = tiny
@@ -1876,16 +1876,16 @@
         qm[m] = 0.
         for n in range(1, m//2):
             qm[m] = qm[m] + (m-2*n+1) * z**(m-2*n) / (2*n-1)
 
     term1 = 1. / zmin1 - 1. / zplus1
     term2 = np.log(zmin1/zplus1)
     wdis[0] = term1
-    zterm = np.complex(1., 0.)
+    zterm = complex(1., 0.)
     for m in range(1, order+1):
         wdis[m] = m * zterm * term2 + z * zterm * term1 + 2. * qm[m]
         zterm = zterm * z
 
-    wdis = - wdis / (np.pi*np.complex(0., 1.)*(z2-z1))
+    wdis = - wdis / (np.pi*complex(0., 1.)*(z2-z1))
     return wdis
```

### Comparing `ttim-0.6.4/ttim/besselnumba_total.py` & `ttim-0.6.5/ttim/besselnumba_total.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,17 +165,17 @@
     complex(kind=8) :: omega
     integer :: n, n2, ts
     real(kind=8) :: a, b, c, A3, u
     complex(kind=8) :: A1, A2, cn, cnp1, cnp2, cnp3
     complex(kind=8) :: z1, z2, S, T
 
     """
-    cnp1 = np.complex(1., 0.)
-    cnp2 = np.complex(0., 0.)
-    cnp3 = np.complex(0., 0.)
+    cnp1 = complex(1., 0.)
+    cnp2 = complex(0., 0.)
+    cnp3 = complex(0., 0.)
     a = 0.5
     c = 1.
     b = 1. + a - c
 
     z1 = 2. * z
     z2 = 2. * z1
     ts = (-1)**(Nt+1)
@@ -391,17 +391,17 @@
 #     integer :: n, n2, ts
 #     real(kind=8) :: A3, u, b
 #     complex(kind=8) :: A1, A2, cn,cnp1,cnp2,cnp3
 #     complex(kind=8) :: z2, S, T
 # 
 #     """
 # 
-#     cnp1 = np.complex(1.)
-#     cnp2 = np.complex(0.)
-#     cnp3 = np.complex(0.)
+#     cnp1 = complex(1.)
+#     cnp2 = complex(0.)
+#     cnp3 = complex(0.)
 #     ts = (-1)**(n0+1)
 #     S = ts
 #     T = 1.
 #     z2 = 2. * z
 #     b = 1. + a - c
 # 
 #     for n in range(n0, -1, -1):
@@ -433,15 +433,15 @@
 #     real(kind=8) :: d
 #     complex(kind=8) :: zeta, zetabar, omega, logdminzdminzbar, dminzeta, term
 #     complex(kind=8), dimension(0:20) :: zminzbar
 #     complex(kind=8), dimension(0:20,0:20) :: gamnew
 #     complex(kind=8), dimension(0:40) :: alpha, beta
 #     """
 #     d = 0.
-#     zeta = np.complex(x, y)
+#     zeta = complex(x, y)
 #     zetabar = np.conj(zeta)
 #     zminzbar = np.zeros(21, dtype=np.complex_)
 #     for n in range(21):
 #         # Ordered from high power to low power
 #         zminzbar[n] = (zeta-zetabar)**(20-n)
 # 
 #     gamnew = np.asarray(gam, dtype=np.complex_)
@@ -452,15 +452,15 @@
 #     beta = np.zeros(41, dtype=np.complex_)
 #     alpha[0] = a[0]
 #     beta[0] = b[0]
 #     for n in range(1, 21):
 #         alpha[n:2*n+1] = alpha[n:2*n+1] + a[n] * gamnew[n, :n+1]
 #         beta[n:2*n+1] = beta[n:2*n+1] + b[n] * gamnew[n, :n+1]
 # 
-#     omega = np.complex(0., 0.)
+#     omega = complex(0., 0.)
 #     logdminzdminzbar = np.log((d-zeta) * (d-zetabar))
 #     dminzeta = d - zeta
 #     term = 1.
 # 
 #     for n in range(41):
 #         omega = omega + (alpha[n] * logdminzdminzbar + beta[n]) * term
 #         term = term * dminzeta
@@ -483,15 +483,15 @@
     real(kind=8) :: L
     complex(kind=8) :: z, zplus1, zmin1, log1, log2, log3, zpower
     """
     omega = np.empty((order+1,), dtype=np.complex_)
     qm = np.empty((order+2,), dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    z = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    z = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     zplus1 = z + 1
     zmin1 = z - 1
 
     # Not sure if this gives correct answer at corner point(z also appears in qm)
     # should really be caught in code that calls this def
     if (np.abs(zplus1) < tiny):
         zplus1 = tiny
@@ -529,21 +529,21 @@
     complex(kind=8), dimension(0:20) :: zminzbar
     complex(kind=8), dimension(0:20,0:20) :: gamnew
     complex(kind=8), dimension(0:40) :: alpha, beta
 
     """
     zminzbar = np.zeros(21, dtype=np.complex_)
 
-    z1 = np.complex(x1, y1)
-    z2 = np.complex(x2, y2)
+    z1 = complex(x1, y1)
+    z2 = complex(x2, y2)
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     biglab = 2 * biga / L
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     for n in range(21):
         # Ordered from high power to low power
         zminzbar[n] = (zeta-zetabar)**(20-n)
     gamnew = np.zeros((21, 21), dtype=np.complex_)
     for n in range(21):
         gamnew[n, 0:n+1] = gam[n, 0:n+1] * zminzbar[20-n:20+1]
@@ -593,21 +593,21 @@
     complex(kind=8) :: cm
     complex(kind=8), dimension(0:50) :: alphanew, betanew ! Maximum programmed order is 10
     integer :: n, m, p
     """
     phi = np.zeros(order+1, dtype=np.float_)
     zminzbar = np.zeros(21, dtype=np.complex_)
 
-    z1 = np.complex(x1, y1)
-    z2 = np.complex(x2, y2)
+    z1 = complex(x1, y1)
+    z2 = complex(x2, y2)
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     biglab = 2 * biga / L
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     for n in range(21):
         # Ordered from high power to low power
         zminzbar[n] = (zeta-zetabar)**(20-n)
         
     gamnew = np.zeros((21, 21), dtype=np.complex_)
     for n in range(21):
@@ -674,19 +674,19 @@
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2 * biga / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a * exprange
-    bnew = (b - a * np.complex(0, 2) * ang) * exprange
+    bnew = (b - a * complex(0, 2) * ang) * exprange
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     # #for n in range(21):
     # #    zminzbar[n] = (zeta-zetabar)**(20-n)  # Ordered from high power to low power
     zminzbar[20] = 1
 
     for n in range(1, 21):
         # Ordered from high power to low power
@@ -712,17 +712,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     omega = 0
     d1minzeta = -1/biglab - zeta
     d2minzeta = 1/biglab - zeta
 
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
 
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
     term1 = 1
     term2 = 1
 
     # I tried to serialize this, but it didn't speed things up
@@ -762,19 +762,19 @@
     L = np.abs(z2-z1)
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2 * biga / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a * exprange
-    bnew = (b - a * np.complex(0, 2) * ang) * exprange
+    bnew = (b - a * complex(0, 2) * ang) * exprange
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
 
     # #for n in range(21):
     # #    zminzbar[n] = (zeta-zetabar)**(20-n)  # Ordered from high power to low power
     #
     zminzbar = np.zeros(21, dtype=np.complex_)
     zminzbar[20] = 1
@@ -801,17 +801,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
     # #d1minzeta = -1/biglab - zeta
     # #d2minzeta = 1/biglab - zeta
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(51, dtype=np.complex_)
     alphanew2 = np.zeros(51, dtype=np.complex_)
     betanew = np.zeros(51, dtype=np.complex_)
 
@@ -869,30 +869,30 @@
     complex(kind=8), dimension(0:order) :: omegalap ! To store intermediate result
 
     integer :: m, n, p
     """
     zminzbar = np.zeros(21, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     bigx = bigz.real
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     angz = np.arctan2((z2-z1).imag, (z2-z1).real)
     biglab = 2 * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[20] = 1
 
     for n in range(1, 21):
         # Ordered from high power to low po
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -913,17 +913,17 @@
         beta[n:2*n+1] = beta[n:2*n+1] + bnew[n] * gamnew[n, 0:n+1]
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1 / biglab - zeta
     d2minzeta = d2 / biglab - zeta
 
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(52, dtype=np.complex_)
     alphanew2 = np.zeros(52, dtype=np.complex_)
     betanew = np.zeros(52, dtype=np.complex_)
 
@@ -980,16 +980,16 @@
     complex(kind=8) :: omega
     integer :: n
     real(kind=8) :: L, x0
     complex(kind=8) :: bigz, biglab
     """
     L = np.abs(z2-z1)
     biglab = 2 * lab / L
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
-    omega = np.complex(0, 0)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
+    omega = complex(0, 0)
     for n in range(1, 9):
         x0 = bigz.real - xg[n-1]
         omega = omega + wg[n-1] * besselk0(x0, bigz.imag, biglab)
 
     omega = -L/(4*np.pi) * omega
     return omega
 
@@ -1006,24 +1006,24 @@
     integer :: n, p
     real(kind=8) :: L, x0
     complex(kind=8) :: bigz, biglab
     complex(kind=8), dimension(8) :: k0
     """
     L = np.abs(z2-z1)
     biglab = 2 * lab / L
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
 
     k0 = np.zeros(8, dtype=np.complex_)
     for n in range(8):
         x0 = bigz.real - xg[n]
         k0[n] = besselk0(x0, bigz.imag, biglab)
 
     omega = np.zeros(order+1, dtype=np.complex_)
     for p in range(order+1):
-        omega[p] = np.complex(0, 0)
+        omega[p] = complex(0, 0)
         for n in range(8):
             omega[p] = omega[p] + wg[n] * xg[n]**p * k0[n]
         omega[p] = -L/(4*np.pi) * omega[p]
 
     return omega
 
 
@@ -1039,16 +1039,16 @@
     complex(kind=8), dimension(0:order) :: omega, omegac
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
     omega = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0)
-    bigz2 = np.complex(d2, 0)
+    bigz1 = complex(d1, 0)
+    bigz2 = complex(d2, 0)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     omegac = bessells_gauss_ho(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             omega[n] = omega[n] + gam[n, m] * dc**(n-m) * omegac[m]
@@ -1075,15 +1075,15 @@
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
     xmind = np.zeros(8, dtype=np.complex_)
     k1 = np.zeros(8, dtype=np.complex_)
     r = np.zeros(8, dtype=np.complex_)
 
     L = np.abs(z2-z1)
     biglab = 2 * lab / L
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     for n in range(8):
         xmind[n] = bigz.real - xg[n]
         r[n] = np.sqrt(xmind[n]**2 + bigz.imag**2)
         k1[n] = besselk1(xmind[n], bigz.imag, biglab)
 
     qx = np.zeros(order+1, dtype=np.complex_)
@@ -1115,16 +1115,16 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqy, qxqyc
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     qxqyc = bessells_gauss_ho_qxqy(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             qxqy[n] = qxqy[n] + gam[n, m] * dc**(n-m) * qxqyc[m]
@@ -1149,15 +1149,15 @@
     integer :: Nls, n
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
     """
     omega = np.zeros(order+1, dtype=np.complex_)
 
     Lnear = 3
-    z = np.complex(x, y)
+    z = complex(x, y)
     L = np.abs(z2-z1)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             omega = bessells_int_ho(x, y, z1, z2, lab, order, d1in, d2in)
         else:
             omega = bessells_gauss_ho_d1d2(
                 x, y, z1, z2, lab, order, d1in, d2in)
@@ -1197,15 +1197,15 @@
     complex(kind=8), dimension(nlab*(order+1)) :: omega
     integer :: n, nterms
     """
     nterms = order+1
     omega = np.zeros(nlab*(order+1), dtype=np.complex_)
     # Check if endpoints need to be adjusted using
     # the largest lambda (the first one)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(0, nlab):
         omega[n*nterms:(n+1)*nterms] = bessells(x, y, z1, z2, lab[n],
                                                   order, d1, d2)
     return omega
 
 
 @numba.njit(nogil=True, cache=True)
@@ -1220,15 +1220,15 @@
     complex(kind=8), dimension(nlab), intent(in) :: lab
     complex(kind=8), dimension(order+1,nlab) :: omega
     integer :: n, nterms
     """
     nterms = order+1
     omega = np.zeros((order+1, nlab), dtype=np.complex_)
     # Check if endpoints need to be adjusted using the largest lambda (the first one)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         omega[:nterms+1, n] = bessells(x, y, z1, z2, lab[n], order, d1, d2)
     return omega
 
 
 @numba.njit(nogil=True, cache=True)
 def bessellsqxqy(x, y, z1, z2, lab, order, d1in, d2in):
@@ -1241,15 +1241,15 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqy
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
     """
     Lnear = 3.
-    z = np.complex(x, y)
+    z = complex(x, y)
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
     L = np.abs(z2-z1)
     # print *,'Lnear*np.abs(lab) ',Lnear*np.abs(lab)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             qxqy = bessells_int_ho_qxqy(x, y, z1, z2, lab, order, d1in, d2in)
         else:
@@ -1294,15 +1294,15 @@
     complex(kind=8), dimension(2*nlab*(order+1)) :: qxqy
     complex(kind=8), dimension(0:2*order+1) :: qxqylab
     integer :: n, nterms, nhalf
     """
     qxqy = np.zeros(2*nlab*(order+1), dtype=np.complex_)
     nterms = order+1
     nhalf = nlab*(order+1)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         qxqylab = bessellsqxqy(x, y, z1, z2, lab[n], order, d1, d2)
         qxqy[(n)*nterms:(n+1)*nterms] = qxqylab[0:order+1]
         qxqy[(n)*nterms+nhalf:(n+1)*nterms +
              nhalf] = qxqylab[order+1:2*order+1+1]
     return qxqy
 
@@ -1320,15 +1320,15 @@
     complex(kind=8), dimension(2*(order+1),nlab) :: qxqy
     complex(kind=8), dimension(0:2*order+1) :: qxqylab
     integer :: n, nterms, nhalf
     """
     qxqy = np.zeros((2*(order+1), nlab), dtype=np.complex_)
     nterms = order+1
     nhalf = nlab*(order+1)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         qxqylab = bessellsqxqy(x, y, z1, z2, lab[n-1], order, d1, d2)
         qxqy[:nterms, n] = qxqylab[0:order+1]
         qxqy[nterms:2*nterms, n] = qxqylab[order+1:2*order+1+1]
     return qxqy
 
 
@@ -1344,16 +1344,16 @@
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L
     complex(kind=8) :: z, delz, za, zb
     """
 
     Lnear = 3.
-    z = np.complex(x, y)
-    omega = np.complex(0., 0.)
+    z = complex(x, y)
+    omega = complex(0., 0.)
     L = np.abs(z2-z1)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             omega = bessells_int(x, y, z1, z2, lab)
         else:
             omega = bessells_gauss(x, y, z1, z2, lab)
     else:  # Break integral up in parts
@@ -1403,15 +1403,15 @@
     complex(kind=8) :: z, zplus1, zmin1
     """
 
     omega = np.zeros(order+1, dtype=np.complex_)
     qm = np.zeros(order+1, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    z = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    z = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     zplus1 = z + 1.
     zmin1 = z - 1.
     # Not sure if this gives correct answer at corner point (z also appears in qm); should really be caught in code that calls this function
     if np.abs(zplus1) < tiny:
         zplus1 = tiny
     if np.abs(zmin1) < tiny:
         zmin1 = tiny
@@ -1424,15 +1424,15 @@
         qm[1] = 2.
     for m in range(3, order+1, 2):
         qm[m] = qm[m-2] * z * z + 2. / m
 
     for m in range(2, order+1, 2):
         qm[m] = qm[m-1] * z
 
-    omega = 1. / (np.complex(0., 2.) * np.pi) * (omega + qm)
+    omega = 1. / (complex(0., 2.) * np.pi) * (omega + qm)
     return omega
 
 
 @numba.njit(nogil=True, cache=True)
 def lapld_int_ho_d1d2(x, y, z1, z2, order, d1, d2):
     """
     Near field only
@@ -1444,16 +1444,16 @@
     complex(kind=8), dimension(0:order) :: omega, omegac
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
     omega = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     omegac = lapld_int_ho(x, y, z1p, z2p, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             omega[n] = omega[n] + gam[n, m] * dc**(n-m) * omegac[m]
@@ -1475,15 +1475,15 @@
     integer :: m, n
     complex(kind=8) :: z, zplus1, zmin1, term1, term2, zterm
     """
 
     qm = np.zeros(11, dtype=np.complex_)
     wdis = np.zeros(order+1, dtype=np.complex_)
 
-    z = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    z = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     zplus1 = z + 1.
     zmin1 = z - 1.
     # Not sure if this gives correct answer at corner point (z also appears in qm); should really be caught in code that calls this function
     if (np.abs(zplus1) < tiny):
         zplus1 = tiny
     if (np.abs(zmin1) < tiny):
         zmin1 = tiny
@@ -1493,20 +1493,20 @@
         qm[m] = 0.
         for n in range(1, m//2):
             qm[m] = qm[m] + (m-2*n+1) * z**(m-2*n) / (2*n-1)
 
     term1 = 1. / zmin1 - 1. / zplus1
     term2 = np.log(zmin1/zplus1)
     wdis[0] = term1
-    zterm = np.complex(1., 0.)
+    zterm = complex(1., 0.)
     for m in range(1, order+1):
         wdis[m] = m * zterm * term2 + z * zterm * term1 + 2. * qm[m]
         zterm = zterm * z
 
-    wdis = - wdis / (np.pi*np.complex(0., 1.)*(z2-z1))
+    wdis = - wdis / (np.pi*complex(0., 1.)*(z2-z1))
     return wdis
 
 
 @numba.njit(nogil=True, cache=True)
 def lapld_int_ho_wdis_d1d2(x, y, z1, z2, order, d1, d2):
     """
     # Near field only
@@ -1519,16 +1519,16 @@
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
 
     wdis = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     wdisc = lapld_int_ho_wdis(x, y, z1p, z2p, order)
     dc = (d1+d2) / (d2-d1)
     wdis[0:order+1] = 0.
     for n in range(order+1):
         for m in range(n+1):
@@ -1556,28 +1556,28 @@
     integer :: m, n, p
     """
 
     zminzbar = np.zeros(21, dtype=np.complex_)
     omega = np.zeros(order+1, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2. * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
 
-    zeta = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2. * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[20] = 1.
     for n in range(1, 21):
         # Ordered from high power to low power
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
 
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -1599,17 +1599,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
     #d1minzeta = -1./biglab - zeta
     #d2minzeta = 1./biglab - zeta
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0.)
+        d1minzeta = d1minzeta + complex(tol, 0.)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0.)
+        d2minzeta = d2minzeta + complex(tol, 0.)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(51, dtype=np.complex_)
     alphanew2 = np.zeros(51, dtype=np.complex_)
     betanew = np.zeros(51, dtype=np.complex_)
 
@@ -1661,21 +1661,21 @@
     """
 
     k1overr = np.zeros(8, dtype=np.complex_)
     omega = np.zeros(order+1, dtype=np.complex_)
 
     L = np.abs(z2-z1)
     biglab = 2. * lab / L
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     for n in range(8):
         x0 = bigz.real - xg[n]
         r = np.sqrt(x0**2 + bigz.imag**2)
         k1overr[n] = besselk1(x0, bigz.imag, biglab) / r
     for p in range(order+1):
-        omega[p] = np.complex(0., 0.)
+        omega[p] = complex(0., 0.)
         for n in range(8):
             omega[p] = omega[p] + wg[n] * xg[n]**p * k1overr[n]
 
         omega[p] = bigz.imag/(2.*np.pi*biglab) * omega[p]
     return omega
 
 
@@ -1691,16 +1691,16 @@
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
 
     omega = np.zeros(order+1, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0.)
-    bigz2 = np.complex(d2, 0.)
+    bigz1 = complex(d1, 0.)
+    bigz2 = complex(d2, 0.)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     omegac = besselld_gauss_ho(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     omega[0:order+1] = 0.
     for n in range(order+1):
         for m in range(n+1):
@@ -1723,15 +1723,15 @@
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
     """
 
     omega = np.zeros(order+1, dtype=np.complex_)
 
     Lnear = 3.
-    z = np.complex(x, y)
+    z = complex(x, y)
     L = np.abs(z2-z1)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             omega = besselld_int_ho(x, y, z1, z2, lab, order, d1in, d2in)
         else:
             omega = besselld_gauss_ho_d1d2(
                 x, y, z1, z2, lab, order, d1in, d2in)
@@ -1773,15 +1773,15 @@
     integer :: n, nterms
     """
 
     omega = np.zeros(nlab*(order+1), dtype=np.complex_)
 
     nterms = order+1
     # Check if endpoints need to be adjusted using the largest lambda (the first one)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         omega[(n)*nterms:(n+1)*nterms] = besselld(x, y, z1, z2,
                                                   lab[n], order, d1, d2)
     return omega
 
 
 @numba.njit(nogil=True, cache=True)
@@ -1798,15 +1798,15 @@
     integer :: n, nterms
     """
 
     omega = np.zeros((order+1, nlab), dtype=np.complex_)
 
     nterms = order+1
     # Check if endpoints need to be adjusted using the largest lambda (the first one)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         omega[:nterms+1, n] = besselld(x, y, z1, z2, lab[n], order, d1, d2)
 
     return omega
 
 
 # @numba.njit(nogil=True, cache=True)
@@ -1825,28 +1825,28 @@
     complex(kind=8), dimension(0:40) :: alpha, beta, alpha2
     complex(kind=8), dimension(0:50) :: alphanew, betanew, alphanew2 ! Order fixed to 10
     integer :: m, n, p
     """
     zminzbar = np.zeros(21, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     biglab = 2. * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
 
-    zeta = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2. * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[-1] = 1.
     for n in range(1, 21):
         # Ordered from high power to low power
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
 
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -1866,17 +1866,17 @@
         beta[n:2*n+1] = beta[n:2*n+1] + bnew[n] * gamnew[n, 0:n+1]
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
 
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0.)
+        d1minzeta = d1minzeta + complex(tol, 0.)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0.)
+        d2minzeta = d2minzeta + complex(tol, 0.)
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(51, dtype=np.complex_)
     alphanew2 = np.zeros(51, dtype=np.complex_)
     betanew = np.zeros(51, dtype=np.complex_)
     omega = np.zeros(order+1, dtype=np.complex_)
@@ -1937,37 +1937,37 @@
     """
 
     zminzbar = np.zeros(21, dtype=np.complex_)
     omega = np.zeros(order+2, dtype=np.complex_)
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
     L = np.abs(z2-z1)
-    bigz = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2 * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     biga = np.abs(lab)
     ang = np.arctan2(lab.imag, lab.real)
     angz = np.arctan2((z2-z1).imag, (z2-z1).real)
     biglab = 2 * biga / L
     biglabcomplex = 2.0 * lab / L
 
     tol = 1e-12
 
-    exprange = np.exp(-np.complex(0, 2) * ang * nrange)
+    exprange = np.exp(-complex(0, 2) * ang * nrange)
     anew = a1 * exprange
-    bnew = (b1 - a1 * np.complex(0, 2) * ang) * exprange
+    bnew = (b1 - a1 * complex(0, 2) * ang) * exprange
     azero = anew[0]
 
     for n in range(20):
         bnew[n] = (n+1)*bnew[n+1] + anew[n+1]
         anew[n] = (n+1)*anew[n+1]
 
     anew[20] = 0  # This is a bit lazy
     bnew[20] = 0
 
-    zeta = (2 * np.complex(x, y) - (z1+z2)) / (z2-z1) / biglab
+    zeta = (2 * complex(x, y) - (z1+z2)) / (z2-z1) / biglab
     zetabar = np.conj(zeta)
     zminzbar[20] = 1
     for n in range(1, 21):
         # Ordered from high power to low power
         zminzbar[20-n] = zminzbar[21-n] * (zeta-zetabar)
 
     gamnew = np.zeros((21, 21), dtype=np.complex_)
@@ -1990,17 +1990,17 @@
         alpha2[n:2*n+1] = alpha2[n:2*n+1] + anew[n] * gam2[n, 0:n+1]
 
     d1minzeta = d1/biglab - zeta
     d2minzeta = d2/biglab - zeta
     # d1minzeta = -1/biglab - zeta
     # d2minzeta = 1/biglab - zeta
     if (np.abs(d1minzeta) < tol):
-        d1minzeta = d1minzeta + np.complex(tol, 0)
+        d1minzeta = d1minzeta + complex(tol, 0)
     if (np.abs(d2minzeta) < tol):
-        d2minzeta = d2minzeta + np.complex(tol, 0)
+        d2minzeta = d2minzeta + complex(tol, 0)
 
     log1 = np.log(d1minzeta)
     log2 = np.log(d2minzeta)
 
     alphanew = np.zeros(52, dtype=np.complex_)
     alphanew2 = np.zeros(52, dtype=np.complex_)
     betanew = np.zeros(52, dtype=np.complex_)
@@ -2029,40 +2029,40 @@
                                    alphanew[n] / (n+1) + betanew[n]) * term1 / (n+1)
             omega[p] = omega[p] + (alphanew2[n] * np.conj(log2) -
                                    alphanew2[n] / (n+1)) * np.conj(term2) / (n+1)
             omega[p] = omega[p] - (alphanew2[n] * np.conj(log1) -
                                    alphanew2[n] / (n+1)) * np.conj(term1) / (n+1)
 
     omegalap = lapld_int_ho_d1d2(
-        x, y, z1, z2, order, d1, d2) / np.complex(0, 1)
+        x, y, z1, z2, order, d1, d2) / complex(0, 1)
     omegaom = besselldpart(x, y, z1, z2, lab, order, d1, d2)
     wdis = lapld_int_ho_wdis_d1d2(x, y, z1, z2, order, d1, d2)
 
     rvz = -biglab * bigy / (2*np.pi*biglabcomplex**2) * (omega[1:order+1+1]/biglab - zetabar * omega[0:order+1]) + \
-        biglab * omegaom / np.complex(0, 2)
+        biglab * omegaom / complex(0, 2)
     rvzbar = -biglab * bigy / (2*np.pi*biglabcomplex**2) * (omega[1:order+1+1]/biglab - zeta * omega[0:order+1]) - \
-        biglab * omegaom / np.complex(0, 2)
+        biglab * omegaom / complex(0, 2)
     # qxqy[0:order+1] = -2.0 / L * ( rvz + rvzbar ) / biglab  # As we need to take derivative w.r.t. z not zeta
-    # qxqy[order+1:2*order+1+1] = -2.0 / L * np.complex(0,1) * (rvz-rvzbar) / biglab
+    # qxqy[order+1:2*order+1+1] = -2.0 / L * complex(0,1) * (rvz-rvzbar) / biglab
     #
     # qxqy[0:order+1] = qxqy[0:order+1] - 2.0 / L / biglabcomplex**2 * azero * ( omegalap + np.conj(omegalap) )
     # qxqy[order+1:2*order+1+1] = qxqy[order+1:2*order+1+1] -  \
-    #                          2.0 / L / biglabcomplex**2 * azero * np.complex(0,1) * (omegalap - np.conj(omegalap))
+    #                          2.0 / L / biglabcomplex**2 * azero * complex(0,1) * (omegalap - np.conj(omegalap))
     #
     # qxqy[0:order+1] = qxqy[0:order+1] + real(wdis)
     # qxqy[order+1:2*order+1+1] = qxqy[order+1:2*order+1+1] - aimag(wdis)
 
     # As we need to take derivative w.r.t. z not zeta
     qx = -2.0 / L * (rvz + rvzbar) / biglab
-    qy = -2.0 / L * np.complex(0, 1) * (rvz-rvzbar) / biglab
+    qy = -2.0 / L * complex(0, 1) * (rvz-rvzbar) / biglab
 
     qx = qx - 2.0 / L * bigy / biglabcomplex**2 * \
         azero * (omegalap + np.conj(omegalap))
     qy = qy - 2.0 / L * bigy / biglabcomplex**2 * azero * \
-        np.complex(0, 1) * (omegalap - np.conj(omegalap))
+        complex(0, 1) * (omegalap - np.conj(omegalap))
 
     # qx = qx + real(wdis * (z2-z1) / L)
     # qy = qy - aimag(wdis * (z2-z1) / L)
 
     # print *,'angz ',angz
     # wdis already includes the correct rotation
     qxqy[0:order+1] = qx * np.cos(angz) - qy * np.sin(angz) + wdis.real
@@ -2093,15 +2093,15 @@
     r = np.zeros(8, dtype=np.float_)
     k0 = np.zeros(8, dtype=np.complex_)
     k1 = np.zeros(8, dtype=np.complex_)
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
     L = np.abs(z2-z1)
     biglab = 2. * lab / L
-    bigz = (2. * np.complex(x, y) - (z1+z2)) / (z2-z1)
+    bigz = (2. * complex(x, y) - (z1+z2)) / (z2-z1)
     bigy = bigz.imag
     for n in range(8):
         xmind[n] = bigz.real - xg[n]
         r[n] = np.sqrt(xmind[n]**2 + bigz.imag**2)
         k0[n] = besselk0(xmind[n], bigz.imag, biglab)
         k1[n] = besselk1(xmind[n], bigz.imag, biglab)
 
@@ -2139,16 +2139,16 @@
     integer :: n, m
     real(kind=8) :: xp, yp, dc, fac
     complex(kind=8) :: z1p,z2p,bigz1,bigz2
     """
 
     qxqy = np.zeros(2*order+2, dtype=np.complex_)
 
-    bigz1 = np.complex(d1, 0)
-    bigz2 = np.complex(d2, 0)
+    bigz1 = complex(d1, 0)
+    bigz2 = complex(d2, 0)
     z1p = 0.5 * (z2-z1) * bigz1 + 0.5 * (z1+z2)
     z2p = 0.5 * (z2-z1) * bigz2 + 0.5 * (z1+z2)
     qxqyc = besselld_gauss_ho_qxqy(x, y, z1p, z2p, lab, order)
     dc = (d1+d2) / (d2-d1)
     for n in range(order+1):
         for m in range(n+1):
             qxqy[n] = qxqy[n] + gam[n, m] * dc**(n-m) * qxqyc[m]
@@ -2173,16 +2173,16 @@
 
     integer :: Nls, n
     real(kind=8) :: Lnear, L, d1, d2, delta
     complex(kind=8) :: z, delz, za, zb
 
     """
     Lnear = 3
-    z = np.complex(x, y)
-    qxqy = np.complex(0, 0)
+    z = complex(x, y)
+    qxqy = complex(0, 0)
     L = np.abs(z2-z1)
 
     # print *,'Lnear*np.abs(lab) ',Lnear*np.abs(lab)
     if (L < Lnear*np.abs(lab)):  # No need to break integral up
         if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
             qxqy = besselld_int_ho_qxqy(x, y, z1, z2, lab, order, d1in, d2in)
         else:
@@ -2228,15 +2228,15 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqylab
     """
 
     qxqy = np.zeros(2*nlab*(order+1), dtype=np.complex_)
 
     nterms = order+1
     nhalf = nlab*(order+1)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         qxqylab = besselldqxqy(x, y, z1, z2, lab[n], order, d1, d2)
         qxqy[n*nterms:(n+1)*nterms] = qxqylab[0:order+1]
         qxqy[n*nterms+nhalf:(n+1)*nterms +
              nhalf] = qxqylab[order+1:2*order+1+1]
 
     return qxqy
@@ -2256,15 +2256,15 @@
     complex(kind=8), dimension(0:2*order+1) :: qxqylab
     integer :: n, nterms, nhalf
     """
     qxqy = np.zeros((2*(order+1), nlab), dtype=np.complex_)
 
     nterms = order+1
     nhalf = nlab*(order+1)
-    d1, d2 = find_d1d2(z1, z2, np.complex(x, y), R*np.abs(lab[0]))
+    d1, d2 = find_d1d2(z1, z2, complex(x, y), R*np.abs(lab[0]))
     for n in range(nlab):
         qxqylab = besselldqxqy(x, y, z1, z2, lab[n], order, d1, d2)
         qxqy[:nterms, n] = qxqylab[0:order+1]
         qxqy[nterms:2*nterms, n] = qxqylab[order+1:2*order+1+1]
     return qxqy
 
 
@@ -2279,22 +2279,22 @@
 
     integer :: Npt, Nls, n
     real(kind=8) :: Lnear, Lzero, L, x1, y1, x2, y2
     complex(kind=8) :: z, z1, z2, delz, za, zb
     """
     Lnear = 3
     Lzero = 20
-    z = np.complex(x, y)
+    z = complex(x, y)
     x1, y1, x2, y2, Npt = circle_line_intersection(
         z1in, z2in, z, Lzero*np.abs(lab))
 
-    z1 = np.complex(x1, y1)
-    z2 = np.complex(x2, y2)
+    z1 = complex(x1, y1)
+    z2 = complex(x2, y2)
 
-    omega = np.complex(0, 0)
+    omega = complex(0, 0)
 
     if (Npt == 2):
         L = np.abs(z2-z1)
         if (L < Lnear*np.abs(lab)):  # No need to break integral up
             if (np.abs(z - 0.5*(z1+z2)) < 0.5 * Lnear * L):  # Do integration
                 omega = bessells_int(x, y, z1, z2, lab)
             else:
@@ -2343,16 +2343,16 @@
     real(kind=8), intent(in) :: R
     real(kind=8), intent(inout) :: xouta, youta, xoutb, youtb
     integer, intent(inout) :: N
     real(kind=8) :: Lover2, d, xa, xb
     complex(kind=8) :: bigz, za, zb
     """
     N = 0
-    za = np.complex(0, 0)
-    zb = np.complex(0, 0)
+    za = complex(0, 0)
+    zb = complex(0, 0)
 
     Lover2 = np.abs(z2-z1) / 2
     bigz = (2*zc - (z1+z2)) * Lover2 / (z2-z1)
 
     if (abs(bigz.imag) < R):
         d = np.sqrt(R**2 - bigz.imag**2)
         xa = bigz.real - d
```

### Comparing `ttim-0.6.4/ttim/circareasink.py` & `ttim-0.6.5/ttim/circareasink.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/circinhom.py` & `ttim-0.6.5/ttim/circinhom.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/element.py` & `ttim-0.6.5/ttim/element.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/equation.py` & `ttim-0.6.5/ttim/equation.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/fit.py` & `ttim-0.6.5/ttim/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,41 +31,41 @@
             parameter name, can include layer information. 
             name can be 'kaq', 'Saq' or 'c'. A number after the parameter 
             name denotes the layer number, i.e. 'kaq0' refers to the hydraulic 
             conductivity of layer 0. 
             name also supports layer ranges, entered by adding a '_' and a
             layer number, i.e. 'kaq0_3' denotes conductivity for layers 0 up to 
             and including 3.
-        initial : np.float, optional
+        initial : float, optional
             initial value for the parameter (the default is 0)
-        pmin : np.float, optional
+        pmin : float, optional
             lower bound for parameter value (the default is -np.inf)
-        pmax : np.float, optional
+        pmax : float, optional
             upper bound for paramater value (the default is np.inf)
         
         """
 
         assert type(name) == str, "Error: name must be string"
         # find numbers in name str for support layer ranges
         layers_from_name = re.findall(r'\d+', name)
         p = None
         if "_" in name:
-            fromlay, tolay = [np.int(i) for i in layers_from_name]
+            fromlay, tolay = [int(i) for i in layers_from_name]
             if name[:3] == 'kaq':
                 p = self.model.aq.kaq[fromlay:tolay+1]
             elif name[:3] == 'Saq':
                 p = self.model.aq.Saq[fromlay:tolay+1]
             elif name[0] == 'c':
                 p = self.model.aq.c[fromlay:tolay+1]
             elif name[:3] == 'Sll':
                 p = self.model.aq.Sll[fromlay:tolay+1]
             elif name[0:8] == 'kzoverkh':
                 p = self.model.aq.kzoverkh[fromlay:tolay+1]
         else:
-            layer = np.int(layers_from_name[0])
+            layer = int(layers_from_name[0])
             # Set, kaq, Saq, c
             if name[:3] == 'kaq':
                 p = self.model.aq.kaq[layer:layer + 1]
             elif name[:3] == 'Saq':
                 p = self.model.aq.Saq[layer:layer + 1]
             elif name[0] == 'c':
                 p = self.model.aq.c[layer:layer + 1]
@@ -87,19 +87,19 @@
         Parameters
         ----------
         name : str
             parameter name
         parameter : np.array
             array reference containing the parameter to be optimized. must be 
             specified as reference, i.e. w.rc[0:]  
-        initial : np.float, optional
+        initial : float, optional
             initial value for the parameter (the default is 0)
-        pmin : np.float, optional
+        pmin : float, optional
             lower bound for parameter value (the default is -np.inf)
-        pmax : np.float, optional
+        pmax : float, optional
             upper bound for paramater value (the default is np.inf)
         
         """
         assert type(name) == str, "Error: name must be string"
         if parameter is not None:
             assert isinstance(parameter, np.ndarray), \
                 "Error: parameter needs to be numpy array"
@@ -111,17 +111,17 @@
     def series(self, name, x, y, layer, t, h):
         """method to add observations to Calibration object
         
         Parameters
         ----------
         name : str
             name of series
-        x : np.float
+        x : float
             x-coordinate
-        y : np.float
+        y : float
             y-coordinate
         layer : int
             layer number, 0-indexed
         t : np.array
             array containing timestamps of timeseries
         h : np.array
             array containing timeseries values, i.e. head observations
@@ -256,15 +256,15 @@
         return self.fit_lmfit(report, printdot)
             
     def rmse(self):
         """calculate root-mean-squared-error
         
         Returns
         -------
-        np.float
+        float
             return rmse value
         """
 
         r = self.residuals(self.parameters['optimal'].values)
         return np.sqrt(np.mean(r ** 2))
     
 class Series:
```

### Comparing `ttim-0.6.4/ttim/invlapnumba.py` & `ttim-0.6.5/ttim/invlapnumba.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/kuhlman_invlap.py` & `ttim-0.6.5/ttim/kuhlman_invlap.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/linedoublet.py` & `ttim-0.6.5/ttim/linedoublet.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/linesink.py` & `ttim-0.6.5/ttim/linesink.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/model.py` & `ttim-0.6.5/ttim/model.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/trace.py` & `ttim-0.6.5/ttim/trace.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/util.py` & `ttim-0.6.5/ttim/util.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim/well.py` & `ttim-0.6.5/ttim/well.py`

 * *Files identical despite different names*

### Comparing `ttim-0.6.4/ttim.egg-info/PKG-INFO` & `ttim-0.6.5/ttim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttim
-Version: 0.6.4
+Version: 0.6.5
 Summary: Transient multi-layer AEM Model
 Home-page: https://github.com/mbakker7/ttim
 Author: Mark Bakker
 Author-email: markbak@gmail.com
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.7
```

### Comparing `ttim-0.6.4/ttim.egg-info/SOURCES.txt` & `ttim-0.6.5/ttim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

