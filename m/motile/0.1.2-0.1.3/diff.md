# Comparing `tmp/motile-0.1.2.tar.gz` & `tmp/motile-0.1.3.tar.gz`

## Comparing `motile-0.1.2.tar` & `motile-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 motile-0.1.2/Makefile
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 motile-0.1.2/.github/workflows/deploy.yaml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 motile-0.1.2/motile/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 motile-0.1.2/motile/solver.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 motile-0.1.2/motile/track_graph.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 motile-0.1.2/motile/utils.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 motile-0.1.2/motile/constraints/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 motile-0.1.2/motile/constraints/constraint.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 motile-0.1.2/motile/constraints/max_children.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 motile-0.1.2/motile/constraints/max_parents.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 motile-0.1.2/motile/constraints/pin.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 motile-0.1.2/motile/constraints/select_edge_nodes.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/appear.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/costs.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/edge_distance.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/edge_selection.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/node_selection.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 motile-0.1.2/motile/costs/split.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 motile-0.1.2/motile/variables/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 motile-0.1.2/motile/variables/edge_selected.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 motile-0.1.2/motile/variables/node_appear.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 motile-0.1.2/motile/variables/node_selected.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 motile-0.1.2/motile/variables/node_split.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 motile-0.1.2/motile/variables/variable.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 motile-0.1.2/tests/data.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 motile-0.1.2/tests/test_api.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 motile-0.1.2/tests/test_constraints.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 motile-0.1.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 motile-0.1.2/LICENSE
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 motile-0.1.2/README.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 motile-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 motile-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 motile-0.1.3/Makefile
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 motile-0.1.3/.github/workflows/deploy.yaml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 motile-0.1.3/motile/__init__.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 motile-0.1.3/motile/solver.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 motile-0.1.3/motile/track_graph.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 motile-0.1.3/motile/utils.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 motile-0.1.3/motile/constraints/__init__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 motile-0.1.3/motile/constraints/constraint.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 motile-0.1.3/motile/constraints/max_children.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 motile-0.1.3/motile/constraints/max_parents.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 motile-0.1.3/motile/constraints/pin.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 motile-0.1.3/motile/constraints/select_edge_nodes.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/appear.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/costs.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/edge_distance.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/edge_selection.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/node_selection.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 motile-0.1.3/motile/costs/split.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 motile-0.1.3/motile/variables/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 motile-0.1.3/motile/variables/edge_selected.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 motile-0.1.3/motile/variables/node_appear.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 motile-0.1.3/motile/variables/node_selected.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 motile-0.1.3/motile/variables/node_split.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 motile-0.1.3/motile/variables/variable.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 motile-0.1.3/tests/data.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 motile-0.1.3/tests/test_api.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 motile-0.1.3/tests/test_constraints.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 motile-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 motile-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 motile-0.1.3/README.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 motile-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 motile-0.1.3/PKG-INFO
```

### Comparing `motile-0.1.2/.github/workflows/deploy.yaml` & `motile-0.1.3/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/solver.py` & `motile-0.1.3/motile/solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,16 +96,22 @@
         self.ilp_solver.set_objective(self.objective)
         self.ilp_solver.set_constraints(self.constraints)
 
         self.ilp_solver.set_num_threads(num_threads)
         if timeout > 0:
             self.ilp_solver.set_timeout(self.timeout)
 
-        self.solution, message = self.ilp_solver.solve()
-        if len(message):
+        solution = self.ilp_solver.solve()
+        if hasattr(solution, "get_status"):
+            # ilpy version >= 0.3.0
+            self.solution, message = solution, solution.get_status()
+        else:
+            self.solution, message = solution
+
+        if message:
             logger.info("ILP solver returned with: %s", message)
 
         return self.solution
 
     def get_variables(self, cls):
         """Get variables by their class name.
```

### Comparing `motile-0.1.2/motile/track_graph.py` & `motile-0.1.3/motile/track_graph.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/utils.py` & `motile-0.1.3/motile/utils.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/constraints/max_children.py` & `motile-0.1.3/motile/constraints/max_children.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/constraints/max_parents.py` & `motile-0.1.3/motile/constraints/max_parents.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/constraints/pin.py` & `motile-0.1.3/motile/constraints/pin.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/constraints/select_edge_nodes.py` & `motile-0.1.3/motile/constraints/select_edge_nodes.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/costs/appear.py` & `motile-0.1.3/motile/costs/appear.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/costs/edge_distance.py` & `motile-0.1.3/motile/costs/edge_distance.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/costs/edge_selection.py` & `motile-0.1.3/motile/costs/edge_selection.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/costs/node_selection.py` & `motile-0.1.3/motile/costs/node_selection.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/costs/split.py` & `motile-0.1.3/motile/costs/split.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/variables/node_appear.py` & `motile-0.1.3/motile/variables/node_appear.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/variables/node_split.py` & `motile-0.1.3/motile/variables/node_split.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/motile/variables/variable.py` & `motile-0.1.3/motile/variables/variable.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/tests/data.py` & `motile-0.1.3/tests/data.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/tests/test_api.py` & `motile-0.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/tests/test_constraints.py` & `motile-0.1.3/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/LICENSE` & `motile-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/README.md` & `motile-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/pyproject.toml` & `motile-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `motile-0.1.2/PKG-INFO` & `motile-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motile
-Version: 0.1.2
+Version: 0.1.3
 Summary: Multi-Object Tracker using Integer Linear Equations
 Project-URL: homepage, https://github.com/funkelab/motile
 Author-email: Jan Funke <funkej@janelia.hhmi.org>, Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Dist: ilpy
 Requires-Dist: networkx
```

