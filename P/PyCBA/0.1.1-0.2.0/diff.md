# Comparing `tmp/PyCBA-0.1.1.tar.gz` & `tmp/PyCBA-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCBA-0.1.1.tar", last modified: Sun Feb  6 16:24:22 2022, max compression
+gzip compressed data, was "PyCBA-0.2.0.tar", last modified: Wed May  3 16:58:56 2023, max compression
```

## Comparing `PyCBA-0.1.1.tar` & `PyCBA-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 16:24:22.058599 PyCBA-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-06 16:23:58.000000 PyCBA-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-02-06 16:24:22.058599 PyCBA-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 16:24:22.058599 PyCBA-0.1.1/PyCBA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-02-06 16:24:21.000000 PyCBA-0.1.1/PyCBA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-02-06 16:24:21.000000 PyCBA-0.1.1/PyCBA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-06 16:24:21.000000 PyCBA-0.1.1/PyCBA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-02-06 16:24:21.000000 PyCBA-0.1.1/PyCBA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-06 16:24:21.000000 PyCBA-0.1.1/PyCBA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-02-06 16:23:58.000000 PyCBA-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 16:24:22.058599 PyCBA-0.1.1/pycba/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7203 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    10911 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/beam.py
--rw-r--r--   0 runner    (1001) docker     (121)    24564 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/bridge.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/inf_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)    20336 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/load.py
--rw-r--r--   0 runner    (1001) docker     (121)    10536 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/results.py
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pycba/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-02-06 16:23:58.000000 PyCBA-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-02-06 16:24:22.058599 PyCBA-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-02-06 16:23:58.000000 PyCBA-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 16:24:22.058599 PyCBA-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 16:23:58.000000 PyCBA-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5498 2022-02-06 16:23:58.000000 PyCBA-0.1.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-02-06 16:23:58.000000 PyCBA-0.1.1/tests/test_bridge.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-02-06 16:23:58.000000 PyCBA-0.1.1/tests/test_inf_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:58:56.920951 PyCBA-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 16:58:41.000000 PyCBA-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-03 16:58:56.920951 PyCBA-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:58:56.916951 PyCBA-0.2.0/PyCBA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-03 16:58:56.000000 PyCBA-0.2.0/PyCBA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-03 16:58:56.000000 PyCBA-0.2.0/PyCBA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:58:56.000000 PyCBA-0.2.0/PyCBA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 16:58:56.000000 PyCBA-0.2.0/PyCBA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 16:58:56.000000 PyCBA-0.2.0/PyCBA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-03 16:58:41.000000 PyCBA-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:58:56.920951 PyCBA-0.2.0/pycba/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/inf_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pycba/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 16:58:41.000000 PyCBA-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-03 16:58:56.920951 PyCBA-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 16:58:41.000000 PyCBA-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:58:56.920951 PyCBA-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:58:41.000000 PyCBA-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-03 16:58:41.000000 PyCBA-0.2.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-03 16:58:41.000000 PyCBA-0.2.0/tests/test_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-03 16:58:41.000000 PyCBA-0.2.0/tests/test_inf_lines.py
```

### Comparing `PyCBA-0.1.1/LICENSE` & `PyCBA-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCBA-0.1.1/PKG-INFO` & `PyCBA-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: PyCBA
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python Continuous Beam Analysis
 Home-page: https://ccaprani.github.io/pycba/
 Author: Colin Caprani
 Author-email: colin.caprani@monash.edu
 License: Apache 2.0
 Project-URL: Documentation, https://ccaprani.github.io/pycba/
 Project-URL: Source, https://github.com/ccaprani/pycba/
 Project-URL: Tracker, https://github.com/ccaprani/pycba/issues/
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -39,9 +38,7 @@
 - Spring supports, both vertical and rotational, enabling it to be used as part of a subframe analysis;
 - Results are output at 100 (user can change) positions along each span, enable accurate deflection estimation.
 
 One of the main functions of `PyCBA` is that the basic analysis engine forms the basis for higher-level analysis. Current `PyCBA` includes modules for:
 
 - Influence line generation
 - Moving load analysis for bridges, targeted at bridge access assessments
-
-
```

### Comparing `PyCBA-0.1.1/PyCBA.egg-info/PKG-INFO` & `PyCBA-0.2.0/PyCBA.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: PyCBA
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python Continuous Beam Analysis
 Home-page: https://ccaprani.github.io/pycba/
 Author: Colin Caprani
 Author-email: colin.caprani@monash.edu
 License: Apache 2.0
 Project-URL: Documentation, https://ccaprani.github.io/pycba/
 Project-URL: Source, https://github.com/ccaprani/pycba/
 Project-URL: Tracker, https://github.com/ccaprani/pycba/issues/
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -39,9 +38,7 @@
 - Spring supports, both vertical and rotational, enabling it to be used as part of a subframe analysis;
 - Results are output at 100 (user can change) positions along each span, enable accurate deflection estimation.
 
 One of the main functions of `PyCBA` is that the basic analysis engine forms the basis for higher-level analysis. Current `PyCBA` includes modules for:
 
 - Influence line generation
 - Moving load analysis for bridges, targeted at bridge access assessments
-
-
```

### Comparing `PyCBA-0.1.1/README.md` & `PyCBA-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PyCBA-0.1.1/pycba/analysis.py` & `PyCBA-0.2.0/pycba/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         R : np.ndarray
             A vector describing the support conditions at each member end.
         LM : Optional[list[list[Union[int, float]]]]
             The load matrix: a list of loads on the beam; each load with several parameters.
         eletype : Optional[np.ndarray]
             A vector of the member types. Defaults to a fixed-fixed element.
 
-
         Returns
         -------
         None.
 
         """
         self.npts = 100
         self._beam_results = None
@@ -82,27 +81,31 @@
         Returns
         -------
         None.
 
         """
         self._beam.loads = LM
 
-    def analyze(self) -> int:
+    def analyze(self, npts: Optional[int] = None) -> int:
         """
         Conducts the analysis on the constructed BeamAnalysis object
 
         Parameters
         ----------
-        None
+        npts : Optional[int]
+            The number of evaluation points along a member for load effects.
 
         Returns
         -------
         0 for a succesful execution
 
         """
+        if npts and npts > 3:
+            self.npts = npts
+
         fU = self._forces()
         f = np.copy(fU)
         ksysU = self._assemble()
         ksys = np.copy(ksysU)
         ksys, f = self._apply_bc(ksys, f)
         d = self._solver(ksys, f)
         r = self._reactions(ksysU, d, fU)
@@ -268,7 +271,9 @@
 
         ax = axs[2]
         ax.plot([0, L], [0, 0], "k", lw=2)
         ax.plot(res.x, res.D * 1e3, "r")
         ax.grid()
         ax.set_ylabel("Deflection (mm)")
         ax.set_xlabel("Distance along beam (m)")
+
+        plt.show()
```

### Comparing `PyCBA-0.1.1/pycba/beam.py` & `PyCBA-0.2.0/pycba/beam.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.1.1/pycba/bridge.py` & `PyCBA-0.2.0/pycba/bridge.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,268 +1,24 @@
 """
 PyCBA - Continuous Beam Analysis - Bridge Crossing Module
 """
-from typing import Optional, Union, Dict
+from __future__ import annotations  # https://bit.ly/3KYiL2o
+from typing import Optional, Union, Dict, List
 import numpy as np
 import matplotlib.pyplot as plt
 from .analysis import BeamAnalysis
 from .results import Envelopes, BeamResults
-
-
-class Vehicle:
-    """
-    A basic vehicle definition for a bridge crossing analysis
-    """
-
-    def __init__(self, axle_spacings: np.ndarray, axle_weights: np.ndarray):
-        """
-        Constructs the :class:`pycba.bridge.Vehicle` object from the supplied data.
-
-        Parameters such as vehicle length, weight, and axle coordinates are
-        calculated from the supplied data.
-
-        Parameters
-        ----------
-        axle_spacings : np.ndarray
-            A vector of axle spacings of length one fewer than the length of the
-            vector of axle weights
-        axle_weights : np.ndarray
-            A vector of axle weights, length one greater than the length of the
-            axle spacings vector.
-
-        Raises
-        ------
-        ValueError
-            If the lengths of the vectors of axle weights and spacings are
-            inconsistent.
-
-        Returns
-        -------
-        None.
-
-        """
-        self.axs = np.asarray(axle_spacings)
-        self.axw = np.asarray(axle_weights)
-
-        if len(self.axs) + 1 != len(self.axw):
-            raise ValueError("Inconsistent axle spacing and weight counts")
-
-        self.L = sum(axle_spacings)
-        self.W = sum(axle_weights)
-        self.NoAxles = len(axle_weights)
-        self.axle_coords = np.zeros(self.NoAxles)
-        for i, s in enumerate(self.axs):
-            self.axle_coords[i + 1] = self.axle_coords[i] + s
-
-
-class VehicleLibrary:
-    """
-    A repository of some useful vehicles for analysis
-    """
-
-    abag_bdouble_aw = (
-        np.array(
-            [
-                6,
-                17 / 2,
-                17 / 2,
-                22.5 / 3,
-                22.5 / 3,
-                22.5 / 3,
-                22.5 / 3,
-                22.5 / 3,
-                22.5 / 3,
-            ]
-        )
-        * 9.81
-    )  # t to kN
-
-    abag_bdouble_as = [
-        [3.0, 1.2, 5.5, 1.2, 1.2, 6.5, 1.2, 1.2],
-        [3.0, 1.2, 6.0, 1.2, 1.2, 6.0, 1.2, 1.2],
-        [3.0, 1.2, 6.5, 1.2, 1.2, 5.5, 1.2, 1.2],
-    ]
-
-    abag_semitrailer_aw = (
-        np.array([6, 17 / 2, 17 / 2, 22.5 / 2, 22.5 / 2, 22.5 / 3]) * 9.81
-    )  # t to kN
-
-    abag_semitrailer_as = [
-        [3.0, 1.2, 4.4, 1.2, 1.2],
-        [3.0, 1.2, 6.4, 1.2, 1.2],
-        [3.0, 1.2, 8.4, 1.2, 1.2],
-        [3.0, 1.2, 10.4, 1.2, 1.2],
-    ]
-
-    @classmethod
-    def get_abag_bdouble(cls, iax: int) -> Vehicle:
-        """
-        Creates one of the Australian Bridge Assessment Guidelines (ABAG) 68.5 t
-        B-double trucks.
-
-        Parameters
-        ----------
-        iax : int
-            The 0-based index of the variable axle spacing required:
-
-                - **0**: Variable spacings are 5.5 and 6.5 from front
-                - **1**: Variable spacings are 6.0 and 6.0 from front
-                - **2**: Variable spacings are 6.5 and 5.5 from front
-
-        Returns
-        -------
-        Vehicle
-            The :class:`pycba.bridge.Vehicle` object.
-
-        """
-        return Vehicle(cls.abag_bdouble_as[iax], cls.abag_bdouble_aw)
-
-    @classmethod
-    def get_abag_semitrailer(cls, iax: int) -> Vehicle:
-        """
-        Creates one of the Australian Bridge Assessment Guidelines (ABAG) 45 t
-        semi-trailer trucks
-
-        Parameters
-        ----------
-        iax : int
-            The 0-based index of the variable axle spacing required:
-
-                - **0**: Variable spacing is 4.4 m
-                - **1**: Variable spacing is 6.4 m
-                - **2**: Variable spacing is 8.4 m
-                - **3**: Variable spacing is 10.4 m
-
-        Returns
-        -------
-        Vehicle
-            The :class:`pycba.bridge.Vehicle` object.
-        """
-        return Vehicle(cls.abag_semitrailer_as[iax], cls.abag_semitrailer_aw)
-
-    @staticmethod
-    def get_example_permit() -> Vehicle:
-        """
-        An example B-double type truck that might seek a network access permit.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        Vehicle
-            The :class:`pycba.bridge.Vehicle` object.
-        """
-        axs = np.array([1.793, 2.507, 1.370, 5.403, 1.232, 1.232, 6.303, 1.232, 1.232])
-        axw = np.array([5.5, 5.5, 8.5, 8.5, 7.5, 7.5, 7.5, 7.5, 7.5, 7.5]) * 9.81
-        return Vehicle(axs, axw)
-
-    @staticmethod
-    def get_m1600(middle_spacing: float) -> Vehicle:
-        """
-        The AS5100 M1600 load model truck. This is the notional load model for
-        moving traffic and is usually critical for short to medium span bridges
-        once the dyanmic load allowance is included.
-
-        Parameters
-        ----------
-        middle_spacing : float
-            The spacing for the variable middle axle spacing; min. 6.25 m.
-
-        Raises
-        ------
-        ValueError
-            If the supplied spacing is less than the code-specified minimum
-            of 6.25 m.
-
-        Returns
-        -------
-        Vehicle
-            The :class:`pycba.bridge.Vehicle` object.
-        """
-        if middle_spacing < 6.25:
-            raise ValueError("Min. M1600 middle spacing is 6.25 m")
-        axs = [
-            1.25,
-            1.25,
-            3.75,
-            1.25,
-            1.25,
-            middle_spacing,
-            1.25,
-            1.25,
-            5.0,
-            1.25,
-            1.25,
-        ]
-        axw = 120 * np.ones(12)
-        return Vehicle(axs, axw)
-
-    @staticmethod
-    def get_s1600(middle_spacing: float) -> Vehicle:
-        """
-        The AS5100 S1600 load model truck. This is the notional load model for
-        stationary traffic and is criticial for longer spans.
-
-        Parameters
-        ----------
-        middle_spacing : float
-            The spacing for the variable middle axle spacing; min. 6.25 m.
-
-        Raises
-        ------
-        ValueError
-            If the supplied spacing is less than the code-specified minimum
-            of 6.25 m.
-
-        Returns
-        -------
-        Vehicle
-            The :class:`pycba.bridge.Vehicle` object.
-        """
-        if middle_spacing < 6.25:
-            raise ValueError("Min. S1600 middle spacing is 6.25 m")
-        axs = [
-            1.25,
-            1.25,
-            3.75,
-            1.25,
-            1.25,
-            middle_spacing,
-            1.25,
-            1.25,
-            5.0,
-            1.25,
-            1.25,
-        ]
-        axw = 80 * np.ones(12)
-        return Vehicle(axs, axw)
-
-    @staticmethod
-    def get_validation_truck() -> Vehicle:
-        """
-        A set of moving loads used for validation on a 20 m span against the
-        textbook, "Structural and Stress Analysis"", 2nd edn., Megson, p. 579.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        Vehicle
-            The :class:`pycba.bridge.Vehicle` object.
-        """
-        return Vehicle(np.array([4, 4]), np.array([5, 4, 3]))
+from .vehicle import Vehicle
 
 
 class BridgeAnalysis:
     """
-    Performs a bridge crossing analysis for a defined vehicle
+    Performs a bridge crossing analysis for a defined vehicle. The vehicle is moved
+    from the zero global x-coordinate of the beam until it has left the beam at the
+    far end.
     """
 
     def __init__(
         self, ba: Optional[BeamAnalysis] = None, veh: Optional[Vehicle] = None
     ):
         """
         Can instantiate with nothing and later add or define the objects, or
@@ -290,27 +46,35 @@
         EI: Union[float, np.ndarray],
         R: np.ndarray,
         eletype: Optional[np.ndarray] = None,
     ):
         """
         Create and add a beam to a bridge analysis
 
+        Parameters
+        ----------
         L : np.ndarray
             A vector of span lengths.
         EI : Union[float, np.ndarray]
             A vector of member flexural rigidities.
         R : np.ndarray
             A vector describing the support conditions at each member end.
         LM : Optional[list[list[Union[int, float]]]]
             The load matrix: a list of loads on the beam; each load with several
             parameters.
         eletype : Optional[np.ndarray]
             A vector of the member types. Defaults to a fixed-fixed element.
+
+        Returns
+        -------
+        ba : BeamAnalysis
+            A :class:`pycba.analysis.BeamAnalysis` object.
         """
         self.ba = BeamAnalysis(L=L, EI=EI, R=R, eletype=eletype)
+        return self.ba
 
     def set_bridge(self, ba: BeamAnalysis):
         """
         Set the bridge for the bridge analysis.
 
         Parameters
         ----------
@@ -332,16 +96,22 @@
         ----------
         axle_spacings : np.ndarray
             A vector of axle spacings of length one fewer than the length of the
             vector of axle weights
         axle_weights : np.ndarray
             A vector of axle weights, length one greater than the length of the
             axle spacings vector.
+
+        Returns
+        -------
+        veh : Vehicle
+            A :class:`pycba.bridge.Vehicle` object.
         """
         self.veh = Vehicle(axle_spacings, axle_weights)
+        return self.veh
 
     def set_vehicle(self, veh: Vehicle):
         """
         Set the vehicle for the bridge analysis.
 
         Parameters
         ----------
@@ -621,21 +391,20 @@
         env_ratios = {}
         env_ratios["x"] = ref_env.x
         env_ratios["Mmax"] = get_ratio(trial_env.Mmax, ref_env.Mmax)
         env_ratios["Mmin"] = get_ratio(trial_env.Mmin, ref_env.Mmin)
         env_ratios["Vmax"] = get_ratio(trial_env.Vmax, ref_env.Vmax)
         env_ratios["Vmin"] = get_ratio(trial_env.Vmin, ref_env.Vmin)
         env_ratios["nsup"] = ref_env.nsup
+
+        maxvals = get_ratio(trial_env.Rmaxval, ref_env.Rmaxval)
+        minvals = get_ratio(trial_env.Rminval, ref_env.Rminval)
         for i in range(ref_env.nsup):
-            env_ratios[f"Rmax{i}"] = get_ratio(
-                trial_env.Rmax[i, :].max(), ref_env.Rmax[i, :].max()
-            )
-            env_ratios[f"Rmin{i}"] = get_ratio(
-                trial_env.Rmin[i, :].min(), ref_env.Rmin[i, :].min()
-            )
+            env_ratios[f"Rmax{i}"] = maxvals[i]
+            env_ratios[f"Rmin{i}"] = minvals[i]
 
         return env_ratios
 
     def plot_static(self, pos: float, axs: Optional[plt.Axes] = None):
         """
         Plots for analysis of static vehicle
 
@@ -719,23 +488,38 @@
         ax.plot(x, env.Vmin, "b")
         ax.grid()
         ax.set_ylabel("Shear Force (kN)")
         ax.set_xlabel("Distance along beam (m)")
 
         # Reactions in right panel
         subfigs[1].suptitle("Support Reactions")
-        axsRight = subfigs[1].subplots(nreactions, 1, sharex=True)
 
-        for i, ax in enumerate(axsRight):
-            ax.plot([0, L], [0, 0], "k", lw=2)
-            ax.plot(self.pos, env.Rmax[i, :], "r")
-            ax.plot(self.pos, env.Rmin[i, :], "b")
-            ax.grid()
-            ax.set_ylabel(f"Reaction {i+1} (kN/kNm)")
-        axsRight[-1].set_xlabel("Position of Front Axle (m)")
+        # Check if consistent envelope
+        if len(self.pos) == env.Rmax.shape[1]:
+            axsRight = subfigs[1].subplots(nreactions, 1, sharex=True)
+            for i, ax in enumerate(axsRight):
+                ax.plot([0, L], [0, 0], "k", lw=2)
+                ax.plot(self.pos, env.Rmax[i, :], "r")
+                ax.plot(self.pos, env.Rmin[i, :], "b")
+                ax.grid()
+                ax.set_ylabel(f"Reaction {i+1} (kN/kNm)")
+            axsRight[-1].set_xlabel("Position of Front Axle (m)")
+
+        else:  # Otherwise envelope of envelopes
+            axsRight = subfigs[1].subplots(2, 1, sharex=True)
+            for i, (ax, le, col) in enumerate(
+                zip(axsRight, ["max", "min"], ["r", "b"])
+            ):
+                r = eval(f"env.R{le}val")  # kinda yuk!
+                ax.bar(np.arange(env.nsup), r, color=col)
+                ax.set_xticks(np.arange(env.nsup))
+                ax.set_xticklabels([f"R{i+1}" for i in range(env.nsup)])
+                ax.set_ylabel(f"Reactions [{le}]")
+                ax.grid()
+            axsRight[1].set_xlabel("Reaction ID")
 
     def plot_ratios(self, env_ratios: Dict[str, np.ndarray]):
         """
         Plots the output of :meth:`pycba.bridge.BridgeAnalysis.envelopes_ratios`.
 
         Parameters
         ----------
@@ -791,15 +575,15 @@
         subfigs[1].suptitle("Support Reactions")
         axsRight = subfigs[1].subplots(2, 1, sharex=True)
 
         for i, (ax, le, col) in enumerate(zip(axsRight, ["max", "min"], ["r", "b"])):
             r = np.array([env_ratios[f"R{le}{i}"] for i in range(nsup)])
             ax.bar(np.arange(nsup), r, color=col)
             ax.set_xticks(np.arange(nsup))
-            ax.set_xticklabels([f"R {i+1}" for i in range(nsup)])
+            ax.set_xticklabels([f"R{i+1}" for i in range(nsup)])
             ax.set_ylabel(f"Reaction Ratio [{le}]")
             ax.grid()
         axsRight[1].set_xlabel("Reaction ID")
 
     def _check_objects(self):
         """
         Check that suitable objects are defined before an analysis is run.
```

### Comparing `PyCBA-0.1.1/pycba/inf_lines.py` & `PyCBA-0.2.0/pycba/inf_lines.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.1.1/pycba/load.py` & `PyCBA-0.2.0/pycba/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 PyCBA - Load module
 
-.. autodata:: LoadMatrix
-
-The load matrix represents the loads as a `List` of `Lists`. 
+The load matrix represents the loads as a `List` of `Lists`.
 Each list entry represents a single load and must be in the following format:
 
      Span No. | Load Type | Load Value | Distance a | Load Cover c
-     
-Load Types are: 
+
+Load Types are:
 
     1 - **Uniformly Distributed Loads**, which only have a load value; distances `a` and `c` are set to "0".
-    
+
     2 - **Point Loads**, located at `a` from the left end of the span; distances `c` is set to "0".
-    
+
     3 - **Partial UDLs**, starting at `a` for a distance of `c` (i.e. the cover) where $L >= a+c$.
-    
+
     4 - **Moment Load**, located at `a`; distances `c` is set to "0".
-    
+
 It has dimension `M` x 5, where `M` is the number of loads applied to the beam.
+
+The type alias `LoadMatrix` is defined as
+
+.. autodata:: LoadMatrix
+
 """
 
 from __future__ import annotations
 from typing import Union, List, NamedTuple, Tuple, Optional
 import numpy as np
 
 # Define a type alias
@@ -192,25 +195,28 @@
         Parameters
         ----------
         v : np.ndarray
             The vector to which the Macaulay Bracket will be applied
         """
         return v.clip(0.0)
 
-    def H(self, v: np.ndarray) -> np.ndarray:
+    def H(self, v: np.ndarray, value: float = 0.0) -> np.ndarray:
         """
         Heaviside step function: values less than zero are clipped to zero;
         values greater than zero are clipped to unity; zeros are retained.
 
         Parameters
         ----------
         v : np.ndarray
             The vector to which the Heaviside function will be applied
+        value : float
+            The value of the Heaviside function at zero, usually 0, but sometimes
+            0.5 (average of adjacent values) or 1.0.
         """
-        return np.heaviside(v, 0)
+        return np.heaviside(v, value)
 
     def released_end_forces(self, cnl: LoadCNL, L: float, eType: int) -> LoadCNL:
         """
         The released end forces for each element type: converts the Consistent Nodal
         Loads of the applied loading to the correct nodal loading depending on the
         element type.
 
@@ -710,16 +716,33 @@
         m = self.M
         a = self.a
         b = L - a
 
         Va = m / L
         Ra = (m / 6) * (3 * b**2 / L - L)
 
+        # # For moment we must insert an additional point to properly capture the step
+        # idx = np.searchsorted(x, a)
+        # if not np.any(np.isclose(x, a)):
+        #     x = np.insert(x, idx, a)
+        # x = np.insert(x, idx, a)
+        # res.x = x
+
         res.V = Va * np.ones(npts)
-        res.M = Va * x - m * self.H(x - a)
+
+        if a == 0:
+            res.M = Va * x - m * self.H(x - a, 1)
+        elif a == L:
+            res.M = Va * x - m * self.H(x - a, 0)
+        else:
+            res.M = Va * x - m * self.H(x - a, 0.5)
+
+        # res.M = np.array(
+        #     [Va * xi - m if i > idx else Va * xi for i, xi in enumerate(x)]
+        # )
         res.R = (Va / 2) * x**2 - m * self.MB(x - a) + Ra
         res.D = (Va / 6) * x**3 - (m / 2) * self.MB(x - a) ** 2 + Ra * x
 
         res.V[0] = 0.0
         res.V[npts - 1] = 0.0
         res.M[0] = 0.0
         res.M[npts - 1] = 0.0
```

### Comparing `PyCBA-0.1.1/pycba/results.py` & `PyCBA-0.2.0/pycba/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         res = MaMb.get_mbr_results(x, L)
 
         # Now get the results for all the applied loads on a simple span
         for load in beam.loads:
             if load.i_span != i_span:
                 continue
             res += load.get_mbr_results(x, L)
+
         # And superimpose end displacements using Moment-Area
         h = L / self.npts
         EI = beam.mbr_EIs[i_span]
 
         R = integrate.cumtrapz(res.M[1:-1], dx=h, initial=0) / EI + d[1]
         D = integrate.cumtrapz(R, dx=h, initial=0) + d[0]
 
@@ -189,14 +190,16 @@
         self.npts = len(self.x)
         self.nres = len(vResults)
         self.nsup = len(vResults[0].R)
 
         self.Vmax, self.Vmin = self._get_envelope_V()
         self.Mmax, self.Mmin = self._get_envelope_M()
         self.Rmax, self.Rmin = self._get_envelope_R()
+        self.Rmaxval = self.Rmax.max(axis=1)
+        self.Rminval = self.Rmin.min(axis=1)
 
     def _get_envelope_V(self) -> Tuple[np.ndarray, np.ndarray]:
         """
         Creates the envelopes for shear.
 
         Parameters
         ----------
@@ -293,23 +296,29 @@
         zero_env.Vmax = np.zeros(env.npts)
         zero_env.Vmin = np.zeros(env.npts)
         zero_env.Mmax = np.zeros(env.npts)
         zero_env.Mmin = np.zeros(env.npts)
         for i in range(env.nsup):
             zero_env.Rmax[i] = np.zeros(env.nres)
             zero_env.Rmin[i] = np.zeros(env.nres)
+        zero_env.Rmaxval = np.zeros(env.nsup)
+        zero_env.Rminval = np.zeros(env.nsup)
         return zero_env
 
     def augment(self, env: Envelopes):
         """
         Augments this set of envelopes with another compatible set, making this the
         envelopes of the two sets of envelopes.
 
         All envelopes must be from the same :class:`pycba.bridge.BridgeAnalysis` object.
 
+        If the envelopes have a different number of analyses (due to differing vehicle
+        lengths, for example), then only the reaction extreme are retained, and not
+        the entire reaction history.
+
         Parameters
         ----------
         env : Envelopes
             A compatible :class:`pycba.results.Envelopes` object.
 
         Raises
         ------
@@ -317,17 +326,25 @@
             All envelopes must be for the same bridge.
 
         Returns
         -------
         None.
         """
 
-        if self.nres != env.nres or self.npts != env.npts or self.nsup != env.nsup:
+        if self.npts != env.npts or self.nsup != env.nsup:
             raise ValueError("Cannot augment with an inconsistent envelope")
         self.Vmax = np.maximum(self.Vmax, env.Vmax)
         self.Vmin = np.minimum(self.Vmin, env.Vmin)
 
         self.Mmax = np.maximum(self.Mmax, env.Mmax)
         self.Mmin = np.minimum(self.Mmin, env.Mmin)
 
-        self.Rmax = np.maximum(self.Rmax, env.Rmax)
-        self.Rmin = np.minimum(self.Rmin, env.Rmin)
+        self.Rmaxval = np.maximum(self.Rmaxval, env.Rmaxval)
+        self.Rminval = np.minimum(self.Rminval, env.Rminval)
+
+        if self.nres == env.nres:
+            self.Rmax = np.maximum(self.Rmax, env.Rmax)
+            self.Rmin = np.minimum(self.Rmin, env.Rmin)
+        else:
+            # Ensure no misleading results returned
+            self.Rmax = np.zeros((self.nsup, self.nres))
+            self.Rmin = np.zeros((self.nsup, self.nres))
```

### Comparing `PyCBA-0.1.1/pycba/utils.py` & `PyCBA-0.2.0/pycba/utils.py`

 * *Files identical despite different names*

### Comparing `PyCBA-0.1.1/setup.cfg` & `PyCBA-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyCBA-0.1.1/tests/test_basic.py` & `PyCBA-0.2.0/tests/test_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     r = beam_analysis.beam_results.R
     assert r == pytest.approx([14.0, 57.6, -21.6, 28.0])
 
     dmax = max(beam_analysis.beam_results.results.D)
     dmin = min(beam_analysis.beam_results.results.D)
     assert [dmax, dmin] == pytest.approx(
-        [0.00017713513888888886, -0.00042251493055555565], abs=1e-6
+        [0.00017414416666666662, -0.00042251493055555565], abs=1e-6
     )
 
 
 def test_3span_diff_settlement():
     L = [15, 15, 15]
     EI = 30 * np.array([500e8, 500e8, 500e8]) * 1e-6  # kNm2
     R = [-1, 0, 1e8, 0, 1e8, 0, -1, 0]
@@ -175,7 +175,24 @@
     R = [-1, -1, 0, 0, -1, 0, -1, 0]
 
     ils = cba.InfluenceLines(L, EI, R, eType)
     ils.create_ils(step=0.05)
     (x, y) = ils.get_il(15.0, "V")
 
     assert [min(y), max(y)] == pytest.approx([-0.4009469062500001, 0.59375], abs=1e-6)
+
+
+def test_moment_load():
+    L = [10.0]
+    EI = 30 * 600e7 * np.ones(len(L)) * 1e-6
+    eType = [1]
+    R = [-1, 0, -1, 0]
+
+    for a in [0, 5, 10]:
+        LM = [[1, 4, 10, a, 0]]
+        beam_analysis = cba.BeamAnalysis(L, EI, R, LM, eType)
+        out = beam_analysis.analyze()
+        assert out == 0
+
+        # Check deflection closes
+        d = beam_analysis.beam_results.D[[0, 2]]
+        assert d == pytest.approx([0.0, 0.0])
```

### Comparing `PyCBA-0.1.1/tests/test_inf_lines.py` & `PyCBA-0.2.0/tests/test_inf_lines.py`

 * *Files identical despite different names*

