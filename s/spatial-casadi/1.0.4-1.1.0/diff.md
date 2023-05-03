# Comparing `tmp/spatial_casadi-1.0.4.tar.gz` & `tmp/spatial_casadi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_casadi-1.0.4.tar", last modified: Mon Apr 10 12:13:47 2023, max compression
+gzip compressed data, was "spatial_casadi-1.1.0.tar", last modified: Wed May  3 20:26:34 2023, max compression
```

## Comparing `spatial_casadi-1.0.4.tar` & `spatial_casadi-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     7650 2023-03-12 23:07:25.000000 spatial_casadi-1.0.4/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     4708 2023-03-26 19:51:34.000000 spatial_casadi-1.0.4/README.md
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      785 2023-04-10 12:12:34.000000 spatial_casadi-1.0.4/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      920 2023-04-10 12:12:39.000000 spatial_casadi-1.0.4/setup.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/spatial_casadi/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       77 2023-03-26 20:00:43.000000 spatial_casadi-1.0.4/spatial_casadi/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    23420 2023-04-10 12:11:04.000000 spatial_casadi-1.0.4/spatial_casadi/spatial.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/spatial_casadi.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      377 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       34 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       15 2023-04-10 12:13:47.000000 spatial_casadi-1.0.4/spatial_casadi.egg-info/top_level.txt
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-04-10 12:13:47.974830 spatial_casadi-1.0.4/test/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     6732 2023-04-04 12:31:15.000000 spatial_casadi-1.0.4/test/test_rotation.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1316 2023-03-13 19:43:36.000000 spatial_casadi-1.0.4/test/test_transformation.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1903 2023-03-13 19:43:40.000000 spatial_casadi-1.0.4/test/test_translation.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      597 2023-03-13 19:43:43.000000 spatial_casadi-1.0.4/test/test_utils.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-03 20:26:34.884353 spatial_casadi-1.1.0/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     7650 2023-03-12 23:07:25.000000 spatial_casadi-1.1.0/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-05-03 20:26:34.884353 spatial_casadi-1.1.0/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     4708 2023-03-26 19:51:34.000000 spatial_casadi-1.1.0/README.md
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      785 2023-05-03 20:24:43.000000 spatial_casadi-1.1.0/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-05-03 20:26:34.884353 spatial_casadi-1.1.0/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      920 2023-05-03 20:24:28.000000 spatial_casadi-1.1.0/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-03 20:26:34.884353 spatial_casadi-1.1.0/spatial_casadi/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       77 2023-03-26 20:00:43.000000 spatial_casadi-1.1.0/spatial_casadi/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    23851 2023-05-03 20:23:13.000000 spatial_casadi-1.1.0/spatial_casadi/spatial.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-03 20:26:34.884353 spatial_casadi-1.1.0/spatial_casadi.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5566 2023-05-03 20:26:34.000000 spatial_casadi-1.1.0/spatial_casadi.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      377 2023-05-03 20:26:34.000000 spatial_casadi-1.1.0/spatial_casadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-05-03 20:26:34.000000 spatial_casadi-1.1.0/spatial_casadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       34 2023-05-03 20:26:34.000000 spatial_casadi-1.1.0/spatial_casadi.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       15 2023-05-03 20:26:34.000000 spatial_casadi-1.1.0/spatial_casadi.egg-info/top_level.txt
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-05-03 20:26:34.884353 spatial_casadi-1.1.0/test/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     6711 2023-05-03 20:23:13.000000 spatial_casadi-1.1.0/test/test_rotation.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1316 2023-03-13 19:43:36.000000 spatial_casadi-1.1.0/test/test_transformation.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1903 2023-03-13 19:43:40.000000 spatial_casadi-1.1.0/test/test_translation.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      597 2023-03-13 19:43:43.000000 spatial_casadi-1.1.0/test/test_utils.py
```

### Comparing `spatial_casadi-1.0.4/LICENSE` & `spatial_casadi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.4/PKG-INFO` & `spatial_casadi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial_casadi
-Version: 1.0.4
+Version: 1.1.0
 Summary: Spatial transformation library for CasADi Python. 
 Home-page: https://github.com/cmower/spatial-casadi
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://cmower.github.io/spatial-casadi/
 Project-URL: Documentation, https://cmower.github.io/spatial-casadi/
```

### Comparing `spatial_casadi-1.0.4/README.md` & `spatial_casadi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.4/pyproject.toml` & `spatial_casadi-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spatial_casadi"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = "Spatial transformation library for CasADi Python. "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spatial_casadi-1.0.4/setup.py` & `spatial_casadi-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="spatial-casadi",
     description="Spatial transformation library for CasADi Python.",
-    version="1.0.4",
+    version="1.1.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmower/spatial-casadi",
     project_urls={
         "Homepage": "https://cmower.github.io/spatial-casadi/",
         "Documentation": "https://cmower.github.io/spatial-casadi/",
         "Bug Tracker": "https://github.com/cmower/spatial-casadi/issues",
```

### Comparing `spatial_casadi-1.0.4/spatial_casadi/spatial.py` & `spatial_casadi-1.1.0/spatial_casadi/spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,19 @@
 
 @return Random rotation.
         """
         return Rotation(casadi.np.random.normal(size=(4,)))
 
     @staticmethod
     def symbolic():
-        """! Symbolic representation."""
-        quat = cs.SX.sym("quat", 4)
+        """! Symbolic representation.
+
+@return Symbolic rotation.
+        """
+        quat = casadi.SX.sym("quat", 4)
         return Rotation(quat, normalize=False)
 
     def inv(self):
         """! Invert this rotation."""
         return Rotation(
             casadi.vertcat(self._quat[:-1], -self._quat[-1]),
             normalize=not isinstance(self._quat, casadi.SX),
@@ -384,22 +387,21 @@
 
     def as_rotvec(self, degrees: bool = False) -> ArrayType:
         """! Represent as rotation vector.
 
 @param degrees If True, then the given magnitudes are assumed to be in degrees. Default is False.
 @return A 3-dimensional rotation vector
         """
+
+        # w > 0 to ensure 0 <= angle <= pi
         quat = casadi.if_else(self._quat[3] < 0, -self._quat, self._quat)
-        angle = 2.0 * casadi.arctan2(casadi.norm_fro(quat), quat[3])
-        # angle2 = angle * angle
-        scale = casadi.if_else(
-            angle <= 1e-3,
-            2.0 + angle**2 / 12.0 + 7.0 * angle**2 * angle**2 / 2880.0,
-            angle / casadi.sin(angle * 0.5),
-        )
+
+        # Use formula: https://uk.mathworks.com/help/fusion/ref/quaternion.rotvec.html
+        theta = 2.0 * casadi.acos(quat[3])
+        scale = theta / casadi.sin(theta * 0.5)
 
         rotvec = casadi.vertcat(
             scale * quat[0],
             scale * quat[1],
             scale * quat[2],
         )
 
@@ -584,16 +586,19 @@
 
 @return Random translation.
         """
         return Translation(casadi.np.random.normal(size=(3,)))
 
     @staticmethod
     def symbolic():
-        """! Symbolic representation."""
-        t = cs.SX.sym("t", 3)
+        """! Symbolic representation.
+
+@return Symbolic translation.
+        """
+        t = casadi.SX.sym("t", 3)
         return Translation(t)
 
     @staticmethod
     def from_vector(t):
         """! Initialize from translation vector.
 
 @param t A 3-dimensional translation vector.
@@ -680,15 +685,18 @@
 
 @return Random homogeneous transform.
         """
         return Transformation(Rotation.random(), Translation.random())
 
     @staticmethod
     def symbolic():
-        """! Symbolic representation."""
+        """! Symbolic representation.
+
+@return Symbolic homogenous transform.
+"""
         return Transformation(Rotation.symbolic(), Translation.symbolic())
 
     @staticmethod
     def from_matrix(T: ArrayType):
         """! Initialize from homogenous transformation matrix.
 
 @param matrix A 4-by-4 homogeneous transformation matrix.
@@ -715,7 +723,17 @@
 @param other Object containing the transformation to be composed with this one. Note that transformation compositions are not commutative, so p * q is different from q * p.
 @return The homgeonous transformation that is the product A * B.
         """
         # DEV NOTE: this computes the product self * other
         rotation = self._rotation * other.rotation()
         translation = self._rotation * other.translation() + self._translation
         return Transformation(rotation, translation)
+
+    def flatten(self):
+        """! Returns the homogenous transform as a vector representation [quat, t] where quat is a unit-quaternion for the rotation and t is the translation.
+
+@return Vector representation for the homogeneous transform.
+"""
+        return casadi.vertcat(
+            self._rotation.as_quat(),
+            self._translation.as_vector(),
+        )
```

### Comparing `spatial_casadi-1.0.4/spatial_casadi.egg-info/PKG-INFO` & `spatial_casadi-1.1.0/spatial_casadi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial-casadi
-Version: 1.0.4
+Version: 1.1.0
 Summary: Spatial transformation library for CasADi Python. 
 Home-page: https://github.com/cmower/spatial-casadi
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://cmower.github.io/spatial-casadi/
 Project-URL: Documentation, https://cmower.github.io/spatial-casadi/
```

### Comparing `spatial_casadi-1.0.4/test/test_rotation.py` & `spatial_casadi-1.1.0/test/test_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import casadi as cs
 from spatial_casadi import Rotation
 from scipy.spatial.transform import Rotation as Rot
 
+
 NUM_RANDOM = 100
 
 EULER_SEQS = (
     "xyz",
     "zyx",
     "xyx",
     "zyz",
@@ -215,15 +216,15 @@
         RV = R.as_rotvec()
         rv = r.as_rotvec().toarray().flatten()
 
         print("Test:", i + 1, "/", NUM_RANDOM)
         print("  Scipy:", RV)
         print("  Lib:  ", rv)
 
-        assert np.allclose(rv, RV, atol=1e-1, rtol=1e-1)
+        assert np.allclose(rv, RV)
 
 
 def test_Rotation_as_mrp():
     for i in range(NUM_RANDOM):
         R = Rot.random()
         r = Rotation(R.as_quat())
```

### Comparing `spatial_casadi-1.0.4/test/test_transformation.py` & `spatial_casadi-1.1.0/test/test_transformation.py`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.4/test/test_translation.py` & `spatial_casadi-1.1.0/test/test_translation.py`

 * *Files identical despite different names*

### Comparing `spatial_casadi-1.0.4/test/test_utils.py` & `spatial_casadi-1.1.0/test/test_utils.py`

 * *Files identical despite different names*

