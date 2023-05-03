# Comparing `tmp/riccati-1.0.7.tar.gz` & `tmp/riccati-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riccati-1.0.7.tar", last modified: Thu Feb 23 15:41:45 2023, max compression
+gzip compressed data, was "riccati-1.0.8.tar", last modified: Mon Mar 20 19:00:34 2023, max compression
```

## Comparing `riccati-1.0.7.tar` & `riccati-1.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.084734 riccati-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 15:41:34.000000 riccati-1.0.7/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 15:41:34.000000 riccati-1.0.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.080734 riccati-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.080734 riccati-1.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-23 15:41:34.000000 riccati-1.0.7/.github/ISSUE_TEMPLATE/issue-name.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-23 15:41:34.000000 riccati-1.0.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.080734 riccati-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-02-23 15:41:34.000000 riccati-1.0.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-23 15:41:34.000000 riccati-1.0.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-23 15:41:34.000000 riccati-1.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-23 15:41:34.000000 riccati-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-23 15:41:45.084734 riccati-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-02-23 15:41:34.000000 riccati-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.080734 riccati-1.0.7/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-23 15:41:34.000000 riccati-1.0.7/binder/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.080734 riccati-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1061269 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81767 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 15:41:34.000000 riccati-1.0.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-23 15:41:34.000000 riccati-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-23 15:41:34.000000 riccati-1.0.7/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 15:41:34.000000 riccati-1.0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.084734 riccati-1.0.7/riccati/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-23 15:41:45.084734 riccati-1.0.7/riccati/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/chebutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/evolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/solversetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/stepsize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.084734 riccati-1.0.7/riccati/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10478 2023-02-23 15:41:34.000000 riccati-1.0.7/riccati/tests/test_riccati.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:41:45.084734 riccati-1.0.7/riccati.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-23 15:41:45.000000 riccati-1.0.7/riccati.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-23 15:41:45.000000 riccati-1.0.7/riccati.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:41:45.000000 riccati-1.0.7/riccati.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-23 15:41:45.000000 riccati-1.0.7/riccati.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 15:41:45.000000 riccati-1.0.7/riccati.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 15:41:45.084734 riccati-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-23 15:41:34.000000 riccati-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 19:00:23.000000 riccati-1.0.8/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 19:00:23.000000 riccati-1.0.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.111193 riccati-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.111193 riccati-1.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-20 19:00:23.000000 riccati-1.0.8/.github/ISSUE_TEMPLATE/issue-name.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-20 19:00:23.000000 riccati-1.0.8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.115193 riccati-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-20 19:00:23.000000 riccati-1.0.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 19:00:23.000000 riccati-1.0.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-20 19:00:23.000000 riccati-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-20 19:00:23.000000 riccati-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-20 19:00:34.123193 riccati-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-20 19:00:23.000000 riccati-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.115193 riccati-1.0.8/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-20 19:00:23.000000 riccati-1.0.8/binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.119193 riccati-1.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1061269 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81767 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-20 19:00:23.000000 riccati-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-20 19:00:23.000000 riccati-1.0.8/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-20 19:00:23.000000 riccati-1.0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/chebutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/solversetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/stepsize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/tests/test_riccati.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:00:34.123193 riccati-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-20 19:00:23.000000 riccati-1.0.8/setup.py
```

### Comparing `riccati-1.0.7/.github/ISSUE_TEMPLATE/issue-name.md` & `riccati-1.0.8/.github/ISSUE_TEMPLATE/issue-name.md`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/.github/workflows/tests.yml` & `riccati-1.0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/CONTRIBUTING.md` & `riccati-1.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/LICENSE` & `riccati-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/PKG-INFO` & `riccati-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riccati
-Version: 1.0.7
+Version: 1.0.8
 Summary: adaptive Riccati defect correction solver
 Home-page: 
 Author: Fruzsina J Agocs and Alex H Barnett
 Author-email: 
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `riccati-1.0.7/README.md` & `riccati-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/docs/Makefile` & `riccati-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/docs/api.rst` & `riccati-1.0.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/docs/conf.py` & `riccati-1.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/docs/examples.ipynb` & `riccati-1.0.8/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/docs/index.rst` & `riccati-1.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/docs/quickstart.ipynb` & `riccati-1.0.8/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/riccati/__init__.py` & `riccati-1.0.8/riccati/__init__.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/riccati/chebutils.py` & `riccati-1.0.8/riccati/chebutils.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/riccati/evolve.py` & `riccati-1.0.8/riccati/evolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,18 @@
         info.y = np.array([y10, y11])
         info.x = x0 + h
         # Determine new stepsize
         wnext = info.wn[0]
         gnext = info.gn[0]
         dwnext = 2/h*(info.Dn @ info.wn)[0]
         dgnext = 2/h*(info.Dn @ info.gn)[0]
-        hosc_ini = min(1e8, np.abs(wnext/dwnext), np.abs(gnext/dgnext))
+        hosc_ini = sign*min(1e8, np.abs(wnext/dwnext), np.abs(gnext/dgnext))
+        # Check if estimate for next stepsize would be out of range
+        if sign*(info.x + hosc_ini) > sign*x1:
+            hosc_ini = x1 - info.x
         info.h = choose_osc_stepsize(info, info.x, hosc_ini, epsh = epsh)  
     return success
 
 def nonosc_evolve(info, x0, x1, h, y0, epsres = 1e-12, epsh = 0.2):
     """
     Allows continuous evolution between the independent variable values `x0`
     and `x1`. Starting from `x0` and `y = [y0, yd0]` takes a Chebyshev step of
@@ -142,16 +145,19 @@
     else:
         # Successful step
         success = 1
         info.y = np.array([y10, y11])
         info.x += h
         # Determine new stepsize
         wnext = info.w(info.x)
-        hosc_ini = min(1e8, np.abs(1/wnext))
-        info.h = choose_nonosc_stepsize(info, info.x, hosc_ini, epsh = epsh)  
+        hslo_ini = sign*min(1e8, np.abs(1/wnext))
+        # Check if estimate for next stepsize would be out of range
+        if sign*(info.x + hslo_ini) > sign*x1:
+            hslo_ini = x1 - info.x
+        info.h = choose_nonosc_stepsize(info, info.x, hslo_ini, epsh = epsh)  
     return success
 
 def solve(info, xi, xf, yi, dyi, eps = 1e-12, epsh = 1e-12, xeval = np.array([]), hard_stop = False):
     """
     Solves y'' + 2gy' + w^2y = 0 on the interval (xi, xf), starting from the
     initial conditions y(xi) = yi, y'(xi) = dyi. Keeps the residual of the ODE
     below eps, and returns an interpolated solution (dense output) at points
```

### Comparing `riccati-1.0.7/riccati/solversetup.py` & `riccati-1.0.8/riccati/solversetup.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/riccati/step.py` & `riccati-1.0.8/riccati/step.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/riccati/stepsize.py` & `riccati-1.0.8/riccati/stepsize.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/riccati/tests/test_riccati.py` & `riccati-1.0.8/riccati/tests/test_riccati.py`

 * *Files 18% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     dyi = -sp.airy(-xi)[1] - 1j*sp.airy(-xi)[3]
     xs, ys, dys, ss, ps, stypes = solve(info, xi, xf, yi, dyi, eps = eps, epsh = epsh)
     xs = np.array(xs)
     ys = np.array(ys)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
     yerr = np.abs((ytrue - ys)/ytrue)
     maxerr = max(yerr)
-    print(maxerr, stypes)
+    print(maxerr)
     assert maxerr < 1e-6
 
 def test_solve_airy_backwards():
     w = lambda x: np.sqrt(x)
     g = lambda x: np.zeros_like(x)
     info = solversetup(w, g, n = 32, p = 32)
     xi = 1e6
@@ -191,15 +191,15 @@
     xs, ys, dys, ss, ps, stypes, yeval = solve(info, xi, xf, yi, dyi,\
                                                        xeval = xeval,\
                                                        eps = eps, epsh = epsh,\
                                                        hard_stop = True)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xeval])
     yerr = np.abs((ytrue - yeval)/ytrue)
     maxerr = max(yerr)
-    print(yeval, yerr, maxerr)
+    print(maxerr)
     assert maxerr < 1e-6
 
 def test_denseoutput_backwards_xback():
     w = lambda x: np.sqrt(x)
     g = lambda x: np.zeros_like(x)
     info = solversetup(w, g, n = 32, p = 32)
     xi = 1e6
@@ -213,15 +213,15 @@
     xs, ys, dys, ss, ps, stypes, yeval = solve(info, xi, xf, yi, dyi,\
                                                        xeval = xeval,\
                                                        eps = eps, epsh = epsh,\
                                                        hard_stop = True)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xeval])
     yerr = np.abs((ytrue - yeval)/ytrue)
     maxerr = max(yerr)
-    print(yeval, yerr, maxerr)
+    print(maxerr)
     assert maxerr < 1e-6
 
 def test_solve_burst():
     m = int(1e6) # Frequency parameter
     w = lambda x: np.sqrt(m**2 - 1)/(1 + x**2)
     g = lambda x: np.zeros_like(x)
     bursty = lambda x: np.sqrt(1 + x**2)/m*(np.cos(m*np.arctan(x)) + 1j*np.sin(m*np.arctan(x))) 
@@ -269,14 +269,15 @@
         xs.append(info.x)
         ys.append(info.y[0])
     xs = np.array(xs)
     ys = np.array(ys)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
     yerr = np.abs((ytrue - ys)/ytrue)
     maxerr = max(yerr)
+    print("Forward osc evolve max error:", maxerr)
     assert maxerr < 1e-6
    
 def test_nonosc_evolve():
     w = lambda x: np.sqrt(x)
     g = lambda x: np.zeros_like(x)
     info = solversetup(w, g, n = 32, p = 32)
     xi = 1e0
@@ -302,9 +303,78 @@
         xs.append(info.x)
         ys.append(info.y[0])
     xs = np.array(xs)
     ys = np.array(ys)
     ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
     yerr = np.abs((ytrue - ys)/ytrue)
     maxerr = max(yerr)
+    print("Forward nonosc evolve max error:", maxerr)
+    assert maxerr < 1e-10
+
+def test_osc_evolve_backwards():
+    w = lambda x: np.sqrt(x)
+    g = lambda x: np.zeros_like(x)
+    info = solversetup(w, g, n = 32, p = 32)
+    xi = 1e6
+    xf = 1e2
+    eps = 1e-12
+    epsh = 1e-13
+    yi = sp.airy(-xi)[0] + 1j*sp.airy(-xi)[2]
+    dyi = -sp.airy(-xi)[1] - 1j*sp.airy(-xi)[3]
+    # Store things
+    xs, ys, dys = [], [], []
+    # Always necessary for setting info.y
+    info.y = np.array([yi, dyi])
+    # Always necessary for setting info.wn, info.gn, and for getting an initial stepsize
+    hi = -xi/10
+    hi = choose_osc_stepsize(info, xi, hi, epsh = epsh)
+    info.h = hi
+    # Not necessary here because info.x is already xi, but in general it might be:
+    info.x = xi
+    while info.x > xf:
+        status = osc_evolve(info, info.x, xf, info.h, info.y, epsres = eps, epsh = epsh)
+        if status != 1:
+            break
+        xs.append(info.x)
+        ys.append(info.y[0])
+    xs = np.array(xs)
+    ys = np.array(ys)
+    ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
+    yerr = np.abs((ytrue - ys)/ytrue)
+    maxerr = max(yerr)
+    print("Backwards osc evolve max error:", maxerr)
+    assert maxerr < 1e-6
+   
+def test_nonosc_evolve_backwards():
+    w = lambda x: np.sqrt(x)
+    g = lambda x: np.zeros_like(x)
+    info = solversetup(w, g, n = 32, p = 32)
+    xi = 4e1
+    xf = 1e0
+    eps = 1e-12
+    epsh = 2e-1 # Note different definition of epsh for Chebyshev steps!
+    yi = sp.airy(-xi)[0] + 1j*sp.airy(-xi)[2]
+    dyi = -sp.airy(-xi)[1] - 1j*sp.airy(-xi)[3]
+    # Store things
+    xs, ys, dys = [], [], []
+    # Always necessary for setting info.y
+    info.y = np.array([yi, dyi])
+    # Necessary for getting an initial stepsize
+    hi = -1/w(xi)
+    hi = choose_nonosc_stepsize(info, xi, hi, epsh = epsh)
+    info.h = hi
+    # Not necessary here because info.x is already xi, but in general it might be:
+    info.x = xi
+    while info.x > xf:
+        status = nonosc_evolve(info, info.x, xf, info.h, info.y, epsres = eps, epsh = epsh)
+        if status != 1:
+            break
+        xs.append(info.x)
+        ys.append(info.y[0])
+    xs = np.array(xs)
+    ys = np.array(ys)
+    ytrue = np.array([mpmath.airyai(-x) + 1j*mpmath.airybi(-x) for x in xs])
+    yerr = np.abs((ytrue - ys)/ytrue)
+    maxerr = max(yerr)
+    print("Backward nonosc evolve max error:", maxerr)
     assert maxerr < 1e-10
```

### Comparing `riccati-1.0.7/riccati.egg-info/PKG-INFO` & `riccati-1.0.8/riccati.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riccati
-Version: 1.0.7
+Version: 1.0.8
 Summary: adaptive Riccati defect correction solver
 Home-page: 
 Author: Fruzsina J Agocs and Alex H Barnett
 Author-email: 
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
```

### Comparing `riccati-1.0.7/riccati.egg-info/SOURCES.txt` & `riccati-1.0.8/riccati.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riccati-1.0.7/setup.py` & `riccati-1.0.8/setup.py`

 * *Files identical despite different names*

