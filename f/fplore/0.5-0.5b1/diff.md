# Comparing `tmp/fplore-0.5.tar.gz` & `tmp/fplore-0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplore-0.5.tar", last modified: Wed May  3 19:11:16 2023, max compression
+gzip compressed data, was "fplore-0.5b1.tar", last modified: Thu Apr 13 15:59:23 2023, max compression
```

## Comparing `fplore-0.5.tar` & `fplore-0.5b1.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:16.576019 fplore-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-03 19:10:57.000000 fplore-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 19:11:16.576019 fplore-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-03 19:10:57.000000 fplore-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-03 19:10:57.000000 fplore-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:11:16.576019 fplore-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-03 19:10:57.000000 fplore-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:16.572019 fplore-0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:16.576019 fplore-0.5/src/fplore/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8774 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/arpes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/fast_util.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:16.576019 fplore-0.5/src/fplore/files/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19325 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/files/band.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/files/dos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/files/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-05-03 19:10:57.000000 fplore-0.5/src/fplore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:16.576019 fplore-0.5/src/fplore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 19:11:16.000000 fplore-0.5/src/fplore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 19:11:16.000000 fplore-0.5/src/fplore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:11:16.000000 fplore-0.5/src/fplore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-03 19:11:16.000000 fplore-0.5/src/fplore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 19:11:16.000000 fplore-0.5/src/fplore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:11:16.576019 fplore-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-03 19:10:57.000000 fplore-0.5/tests/test_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-03 19:10:57.000000 fplore-0.5/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.940894 fplore-0.5b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-13 15:59:15.000000 fplore-0.5b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-13 15:59:23.940894 fplore-0.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 15:59:15.000000 fplore-0.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.936893 fplore-0.5b1/fplore/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.940894 fplore-0.5b1/fplore/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18963 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/files/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-13 15:59:15.000000 fplore-0.5b1/fplore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.936893 fplore-0.5b1/fplore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 15:59:23.000000 fplore-0.5b1/fplore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:59:23.940894 fplore-0.5b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 15:59:15.000000 fplore-0.5b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:59:23.940894 fplore-0.5b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-13 15:59:15.000000 fplore-0.5b1/tests/test_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 15:59:15.000000 fplore-0.5b1/tests/test_util.py
```

### Comparing `fplore-0.5/LICENSE` & `fplore-0.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fplore-0.5/PKG-INFO` & `fplore-0.5b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: fplore
-Version: 0.5
+Version: 0.5b1
 Summary: FPLO run evaluation
+Home-page: https://github.com/mueslo/fplore
 License: GPLv3
-Project-URL: Homepage, https://github.com/mueslo/fplore
-Keywords: dft,fplo,physics,chemistry
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: <4,>=3.8
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-Provides-Extra: tests-core
 Provides-Extra: docs
 License-File: LICENSE
 
 [![](https://img.shields.io/github/release/mueslo/fplore.svg?style=flat-square)](https://github.com/mueslo/fplore/releases)
 [![](https://img.shields.io/pypi/v/fplore.svg?style=flat-square)](https://pypi.org/project/fplore/)
-[![](https://img.shields.io/github/actions/workflow/status/mueslo/fplore/tests.yml?branch=master&style=flat-square)](https://github.com/mueslo/fplore/actions/workflows/tests.yml)
+[![](https://img.shields.io/github/workflow/status/mueslo/fplore/Run%20tests/master?style=flat-square)](https://github.com/mueslo/fplore/actions/workflows/tests.yml)
 [![](https://img.shields.io/readthedocs/fplore.svg?style=flat-square)](https://fplore.readthedocs.io)
 [![](https://img.shields.io/github/license/mueslo/fplore.svg?style=flat-square)](https://github.com/mueslo/fplore/blob/master/LICENSE)
 
 
 # fplore
 A python library for [FPLO](https://www.fplo.de/) run evaluation.
```

### Comparing `fplore-0.5/README.md` & `fplore-0.5b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![](https://img.shields.io/github/release/mueslo/fplore.svg?style=flat-square)](https://github.com/mueslo/fplore/releases)
 [![](https://img.shields.io/pypi/v/fplore.svg?style=flat-square)](https://pypi.org/project/fplore/)
-[![](https://img.shields.io/github/actions/workflow/status/mueslo/fplore/tests.yml?branch=master&style=flat-square)](https://github.com/mueslo/fplore/actions/workflows/tests.yml)
+[![](https://img.shields.io/github/workflow/status/mueslo/fplore/Run%20tests/master?style=flat-square)](https://github.com/mueslo/fplore/actions/workflows/tests.yml)
 [![](https://img.shields.io/readthedocs/fplore.svg?style=flat-square)](https://fplore.readthedocs.io)
 [![](https://img.shields.io/github/license/mueslo/fplore.svg?style=flat-square)](https://github.com/mueslo/fplore/blob/master/LICENSE)
 
 
 # fplore
 A python library for [FPLO](https://www.fplo.de/) run evaluation.
```

### Comparing `fplore-0.5/src/fplore/files/band.py` & `fplore-0.5b1/fplore/files/band.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,32 +400,25 @@
 
     @cached_property
     def interpolator(self):
         """Default interpolator from Band.get_interpolator()"""
         return self.get_interpolator()
 
     @staticmethod
-    def smooth_overlap(arr_e, e=0., scale=0.02, axis=2, weights=None):
-        """
-        Calculates the Gaussian overlap of the energy levels in arr_e with the Fermi level or desired energy level `e`.
-        Useful for generating smooth Fermi surface pseudospectra.
-
-        :param arr_e: array containing energy levels of shape (..., n_e)
-        :param e: energy level to calculate overlap for (default: 0)
-        :param scale: scale of the gaussian (default: 0.02)
-        :param axis: extra axis or tuple of axes along which the energy levels are summed (default: -1)
-        :param weights: weights for each energy level, should have shape compatible with e_k_3d (default: None)
-        """
-        arr_e[np.isnan(arr_e)] = -np.inf
-        t1 = norm.pdf(arr_e, loc=e, scale=scale)
-        sum_axis = (-1,) if axis is None else (axis, -1)
+    def smooth_overlap(e_k_3d, e=0., scale=0.02, axis=2, weights=None):
+        log.debug('smooth_overlap {} {}', e_k_3d.shape, weights)
+        e_k_3d[np.isnan(e_k_3d)] = -np.inf
+        t1 = norm.pdf(e_k_3d, loc=e, scale=scale)
 
         if weights is not None:
-            weights = np.ones_like(arr_e) * weights
-        return np.average(t1, axis=sum_axis, weights=weights)
+            assert weights.ndim == 1 and len(weights) == e_k_3d.shape[axis]
+            weights_shape = [1]*e_k_3d.ndim
+            weights_shape[axis] = len(weights)
+            weights = np.ones_like(e_k_3d) * weights.reshape(weights_shape)
+        return np.average(t1, axis=(axis, -1), weights=weights)  # todo why sum tuple?
 
     @classmethod
     def apply_symmetry(cls, data, symm_ops, basis=None):
         """
         Applies the given symmetry operations to the k-space coordinates in
         `data` and returns a structured array with fields `k` and `idx`.
 
@@ -439,15 +432,16 @@
             k_points = k_points @ np.linalg.inv(basis)  # from cartesian to basis vectors
         num_k = len(k_points)
 
         k_idx = np.arange(num_k)
         new_data_idx = cls._gen_band_data_array(num_k*len(symm_ops),
                                                 k_coords=True, index=True)
         for i, op in enumerate(symm_ops):
-            new_k_points = k_points @ op.T    # .T since we are multiplying from the right
+            rot = op.rotation_matrix
+            new_k_points = k_points @ rot.T    # .T important! == op.operate_multi(k_points)
             new_data_idx['k'][num_k*i:num_k*(i+1)] = new_k_points
             new_data_idx['idx'][num_k*i:num_k*(i+1)] = k_idx
 
         log.debug('applied {} symm ops to {} k points', len(symm_ops), num_k)
         new_data_idx = remove_duplicates(new_data_idx)
 
         if basis is not None:
```

### Comparing `fplore-0.5/src/fplore/files/base.py` & `fplore-0.5b1/fplore/files/base.py`

 * *Files identical despite different names*

### Comparing `fplore-0.5/src/fplore/files/config.py` & `fplore-0.5b1/fplore/files/config.py`

 * *Files identical despite different names*

### Comparing `fplore-0.5/src/fplore/files/dos.py` & `fplore-0.5b1/fplore/files/dos.py`

 * *Files identical despite different names*

### Comparing `fplore-0.5/src/fplore/files/misc.py` & `fplore-0.5b1/fplore/files/misc.py`

 * *Files identical despite different names*

### Comparing `fplore-0.5/src/fplore/plot.py` & `fplore-0.5b1/fplore/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,21 +107,20 @@
 
 
 class Arrow3D(FancyArrowPatch):
     def __init__(self, xs, ys, zs, *args, **kwargs):
         FancyArrowPatch.__init__(self, (0, 0), (0, 0), *args, **kwargs)
         self._verts3d = xs, ys, zs
 
-    def do_3d_projection(self, renderer=None):
+    def do_3d_projection(self, renderer):  # renderer arg will be removed in matplotlib==3.6
         xs3d, ys3d, zs3d = self._verts3d
         xs, ys, zs = proj3d.proj_transform(xs3d, ys3d, zs3d, self.axes.M)
         self.set_positions((xs[0], ys[0]), (xs[1], ys[1]))
-        if renderer is not None:  # matplotlib<3.6
-            FancyArrowPatch.draw(self, renderer)
-        return min(zs)
+        FancyArrowPatch.draw(self, renderer)
+        return 0
 
     draw = do_3d_projection  # for matplotlib<3.5
 
 
 # from http://stackoverflow.com/questions/23840756/
 def orthogonal_proj(zfront, zback):
     a = (zfront + zback) / (zfront - zback)
@@ -190,14 +189,15 @@
 
         for label, coord in points.items():
             ax.text(*coord, s='${}$'.format(label), color='k')
 
     ax.set_xlabel('$k_x$')
     ax.set_ylabel('$k_y$')
     ax.set_zlabel('$k_z$')
+    ax.legend()
 
 
 def plot_bz_proj(run, ax, neighbours=False, rot=None, axis=-1, vectors=True,
                  **kwargs):
     """Projects along given axis (default: last axis) after applying
     rotation matrix rot"""
     if rot is None:
```

### Comparing `fplore-0.5/src/fplore/run.py` & `fplore-0.5b1/fplore/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 from functools import cached_property
 
 import numpy as np
 from scipy.spatial.transform import Rotation
 from pymatgen.core import Structure, Lattice
+from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.symmetry.groups import SpaceGroup, sg_symbol_from_int_number
 from pymatgen.symmetry.bandstructure import HighSymmKpath
 
 from .logging import log
 from .util import backfold_k, rot_v1_v2
 from .files.base import FPLOFile
 from .files import DOS
@@ -148,43 +149,18 @@
             coords.append([float(x) for x in wp.tau])
 
         structure = Structure.from_spacegroup(
             self.spacegroup_symbol, self.lattice, elements, coords)
 
         return structure
 
-    @cached_property
-    def point_group_operations_frac(self):
-        """Returns the point group operations in real space lattice fractional coordinates.
-        Identity (E) is guaranteed to be first."""
-
-        # note: SpacegroupAnalyzer(self.structure).get_point_group_operations(cartesian=False) gives the actual
-        # symmetry and should typically give the same results, but sometimes you might intentionally be running
-        # in a lower symmetry setting than the actual symmetry, so we use the declared symmetry instead.
-
-        seen = set()
-        pg_ops = [op.rotation_matrix for op in self.spacegroup.symmetry_ops
-                  if not op.rotation_matrix.tobytes() in seen
-                  and seen.add(op.rotation_matrix.tobytes()) is None]  # for uniqueness
-
-        return sorted(pg_ops, key=lambda x: np.linalg.norm(x - np.eye(3)))  # ensure identity is first
-
-    @cached_property
+    @property
     def point_group_operations(self):
-        """Returns the point group operations in cartesian coordinates.
-        Identity (E) is guaranteed to be first."""
-
-        pg_ops_cart = []
-        for op_frac in self.point_group_operations_frac:
-            op = self.lattice.matrix.T @ op_frac @ self.lattice.inv_matrix.T  # fractional -> cartesian
-            op[abs(op) < 1e-12] = 0  # nearly zero
-            nearly_1 = (abs(abs(op) - 1) < 1e-12)  # nearly +-1
-            op[nearly_1] = np.rint(op[nearly_1])
-            pg_ops_cart.append(op)
-        return pg_ops_cart
+        # returns the point group operations in cartesian coordinates
+        return SpacegroupAnalyzer(self.structure).get_point_group_operations(cartesian=True)
 
     @property
     def primitive_structure(self):
         return self.structure.get_primitive_structure()
 
     @property
     def primitive_lattice(self):
```

### Comparing `fplore-0.5/src/fplore/util.py` & `fplore-0.5b1/fplore/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 import numpy as np
 from scipy.ndimage import map_coordinates
 from scipy.spatial.distance import cdist
 from scipy.spatial.transform import Rotation
 from scipy.spatial import Delaunay, Voronoi
 import scipy.cluster.hierarchy as hcluster
+from scipy.constants import hbar, m_e, eV, angstrom, c
 from pymatgen.core import Lattice
 
 from .logging import log
-from .fast_util import backfold_k_inplace
 
 nbs = (0, 1, -1)
-neighbours = list(itertools.product(nbs, nbs, nbs))  # 27
-pe_neighbours = list(itertools.product(nbs[:-1], nbs[:-1], nbs[:-1]))  # 8
+neighbours = list(itertools.product(nbs, nbs, nbs))
 idx_000 = neighbours.index((0, 0, 0))
 
 def cartesian_product(*xs):
     """Iterates over primary axis first, then second, etc."""
     return np.array(np.meshgrid(*xs, indexing='ij')).reshape(len(xs), -1).T
 
 
@@ -73,20 +72,18 @@
         xs_grid = np.linspace(dim_min, dim_max, len(xs), dtype=dtype)
         assert np.allclose(xs, xs_grid, **tol), "xs"
         axes_grid.append(xs_grid)
 
     return axes_grid
 
 
-def find_basis(lattice_points):
-    """Given lattice points of shape (N, 3), this function attempts to find a basis"""
-
-    min_length = 1e-6
+def find_basis(lattice_points):  
+    basis = []
     dists = np.linalg.norm(lattice_points, axis=1)
-    valid = (dists > min_length)
+    valid = (dists != 0)
     lattice_points = lattice_points[valid]
     dists = dists[valid]
     
     n=12
     
     # find n shortest vectors
     partition = np.argpartition(dists, n)[:n]
@@ -248,107 +245,90 @@
     extra_ijk = np.array(list(expanded_lattice_ijk - ksamp_lattice_ijk))
     extra_k = extra_ijk @ ksamp_lattice.matrix
 
     return extra_k, extra_ijk"""
 
 
 def backfold_k_parallelepiped(lattice, b, atol=1e-4):
-    """Fold an array of k-points b (shape (..., 3)) back to the parallelepiped
-    spanned by the lattice vectors."""
-    return ((b @ lattice.inv_matrix + atol) % 1 - atol) @ lattice.matrix
+    b_shape = b.shape
+    b = b.reshape((-1, 3))  # convert (..., 3) to (N, 3) shape
+    b = ((b @ lattice.inv_matrix + atol) % 1 - atol) @ lattice.matrix
+    return b.reshape(b_shape)
+
+
+def backfold_k(lattice, b):
+    """
+    Folds an array of k-points b (shape (..., 3)) back to the first
+    Brillouin zone given a reciprocal lattice matrix A.
+
+    Translationally equivalent points will be mapped to the same actual point.
+
+    Note: Assumes that the lattice vectors contained in A correspond to the
+    shortest lattice vectors, i.e. that pairwise combinations of reciprocal
+    lattice vectors in A and their negatives cover all the nearest neighbours
+    of the BZ.
+    """
 
+    # TODO handle points on borders of BZ more elegantly
+    # TODO make sure translationally equivalent points not present (brillouin zone boundary)
 
-BOUNDARY_ATOL = 1e-6  # for BZ/backfolding
-def backfold_k_old(lattice, b):
+    # get adjacent BZ cell's Gamma point locations
     assert idx_000 == 0
-    # get adjacent BZ cells and all parallelepiped corners
-    neighbours_frac = wigner_seitz_neighbours(lattice) | set(pe_neighbours[1:])
-    neighbours_k = np.array(list(neighbours_frac)) @ lattice.matrix
-    neighbours_k = np.vstack([[0, 0, 0], neighbours_k])  # we rely on idx_000 being 0
-    log.debug("#neighbours_k: {}", len(neighbours_k))
+    neighbours_k = np.array(neighbours) @ lattice.matrix
+
+    #would reduce memory usage:
+    #neighbours_k = np.array(list(wigner_seitz_neighbours(lattice))) @ lattice.matrix
+    #neighbours_k = np.vstack([[0, 0, 0], neighbours_k])
+
+    # make a copy of `b' since we will be operating directly on it
+    b_shape = b.shape
+    b = np.copy(b).reshape((-1, 3))  # convert (..., 3) to (N, 3) shape
 
     # to reduce problems due to translational equivalence (borders of BZ)
     # we directly fold to the parallelepiped spanned by the reciprocal lattice basis
     b = backfold_k_parallelepiped(lattice, b)
 
-    b_shape = b.shape
-    b = b.reshape(-1, 3)  # for some reason it is faster WITH a reshape
-
     # all coordinates need to be backfolded initially
-    idx_requires_backfolding = np.ones(b.shape[:-1], dtype=bool)  # boolean indexing
+    idx_requires_backfolding = np.arange(len(b))
     i = 0
     while True:
         i += 1
         if i > 20:
             raise Exception('Backfolding failed')
         log.debug('backfolding... (round {})', i)
 
         # calculate distances to nearest neighbour BZ origins
         dists = cdist(b[idx_requires_backfolding], neighbours_k)
 
         # get the index of the BZ origin to which distance is minimal
-        # if multiple dists are minimal, choose the one with the lowest index
-        # (this is important for translational equivalence stability w.r.t numerical error)
-        bz_idx = np.argmax((dists - dists.min(axis=1)[:, np.newaxis]) < BOUNDARY_ATOL, axis=1)
+        # bz_idx = np.argmin(dists, axis=1)  # naive, but does not work reliably w.r.t.
+        #                                      translational equivalence due to float inaccuracies
+        bz_idx = np.argmax(np.isclose(dists, np.min(dists, axis=1)[:, np.newaxis]), axis=1)  # argmax for first True
 
         # perform backfolding
         backfolded = b[idx_requires_backfolding] - neighbours_k[bz_idx]
 
         # get indices of points that were backfolded (boolean index array)
-        idx_backfolded = (bz_idx != idx_000)
+        idx_backfolded = np.any(b[idx_requires_backfolding] != backfolded,
+                                axis=1)
 
         log.debug('backfolded {} of {} coordinates',
-                  idx_backfolded.sum(),
+                  np.sum(idx_backfolded),
                   len(idx_requires_backfolding))
 
-        if not idx_backfolded.any():
+        if not np.any(idx_backfolded):
             log.debug("backfolding finished")
             return b.reshape(b_shape)
 
         # assign backfolded coordinates to output array
         b[idx_requires_backfolding] = backfolded
 
         # only those coordinates which were changed in this round need to be
-        # backfolded again in the next round
-        idx_requires_backfolding[idx_requires_backfolding] = idx_backfolded
-
-
-def backfold_k(lattice, b):
-    """
-    Folds an array of k-points b (shape (..., 3)) back to the first
-    Brillouin zone given a reciprocal lattice matrix A.
-
-    Guarantees that translationally equivalent points will be mapped to
-    the same output point.
-
-    Note: Assumes that the lattice vectors contained in A correspond to the
-    shortest lattice vectors, i.e. that pairwise combinations of reciprocal
-    lattice vectors in A and their negatives cover all the nearest neighbours
-    of the BZ.
-    """
-
-    # TODO handle points on borders of BZ more elegantly
-    # TODO make sure translationally equivalent points not present (brillouin zone boundary)
-    # TODO drop nans from input and emit warning, and add them back in output
-
-    assert idx_000 == 0
-    # get adjacent BZ cells and all parallelepiped corners
-    neighbours_frac = wigner_seitz_neighbours(lattice) | set(pe_neighbours[1:])
-    neighbours_k = np.array(list(neighbours_frac)) @ lattice.matrix
-    neighbours_k = np.vstack([[0, 0, 0], neighbours_k])  # we rely on idx_000 being 0
-    log.debug("#neighbours_k: {}", len(neighbours_k))
-
-    # to reduce problems due to translational equivalence (borders of BZ)
-    # we directly fold to the parallelepiped spanned by the reciprocal lattice basis
-    b = backfold_k_parallelepiped(lattice, b, 0.5+BOUNDARY_ATOL)
-
-    b_shape = b.shape
-    b = b.reshape(-1, 3)
-    backfold_k_inplace(neighbours_k, b)
-    return b.reshape(b_shape)
+        # backfolded again
+        idx_requires_backfolding = idx_requires_backfolding[idx_backfolded]
 
 
 def remove_duplicates(data):
     """Remove non-unique k-points from data"""
 
     unique, idx = np.unique(data['k'].round(decimals=5),
                             return_index=True, axis=0)
@@ -393,15 +373,16 @@
     ws_neighbours = list(wigner_seitz_neighbours(reciprocal_lattice))
     idx_000 = 0
     ws_neighbours.insert(idx_000, (0, 0, 0))
     neighbours_k = np.array(ws_neighbours) @ reciprocal_lattice.matrix
     dists = cdist(p, neighbours_k)
 
     # prevent float inaccuracies from folding on 1st BZ borders:
-    dists[:, idx_000] -= BOUNDARY_ATOL
+    dists[:, idx_000] -= 1e-6
+
     return np.argmin(dists, axis=1) == idx_000
 
 
 def in_hull(p, hull, **kwargs):
     """
     Test if points in `p` are within `hull`
     """
@@ -453,23 +434,28 @@
     cpm = np.array([[0, -cp[2], cp[1]],
                    [cp[2], 0, -cp[0]],
                    [-cp[1], cp[0], 0]])
 
     return np.eye(3) + cpm + np.dot(cpm, cpm) * 1 / (1 + c)
 
 
-def project(v, t):
-    """Project vector v onto target vector t"""
-    v = np.array(v)
-    t = np.array(t)
-    return np.dot(v, t) / np.dot(t, t) * t
+def k_arpes(theta, e_photon, phi_det, v0, e_bind=0., theta2=0., geometry=None):
+    """Returns the parallel and perpendicular components of electronic plane
+    wave exiting a crystal with inner potential `v0` at angle `theta` with an
+    energy of `e_electron`"""
+
+    e_photon *= eV
+    phi_det *= eV
+    e_bind *= eV
+    v0 *= eV
+    e_electron = e_photon - e_bind - phi_det
+    k = np.array([angstrom*np.sqrt(2 * m_e * e_electron) * np.sin(theta)/hbar,
+         angstrom*np.sqrt(2 * m_e * e_electron) * np.sin(theta2) * np.cos(theta)/hbar,  # noqa: E501
+         angstrom*np.sqrt(2 * m_e * (e_electron * (np.cos(theta)**2 * np.cos(theta2)**2) + v0))/hbar]).T  # noqa: E501
+
+    if geometry:
+        log.debug('using photon momentum correction')
+        k = (k - angstrom*(e_photon/(hbar*c))*geometry.photon_direction_sample_coords)
 
-def project_plane(v, n):
-    """Project vector v onto plane with normal n"""
-    v = np.array(v)
-    n = np.array(n)
-    return v - project(v, n)
+    return k
 
-def normalized(v):
-    """Returns normalized v"""
-    v = np.array(v)
-    return v / np.linalg.norm(v)
+#k_arpes = np.vectorize(k_arpes, signature='(1),(1),(1),(1),(1?),(1?),(1?)->(3)')
```

### Comparing `fplore-0.5/src/fplore.egg-info/PKG-INFO` & `fplore-0.5b1/fplore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: fplore
-Version: 0.5
+Version: 0.5b1
 Summary: FPLO run evaluation
+Home-page: https://github.com/mueslo/fplore
 License: GPLv3
-Project-URL: Homepage, https://github.com/mueslo/fplore
-Keywords: dft,fplo,physics,chemistry
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Python: <4,>=3.8
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-Provides-Extra: tests-core
 Provides-Extra: docs
 License-File: LICENSE
 
 [![](https://img.shields.io/github/release/mueslo/fplore.svg?style=flat-square)](https://github.com/mueslo/fplore/releases)
 [![](https://img.shields.io/pypi/v/fplore.svg?style=flat-square)](https://pypi.org/project/fplore/)
-[![](https://img.shields.io/github/actions/workflow/status/mueslo/fplore/tests.yml?branch=master&style=flat-square)](https://github.com/mueslo/fplore/actions/workflows/tests.yml)
+[![](https://img.shields.io/github/workflow/status/mueslo/fplore/Run%20tests/master?style=flat-square)](https://github.com/mueslo/fplore/actions/workflows/tests.yml)
 [![](https://img.shields.io/readthedocs/fplore.svg?style=flat-square)](https://fplore.readthedocs.io)
 [![](https://img.shields.io/github/license/mueslo/fplore.svg?style=flat-square)](https://github.com/mueslo/fplore/blob/master/LICENSE)
 
 
 # fplore
 A python library for [FPLO](https://www.fplo.de/) run evaluation.
```

### Comparing `fplore-0.5/tests/test_band.py` & `fplore-0.5b1/tests/test_band.py`

 * *Files identical despite different names*

### Comparing `fplore-0.5/tests/test_util.py` & `fplore-0.5b1/tests/test_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 # todo: edge + vertex points?
 # todo: stability (+epsilon)?
 
 
 class TestBackfold:
     @pytest_cases.parametrize("points", [gamma_point, boundary_points])
     def test_translational_invariance(self, reciprocal_lattice, points, neighbours_k):
-        # create n_t translationally equivalent points, shape (n_t, n, 3)
+        # create translationally equivalent points
         points_t = points + np.vstack([[0, 0, 0], neighbours_k])[:, np.newaxis, :]
 
         bf = backfold_k(reciprocal_lattice, points_t)  # todo matrix remove for testing
 
         # assert that backfolded coordinates are equal
         equal = np.all(np.isclose(bf[0], bf), axis=(0, 2))
```

