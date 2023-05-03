# Comparing `tmp/abspy-0.2.2.tar.gz` & `tmp/abspy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abspy-0.2.2.tar", last modified: Mon Nov  7 19:07:44 2022, max compression
+gzip compressed data, was "abspy-0.2.3.tar", last modified: Wed May  3 12:43:35 2023, max compression
```

## Comparing `abspy-0.2.2.tar` & `abspy-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 zhaiyu     (501) staff       (20)        0 2022-11-07 19:07:44.324010 abspy-0.2.2/
--rw-r--r--   0 zhaiyu     (501) staff       (20)     1068 2022-02-15 10:09:23.000000 abspy-0.2.2/LICENSE
--rw-r--r--   0 zhaiyu     (501) staff       (20)       16 2022-02-15 10:09:23.000000 abspy-0.2.2/MANIFEST.in
--rw-r--r--   0 zhaiyu     (501) staff       (20)     7246 2022-11-07 19:07:44.324227 abspy-0.2.2/PKG-INFO
--rw-r--r--   0 zhaiyu     (501) staff       (20)     6715 2022-11-07 18:42:49.000000 abspy-0.2.2/README.md
-drwxr-xr-x   0 zhaiyu     (501) staff       (20)        0 2022-11-07 19:07:44.307737 abspy-0.2.2/abspy/
--rw-r--r--   0 zhaiyu     (501) staff       (20)      209 2022-11-07 17:08:28.000000 abspy-0.2.2/abspy/__init__.py
--rw-r--r--   0 zhaiyu     (501) staff       (20)    34197 2022-11-02 19:23:57.000000 abspy-0.2.2/abspy/complex.py
--rw-r--r--   0 zhaiyu     (501) staff       (20)    17426 2022-10-30 09:53:55.000000 abspy-0.2.2/abspy/graph.py
--rw-r--r--   0 zhaiyu     (501) staff       (20)     2194 2022-02-15 10:09:23.000000 abspy-0.2.2/abspy/logger.py
--rw-r--r--   0 zhaiyu     (501) staff       (20)    26890 2022-10-30 09:56:51.000000 abspy-0.2.2/abspy/primitive.py
--rw-r--r--   0 zhaiyu     (501) staff       (20)      129 2022-11-07 18:53:28.000000 abspy-0.2.2/abspy/version.py
-drwxr-xr-x   0 zhaiyu     (501) staff       (20)        0 2022-11-07 19:07:44.310387 abspy-0.2.2/abspy.egg-info/
--rw-r--r--   0 zhaiyu     (501) staff       (20)     7246 2022-11-07 19:07:44.000000 abspy-0.2.2/abspy.egg-info/PKG-INFO
--rw-r--r--   0 zhaiyu     (501) staff       (20)      337 2022-11-07 19:07:44.000000 abspy-0.2.2/abspy.egg-info/SOURCES.txt
--rw-r--r--   0 zhaiyu     (501) staff       (20)        1 2022-11-07 19:07:44.000000 abspy-0.2.2/abspy.egg-info/dependency_links.txt
--rw-r--r--   0 zhaiyu     (501) staff       (20)        6 2022-11-07 19:07:44.000000 abspy-0.2.2/abspy.egg-info/top_level.txt
-drwxr-xr-x   0 zhaiyu     (501) staff       (20)        0 2022-11-07 19:07:44.323604 abspy-0.2.2/docs/
--rw-r--r--   0 zhaiyu     (501) staff       (20)     6148 2022-11-07 19:00:17.000000 abspy-0.2.2/docs/.DS_Store
--rw-r--r--   0 zhaiyu     (501) staff       (20)      638 2022-02-15 10:09:23.000000 abspy-0.2.2/docs/Makefile
--rw-r--r--   0 zhaiyu     (501) staff       (20)      769 2022-02-15 10:09:23.000000 abspy-0.2.2/docs/make.bat
--rw-r--r--   0 zhaiyu     (501) staff       (20)       72 2022-11-07 16:38:58.000000 abspy-0.2.2/docs/requirements.txt
--rw-r--r--   0 zhaiyu     (501) staff       (20)      518 2022-11-07 18:53:28.000000 abspy-0.2.2/pyproject.toml
--rw-r--r--   0 zhaiyu     (501) staff       (20)      627 2022-11-07 19:07:44.325299 abspy-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:43:35.520900 abspy-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 12:43:22.000000 abspy-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 12:43:22.000000 abspy-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-03 12:43:35.520900 abspy-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-03 12:43:22.000000 abspy-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:43:35.516900 abspy-0.2.3/abspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-03 12:43:22.000000 abspy-0.2.3/abspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-05-03 12:43:22.000000 abspy-0.2.3/abspy/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-05-03 12:43:22.000000 abspy-0.2.3/abspy/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-03 12:43:22.000000 abspy-0.2.3/abspy/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27884 2023-05-03 12:43:22.000000 abspy-0.2.3/abspy/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:43:22.000000 abspy-0.2.3/abspy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:43:35.520900 abspy-0.2.3/abspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-03 12:43:35.000000 abspy-0.2.3/abspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 12:43:35.000000 abspy-0.2.3/abspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:43:35.000000 abspy-0.2.3/abspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 12:43:35.000000 abspy-0.2.3/abspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:43:35.520900 abspy-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 12:43:22.000000 abspy-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-03 12:43:22.000000 abspy-0.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 12:43:22.000000 abspy-0.2.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 12:43:22.000000 abspy-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 12:43:35.520900 abspy-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:43:35.520900 abspy-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-03 12:43:22.000000 abspy-0.2.3/tests/test_combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-03 12:43:22.000000 abspy-0.2.3/tests/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-03 12:43:22.000000 abspy-0.2.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 12:43:22.000000 abspy-0.2.3/tests/test_primitive.py
```

### Comparing `abspy-0.2.2/LICENSE` & `abspy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `abspy-0.2.2/PKG-INFO` & `abspy-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: abspy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python tool for 3D adaptive binary space partitioning and beyond
 Home-page: https://github.com/chenzhaiyu/abspy
 Author: Zhaiyu Chen
 Author-email: zhaiyu.chen@outlook.com
+License: 'MIT'
 Project-URL: Bug Tracker, https://github.com/chenzhaiyu/abspy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/logo.png" width="480"/>
 
 -----------
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/abspy.svg)](https://pypi.python.org/pypi/abspy/) [![Build status](https://readthedocs.org/projects/abspy/badge/)](https://abspy.readthedocs.io/en/latest/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://img.shields.io/pypi/v/abspy)](https://pypi.python.org/pypi/abspy/) [![Build status](https://readthedocs.org/projects/abspy/badge/)](https://abspy.readthedocs.io/en/latest/)
 
 ## Introduction
 
 ***abspy*** is a Python tool for 3D *adaptive binary space partitioning* and beyond: an ambient 3D space is adaptively partitioned to form a linear cell complex with pre-detected planar primitives in a point cloud, where an adjacency graph is dynamically obtained. Though the tool is designed primarily to support compact surface reconstruction, it can be extrapolated to other applications as well.
 
+<div align="center" width="480">
+  <img src="https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/animation.gif"><br>
+</div>
+
 ## Key features
 
 * Manipulation of planar primitives detected from point clouds
 * Linear cell complex creation with adaptive binary space partitioning (a-BSP)
 * Dynamic BSP-tree ([NetworkX](https://networkx.org/) graph) updated locally upon insertion of primitives
 * Support of polygonal surface reconstruction from graph cuts
 * Compatible data structure with [Easy3D](https://github.com/LiangliangNan/Easy3D) on point clouds, primitives, cell complexes and surfaces
@@ -123,33 +128,33 @@
 # perform graph-cut to extract surface
 _, _ = adjacency_graph.cut()
 
 # save surface model to an OBJ file
 adjacency_graph.save_surface_obj('surface.obj', engine='rendering')
 ```
 
-Usage can be found at [API reference](https://abspy.readthedocs.io/en/latest/api.html). For the data structure of a `.vg`/`.bvg` file, please refer to [VertexGroup](https://abspy.readthedocs.io/en/latest/vertexgroup.html).
+Usage can be found at [API reference](https://abspy.readthedocs.io/en/latest/api.html). For the data structure of a `.vg`/`.bvg` file, refer to [VertexGroup](https://abspy.readthedocs.io/en/latest/vertexgroup.html).
 
 ## Misc
 
 * **Why adaptive?**
 
-Adaptive space partitioning can significantly reduce computations for cell complex creation, compared to the exhaustive counterpart. The excessive number of cells from the latter not only hinders computation but also inclines to defective surfaces on subtle structures where inaccurate labels are more likely to be assigned.
+The adaptive strategy significantly unburdens computations for cell complex creation, compared to the exhaustive counterpart, yet retaining meaningful space partitions.
 
 ![adaptive](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/adaptive.png)
 
-Run the benchmark on the number of candidate cells and runtime among adaptive partitioning, exhaustive partitioning, and SageMath's [hyperplane arrangements](https://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/hyperplane_arrangement/arrangement.html):
+Run the benchmark comparing the adaptive, the exhaustive, and SageMath's [hyperplane arrangements](https://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/hyperplane_arrangement/arrangement.html):
 
 ```bash
 python misc/benchmark.py
 ```
 
-* **How can abspy be used for surface reconstruction?**
+* **How can *abspy* be used for surface reconstruction?**
 
-With the cell complex constructed and its adjacency maintained, surface reconstruction can be addressed by a graph cut solver that classifies each cell as being *inside* or *outside* the object. The surface exists in between adjacent cells where one is *inside* and the other is *outside* &mdash; exactly where the cut is performed. For more information, refer to [Points2Poly](https://github.com/chenzhaiyu/points2poly) which wraps ***abspy*** for building surface reconstruction.
+With a constructed cell complex, the surface can be addressed by graph cut &mdash; in between adjacent cells where one being *inside* and the other being *outside* &mdash; exactly where the cut is performed. For more information, refer to ***[Points2Poly](https://github.com/chenzhaiyu/points2poly)*** which wraps ***abspy*** for building surface reconstruction.
 
 ![adaptive](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/surface.png)
 
 ## License
 
 [MIT](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/LICENSE)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `abspy-0.2.2/README.md` & `abspy-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 <img src="https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/logo.png" width="480"/>
 
 -----------
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/abspy.svg)](https://pypi.python.org/pypi/abspy/) [![Build status](https://readthedocs.org/projects/abspy/badge/)](https://abspy.readthedocs.io/en/latest/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://img.shields.io/pypi/v/abspy)](https://pypi.python.org/pypi/abspy/) [![Build status](https://readthedocs.org/projects/abspy/badge/)](https://abspy.readthedocs.io/en/latest/)
 
 ## Introduction
 
 ***abspy*** is a Python tool for 3D *adaptive binary space partitioning* and beyond: an ambient 3D space is adaptively partitioned to form a linear cell complex with pre-detected planar primitives in a point cloud, where an adjacency graph is dynamically obtained. Though the tool is designed primarily to support compact surface reconstruction, it can be extrapolated to other applications as well.
 
+<div align="center" width="480">
+  <img src="https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/animation.gif"><br>
+</div>
+
 ## Key features
 
 * Manipulation of planar primitives detected from point clouds
 * Linear cell complex creation with adaptive binary space partitioning (a-BSP)
 * Dynamic BSP-tree ([NetworkX](https://networkx.org/) graph) updated locally upon insertion of primitives
 * Support of polygonal surface reconstruction from graph cuts
 * Compatible data structure with [Easy3D](https://github.com/LiangliangNan/Easy3D) on point clouds, primitives, cell complexes and surfaces
@@ -108,33 +112,33 @@
 # perform graph-cut to extract surface
 _, _ = adjacency_graph.cut()
 
 # save surface model to an OBJ file
 adjacency_graph.save_surface_obj('surface.obj', engine='rendering')
 ```
 
-Usage can be found at [API reference](https://abspy.readthedocs.io/en/latest/api.html). For the data structure of a `.vg`/`.bvg` file, please refer to [VertexGroup](https://abspy.readthedocs.io/en/latest/vertexgroup.html).
+Usage can be found at [API reference](https://abspy.readthedocs.io/en/latest/api.html). For the data structure of a `.vg`/`.bvg` file, refer to [VertexGroup](https://abspy.readthedocs.io/en/latest/vertexgroup.html).
 
 ## Misc
 
 * **Why adaptive?**
 
-Adaptive space partitioning can significantly reduce computations for cell complex creation, compared to the exhaustive counterpart. The excessive number of cells from the latter not only hinders computation but also inclines to defective surfaces on subtle structures where inaccurate labels are more likely to be assigned.
+The adaptive strategy significantly unburdens computations for cell complex creation, compared to the exhaustive counterpart, yet retaining meaningful space partitions.
 
 ![adaptive](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/adaptive.png)
 
-Run the benchmark on the number of candidate cells and runtime among adaptive partitioning, exhaustive partitioning, and SageMath's [hyperplane arrangements](https://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/hyperplane_arrangement/arrangement.html):
+Run the benchmark comparing the adaptive, the exhaustive, and SageMath's [hyperplane arrangements](https://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/hyperplane_arrangement/arrangement.html):
 
 ```bash
 python misc/benchmark.py
 ```
 
-* **How can abspy be used for surface reconstruction?**
+* **How can *abspy* be used for surface reconstruction?**
 
-With the cell complex constructed and its adjacency maintained, surface reconstruction can be addressed by a graph cut solver that classifies each cell as being *inside* or *outside* the object. The surface exists in between adjacent cells where one is *inside* and the other is *outside* &mdash; exactly where the cut is performed. For more information, refer to [Points2Poly](https://github.com/chenzhaiyu/points2poly) which wraps ***abspy*** for building surface reconstruction.
+With a constructed cell complex, the surface can be addressed by graph cut &mdash; in between adjacent cells where one being *inside* and the other being *outside* &mdash; exactly where the cut is performed. For more information, refer to ***[Points2Poly](https://github.com/chenzhaiyu/points2poly)*** which wraps ***abspy*** for building surface reconstruction.
 
 ![adaptive](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/surface.png)
 
 ## License
 
 [MIT](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/LICENSE)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `abspy-0.2.2/abspy/complex.py` & `abspy-0.2.3/abspy/complex.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,35 +12,38 @@
 
 import os
 import string
 from pathlib import Path
 import itertools
 import heapq
 from copy import copy
-from random import random, choices, uniform
+from random import random, choices, uniform, randint
 import pickle
 import time
 import multiprocessing
 
 import numpy as np
 from tqdm import trange
 import networkx as nx
 import trimesh
 from sage.all import polytopes, QQ, RR, Polyhedron
+from sage.geometry.triangulation.point_configuration import PointConfiguration
+from scipy.spatial import ConvexHull
 
 from .logger import attach_to_log
 from .primitive import VertexGroup
 
 logger = attach_to_log()
 
 
 class CellComplex:
     """
     Class of cell complex from planar primitive arrangement.
     """
+
     def __init__(self, planes, bounds, points=None, initial_bound=None, initial_padding=0.1, additional_planes=None,
                  build_graph=False, quiet=False):
         """
         Init CellComplex.
         Class of cell complex from planar primitive arrangement.
 
         Parameters
@@ -337,15 +340,16 @@
         else:
             # intersection with existing cells' AABB
             center_query = np.mean(bound, axis=0)  # 3,
             center_distance = np.abs(center_query - center_targets)  # N * 3
             extent_query = bound[1] - bound[0]  # 3,
 
             # abs(center_distance) * 2 < (query extent + target extent) for every dimension -> intersection
-            intersection_bound = np.where(np.all(center_distance * 2 < extent_query + extent_targets + epsilon, axis=1))[0]
+            intersection_bound = \
+                np.where(np.all(center_distance * 2 < extent_query + extent_targets + epsilon, axis=1))[0]
 
         # plane-AABB intersection test from extracted intersection_bound only
         # https://gdbooks.gitbooks.io/3dcollisions/content/Chapter2/static_aabb_plane.html
         # compute the projection interval radius of AABB onto L(t) = center + t * normal
         radius = np.dot(extent_targets[intersection_bound] / 2, np.abs(plane[:3]))
         # compute distance of box center from plane
         distance = np.dot(center_targets[intersection_bound], plane[:3]) + plane[3]
@@ -398,15 +402,16 @@
         Implemented for multi-processing across all neighbours.
 
         Parameters
         ----------
         kwargs: (int, Polyhedron object, Polyhedron object, Polyhedron object)
             (neighbour index, positive cell, negative cell, neighbouring cell)
         """
-        n, cell_positive, cell_negative, cell_neighbour = kwargs['n'], kwargs['positive'], kwargs['negative'], kwargs['neighbour']
+        n, cell_positive, cell_negative, cell_neighbour = kwargs['n'], kwargs['positive'], kwargs['negative'], kwargs[
+            'neighbour']
 
         interface_positive = cell_positive.intersection(cell_neighbour)
 
         if interface_positive.dim() == 2:
             # this neighbour can connect with either or both children
             self.graph.add_edge(self.index_node + 1, n)
             interface_negative = cell_negative.intersection(cell_neighbour)
@@ -493,15 +498,16 @@
                         # adjacency test between both created cells and their neighbours
                         # todo:
                         #   Avoid 3d-3d intersection if possible. Unsliced neighbours connect with only one child;
                         #   sliced neighbors connect with both children.
 
                         kwargs = []
                         for n, cell in zip(neighbours, cells_neighbours):
-                            kwargs.append({'n': n, 'positive': cell_positive, 'negative': cell_negative, 'neighbour': cell})
+                            kwargs.append(
+                                {'n': n, 'positive': cell_positive, 'negative': cell_negative, 'neighbour': cell})
 
                         if pool is None:
                             for k in kwargs:
                                 self._intersect_neighbour(k)
                         else:
                             pool.map(self._intersect_neighbour, kwargs)
 
@@ -615,64 +621,174 @@
         Return representatives of cells in the complex.
 
         Parameters
         ----------
         location: str
             'center' represents the average of the vertices of the polyhedron,
             'centroid' represents the center of mass/volume,
-            'random' represents random point(s),
-            'star' represents star-like point(s)
+            'random_r' represents random point(s) by rejection,
+            'random_t' represents random point(s) by tetrahedralization,
+            'skeleton' represents skeleton point(s),
+            'boundary' represents boundary point(s) by triangulation
         num: int
             number of samples per cell, only applies to 'random' and 'star'
 
         Returns
         -------
-        as_float: (n, 3) float for 'center' and 'centroid', or (m, n, 3) for 'random' and 'star'
+        as_float: (n, 3) float for 'center' and 'centroid', or (m, n, 3) for 'random' and 'skeleton' and 'boundary'
             Representatives of cells in the complex.
         """
+        points = []
+
         if location == 'center':
             return [cell.center() for cell in self.cells]
+
         elif location == 'centroid':
             return [cell.centroid() for cell in self.cells]
-        elif location == 'random':
-            points = []
+
+        elif location == 'random_r':
+            # strict random by sampling and rejection
             for cell in self.cells:
                 bbox = cell.bounding_box()
                 points_cell = []
                 while len(points_cell) < num:
                     sample = (uniform(bbox[0][0], bbox[1][0]), uniform(bbox[0][1], bbox[1][1]),
                               uniform(bbox[0][2], bbox[1][2]))
                     if cell.contains(sample):
                         points_cell.append(sample)
                 points.append(points_cell)
             return points
 
-        elif location == 'star':
-            points = []
+        elif location == 'random_t':
+            # strict random by triangulation and sampling
+            def tetrahedron_volume(a, b, c, d, epsilon=10e-6):
+                ab = b - a
+                ac = c - a
+                ad = d - a
+                v = abs(np.dot(ab, np.cross(ac, ad))) / 6.0 + epsilon  # epsilon here to prevent empty volume
+                return v
+
+            for cell in self.cells:
+                points_cell = []
+
+                # triangulate cell
+                vertices = cell.vertices()
+                point_config = PointConfiguration(vertices)
+                triangulation = point_config.triangulate()
+                vertices = np.array([[vertices[v] for v in t] for t in triangulation])
+                volumes = [tetrahedron_volume(*tetra) for tetra in vertices]
+                options = list(range(len(volumes)))
+
+                for _ in range(num):
+                    # select one tetrahedron with volume-based probability
+                    choice = choices(options, volumes)[0]
+
+                    # compute vertex-based probability
+                    u, v, w = sorted([random() for _ in range(3)])
+                    u, v, w = u, v - u, w - v
+
+                    # randomly sample one point within the tetrahedron
+                    v1, v2, v3, v4 = vertices[choice]
+                    point = u * v1 + v * v2 + w * v3 + (1 - u - v - w) * v4
+                    points_cell.append(point)
+                points.append(points_cell)
+            return points
+
+        elif location == 'skeleton':
+            # star-shaped sampling
             for cell in self.cells:
                 vertices = cell.vertices_list()
                 if num <= len(vertices):
                     # vertices given high priority
                     points.append(choices(vertices, k=num))
                 else:
                     num_per_vertex = num // len(vertices)
                     num_remainder = num % len(vertices)
                     centroid = cell.centroid()
                     points_cell = []
                     for vertex in vertices[:-1]:
                         points_cell.extend([vertex + (centroid - np.array(vertex)) / num_per_vertex * i
-                                           for i in range(num_per_vertex)])
+                                            for i in range(num_per_vertex)])
                     # last vertex consumes remainder points
-                    points_cell.extend([vertices[-1] + (centroid - np.array(vertices[-1])) / (num_remainder + num_per_vertex)
-                                       * i for i in range(num_remainder + num_per_vertex)])
+                    points_cell.extend(
+                        [vertices[-1] + (centroid - np.array(vertices[-1])) / (num_remainder + num_per_vertex)
+                         * i for i in range(num_remainder + num_per_vertex)])
                     points.append(points_cell)
             return points
 
+        elif location == 'boundary':
+            # boundary sampling
+            def triangle_area(a, b, c, epsilon=10e-6):
+                ab = b - a
+                ac = c - a
+                cross_prod = np.cross(ab, ac)
+                area = 0.5 * np.linalg.norm(cross_prod) + epsilon
+                return area
+
+            for cell in self.cells:
+                points_cell = []
+
+                # get the list of facets
+                facets = cell.facets()
+
+                # aggregate all triangles
+                triangles = []
+                for f in facets:
+                    vertices = f.vertices()
+                    point_config = PointConfiguration(vertices)
+                    triangulation = point_config.triangulate()  # degrade to 2D triangulation
+                    vertices = np.array([[vertices[v] for v in t] for t in triangulation])
+                    triangles.extend(vertices)
+
+                # assign triangle-wise probabilities proportional to their areas
+                areas = [triangle_area(*triangle) for triangle in triangles]
+                options = list(range(len(areas)))
+
+                for _ in range(num):
+                    # select one triangle with area-based probability
+                    choice = choices(options, areas)[0]
+
+                    # compute vertex-based probability
+                    u, v = sorted([random() for _ in range(2)])
+                    u, v = u, v - u
+
+                    # randomly sample one point within the triangle
+                    v1, v2, v3 = triangles[choice]
+                    point = u * v1 + v * v2 + (1 - u - v) * v3
+                    points_cell.append(point)
+                points.append(points_cell)
+            return points
+
         else:
-            raise ValueError("expected 'center', 'centroid', 'random' or 'star' as mode, got {}".format(location))
+            raise ValueError(
+                "expected 'center', 'centroid', 'random_r', 'random_t', 'skeleton' or 'boundary' as mode, got {}".format(
+                    location))
+
+    def cells_boundary(self, epsilon=1e-5):
+        """
+        Return indices of boundary cells (touching the bounds).
+        These cells could be excluded from a valid reconstruction, only when a significant padding exists.
+
+        Parameters
+        ----------
+        epsilon: float
+            Distance tolerance
+
+        Returns
+        -------
+        as_int: (n, ) int
+            Indices of boundary cells
+        """
+        initial_bound = np.array(self.initial_bound)
+        indices = []
+        for index, cell_bound in enumerate(self.cells_bounds):
+            if (cell_bound[0] < np.array(initial_bound[0]) + epsilon).any() \
+                    or (cell_bound[1] > initial_bound[1] - epsilon).any():
+                indices.append(index)
+        return indices
 
     def cells_in_mesh(self, filepath_mesh, engine='ray'):
         """
         Return indices of cells that are inside a reference mesh.
 
         Parameters
         ----------
```

### Comparing `abspy-0.2.2/abspy/graph.py` & `abspy-0.2.3/abspy/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,14 +422,30 @@
 
         Returns
         -------
         as_list: list of int
             Indices of nodes
         """
         return [self._uid_to_index(i) for i in uids]
+    
+    def to_uids(self, indices):
+        """
+        Convert indices to UIDs.
+
+        Parameters
+        ----------
+        indices: list of int
+            Indices of nodes
+
+        Returns
+        -------
+        as_list: list of int
+            UIDs of nodes
+        """
+        return [self._index_to_uid(i) for i in indices]
 
     def to_dict(self, weights_list):
         """
         Convert a weight list to weight dict keyed by self.uid.
 
         Parameters
         ----------
```

### Comparing `abspy-0.2.2/abspy/logger.py` & `abspy-0.2.3/abspy/logger.py`

 * *Files identical despite different names*

### Comparing `abspy-0.2.2/abspy/primitive.py` & `abspy-0.2.3/abspy/primitive.py`

 * *Files 2% similar despite different names*

```diff
@@ -610,14 +610,40 @@
             points = np.concatenate(points)
 
             # calculate parameters
             plane = VertexGroup.fit_plane(vertices)
             self.planes.append(plane)
             self.bounds.append(self._points_bound(vertices))
             self.points_grouped.append(points)
+
+        # self.mesh.facets do not cover all faces
+        faces_extracted = np.concatenate(self.mesh.facets)
+        faces_left = np.setdiff1d(np.arange(len(self.mesh.faces)), faces_extracted)
+
+        for face_index in faces_left:
+            # group corresponding samples by faces
+            points = []
+            sample_indices = np.where(face_indices == face_index)[0]
+            if len(sample_indices) > 0:
+                points.append(samples[sample_indices])
+
+            # vertices
+            vertices = self.mesh.faces[face_index]
+            vertices = self.mesh.vertices[vertices]
+
+            # append vertices in case there is no sampled points in this group
+            points.append(vertices)
+            points = np.concatenate(points)
+
+            # calculate parameters
+            plane = VertexGroup.fit_plane(vertices)
+            self.planes.append(plane)
+            self.bounds.append(self._points_bound(vertices))
+            self.points_grouped.append(points)
+
         self.points = np.concatenate(self.points_grouped)
 
     def save_vg(self, filepath):
         """
         Save primitives into a vg file.
 
         Parameters
```

### Comparing `abspy-0.2.2/abspy.egg-info/PKG-INFO` & `abspy-0.2.3/abspy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: abspy
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python tool for 3D adaptive binary space partitioning and beyond
 Home-page: https://github.com/chenzhaiyu/abspy
 Author: Zhaiyu Chen
 Author-email: zhaiyu.chen@outlook.com
+License: 'MIT'
 Project-URL: Bug Tracker, https://github.com/chenzhaiyu/abspy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/logo.png" width="480"/>
 
 -----------
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/abspy.svg)](https://pypi.python.org/pypi/abspy/) [![Build status](https://readthedocs.org/projects/abspy/badge/)](https://abspy.readthedocs.io/en/latest/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://img.shields.io/pypi/v/abspy)](https://pypi.python.org/pypi/abspy/) [![Build status](https://readthedocs.org/projects/abspy/badge/)](https://abspy.readthedocs.io/en/latest/)
 
 ## Introduction
 
 ***abspy*** is a Python tool for 3D *adaptive binary space partitioning* and beyond: an ambient 3D space is adaptively partitioned to form a linear cell complex with pre-detected planar primitives in a point cloud, where an adjacency graph is dynamically obtained. Though the tool is designed primarily to support compact surface reconstruction, it can be extrapolated to other applications as well.
 
+<div align="center" width="480">
+  <img src="https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/animation.gif"><br>
+</div>
+
 ## Key features
 
 * Manipulation of planar primitives detected from point clouds
 * Linear cell complex creation with adaptive binary space partitioning (a-BSP)
 * Dynamic BSP-tree ([NetworkX](https://networkx.org/) graph) updated locally upon insertion of primitives
 * Support of polygonal surface reconstruction from graph cuts
 * Compatible data structure with [Easy3D](https://github.com/LiangliangNan/Easy3D) on point clouds, primitives, cell complexes and surfaces
@@ -123,33 +128,33 @@
 # perform graph-cut to extract surface
 _, _ = adjacency_graph.cut()
 
 # save surface model to an OBJ file
 adjacency_graph.save_surface_obj('surface.obj', engine='rendering')
 ```
 
-Usage can be found at [API reference](https://abspy.readthedocs.io/en/latest/api.html). For the data structure of a `.vg`/`.bvg` file, please refer to [VertexGroup](https://abspy.readthedocs.io/en/latest/vertexgroup.html).
+Usage can be found at [API reference](https://abspy.readthedocs.io/en/latest/api.html). For the data structure of a `.vg`/`.bvg` file, refer to [VertexGroup](https://abspy.readthedocs.io/en/latest/vertexgroup.html).
 
 ## Misc
 
 * **Why adaptive?**
 
-Adaptive space partitioning can significantly reduce computations for cell complex creation, compared to the exhaustive counterpart. The excessive number of cells from the latter not only hinders computation but also inclines to defective surfaces on subtle structures where inaccurate labels are more likely to be assigned.
+The adaptive strategy significantly unburdens computations for cell complex creation, compared to the exhaustive counterpart, yet retaining meaningful space partitions.
 
 ![adaptive](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/adaptive.png)
 
-Run the benchmark on the number of candidate cells and runtime among adaptive partitioning, exhaustive partitioning, and SageMath's [hyperplane arrangements](https://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/hyperplane_arrangement/arrangement.html):
+Run the benchmark comparing the adaptive, the exhaustive, and SageMath's [hyperplane arrangements](https://doc.sagemath.org/html/en/reference/discrete_geometry/sage/geometry/hyperplane_arrangement/arrangement.html):
 
 ```bash
 python misc/benchmark.py
 ```
 
-* **How can abspy be used for surface reconstruction?**
+* **How can *abspy* be used for surface reconstruction?**
 
-With the cell complex constructed and its adjacency maintained, surface reconstruction can be addressed by a graph cut solver that classifies each cell as being *inside* or *outside* the object. The surface exists in between adjacent cells where one is *inside* and the other is *outside* &mdash; exactly where the cut is performed. For more information, refer to [Points2Poly](https://github.com/chenzhaiyu/points2poly) which wraps ***abspy*** for building surface reconstruction.
+With a constructed cell complex, the surface can be addressed by graph cut &mdash; in between adjacent cells where one being *inside* and the other being *outside* &mdash; exactly where the cut is performed. For more information, refer to ***[Points2Poly](https://github.com/chenzhaiyu/points2poly)*** which wraps ***abspy*** for building surface reconstruction.
 
 ![adaptive](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/docs/source/_static/images/surface.png)
 
 ## License
 
 [MIT](https://raw.githubusercontent.com/chenzhaiyu/abspy/main/LICENSE)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `abspy-0.2.2/docs/Makefile` & `abspy-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abspy-0.2.2/docs/make.bat` & `abspy-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abspy-0.2.2/pyproject.toml` & `abspy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.2.2"
+current_version = "0.2.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version to {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `abspy-0.2.2/setup.cfg` & `abspy-0.2.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = abspy
-version = 0.2.2
+version = 0.2.3
 author = Zhaiyu Chen
 author_email = zhaiyu.chen@outlook.com
+license = 'MIT'
 description = A Python tool for 3D adaptive binary space partitioning and beyond
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chenzhaiyu/abspy
 project_urls = 
 	Bug Tracker = https://github.com/chenzhaiyu/abspy/issues
 classifiers =
```

