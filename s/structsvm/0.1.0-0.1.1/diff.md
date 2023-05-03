# Comparing `tmp/structsvm-0.1.0.tar.gz` & `tmp/structsvm-0.1.1.tar.gz`

## Comparing `structsvm-0.1.0.tar` & `structsvm-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 structsvm-0.1.0/Makefile
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 structsvm-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 structsvm-0.1.0/.github/workflows/deploy.yaml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 structsvm-0.1.0/structsvm/__init__.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 structsvm-0.1.0/structsvm/bundle_method.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 structsvm-0.1.0/structsvm/hamming_costs.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 structsvm-0.1.0/structsvm/linear_costs.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 structsvm-0.1.0/structsvm/soft_margin_loss.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 structsvm-0.1.0/tests/test_bundle_method.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 structsvm-0.1.0/tests/test_ssvm.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 structsvm-0.1.0/.gitignore
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 structsvm-0.1.0/README.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 structsvm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 structsvm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 structsvm-0.1.1/Makefile
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 structsvm-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 structsvm-0.1.1/.github/workflows/deploy.yaml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 structsvm-0.1.1/structsvm/__init__.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 structsvm-0.1.1/structsvm/bundle_method.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 structsvm-0.1.1/structsvm/hamming_costs.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 structsvm-0.1.1/structsvm/linear_costs.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 structsvm-0.1.1/structsvm/soft_margin_loss.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 structsvm-0.1.1/tests/test_bundle_method.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 structsvm-0.1.1/tests/test_ssvm.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 structsvm-0.1.1/.gitignore
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 structsvm-0.1.1/README.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 structsvm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 structsvm-0.1.1/PKG-INFO
```

### Comparing `structsvm-0.1.0/.github/workflows/ci.yml` & `structsvm-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `structsvm-0.1.0/.github/workflows/deploy.yaml` & `structsvm-0.1.1/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `structsvm-0.1.0/structsvm/bundle_method.py` & `structsvm-0.1.1/structsvm/bundle_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import numpy as np
 import ilpy
 
 logger = logging.getLogger(__name__)
+ILPY_V02 = ilpy.__version__.split(".")[:2] < ["0", "3"]
 
 
 class BundleMethod:
     '''Create a new bundle method for the given value and gradient callback.
 
     Args:
 
@@ -170,14 +171,14 @@
         constraint.set_value(-b)
 
         self._solver.add_constraint(constraint)
 
     def _find_min_lower_bound(self):
 
         # solve the QP
-        solution, _ = self._solver.solve()
+        solution = self._solver.solve()[0] if ILPY_V02 else self._solver.solve()
 
         # read the solution
         w = np.array([solution[i] for i in range(self._dims)])
         value = solution.get_value()
 
         return w, value
```

### Comparing `structsvm-0.1.0/structsvm/hamming_costs.py` & `structsvm-0.1.1/structsvm/hamming_costs.py`

 * *Files identical despite different names*

### Comparing `structsvm-0.1.0/structsvm/soft_margin_loss.py` & `structsvm-0.1.1/structsvm/soft_margin_loss.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import numpy as np
 import ilpy
 from .hamming_costs import HammingCosts
 
 logger = logging.getLogger(__name__)
-
+ILPY_V02 = ilpy.__version__.split(".")[:2] < ["0", "3"]
 
 class SoftMarginLoss:
     '''Implements the soft margin loss, i.e.,
 
        L(w) = max_y <w,φ(x')y' - φ(x')y> + Δ(y',y)
 
     for a ground truth y', features φ(x'), and a linear cost function Δ(y', y).
@@ -92,15 +92,16 @@
         for i in range(self._num_variables):
             self._objective.set_coefficient(i, self._g[i] - f[i])
 
         logger.debug("objective is %s", self._objective)
 
         # solve
         self._solver.set_objective(self._objective)
-        solution, _ = self._solver.solve()
+        # solve the QP
+        solution = self._solver.solve()[0] if ILPY_V02 else self._solver.solve()
 
         # read optimal value L(w)
         value = solution.get_value()
 
         # ∂L(w)/∂w = φ(x')y' - φ(x')y*
         #          = d       - e
```

### Comparing `structsvm-0.1.0/tests/test_ssvm.py` & `structsvm-0.1.1/tests/test_ssvm.py`

 * *Files identical despite different names*

### Comparing `structsvm-0.1.0/README.md` & `structsvm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `structsvm-0.1.0/pyproject.toml` & `structsvm-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `structsvm-0.1.0/PKG-INFO` & `structsvm-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structsvm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Structured Bundle Method for Risk Minimization.
 Project-URL: homepage, https://github.com/funkelab/structsvm
 Project-URL: repository, https://github.com/funkelab/structsvm
 Author-email: Jan Funke <funkej@janelia.hhmi.org>, Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: ilpy
```

