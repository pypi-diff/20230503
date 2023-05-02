# Comparing `tmp/Pulse3D-0.32.6.tar.gz` & `tmp/Pulse3D-0.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.32.6.tar", last modified: Fri Apr 28 20:20:34 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.0.tar", last modified: Tue May  2 22:17:34 2023, max compression
```

## Comparing `Pulse3D-0.32.6.tar` & `Pulse3D-0.33.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.292044 Pulse3D-0.32.6/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-28 20:19:26.000000 Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 20:20:34.300044 Pulse3D-0.32.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 20:20:34.000000 Pulse3D-0.32.6/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-28 20:20:34.000000 Pulse3D-0.32.6/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:20:17.000000 Pulse3D-0.32.6/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-28 20:19:57.000000 Pulse3D-0.32.6/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:20:34.296044 Pulse3D-0.32.6/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45310 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-28 20:19:23.000000 Pulse3D-0.32.6/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.977733 Pulse3D-0.33.0/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-02 22:16:27.000000 Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.977733 Pulse3D-0.33.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 22:17:34.000000 Pulse3D-0.33.0/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 22:17:34.000000 Pulse3D-0.33.0/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:17:17.000000 Pulse3D-0.33.0/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-02 22:16:56.000000 Pulse3D-0.33.0/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:17:34.981733 Pulse3D-0.33.0/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45310 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-02 22:16:23.000000 Pulse3D-0.33.0/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.32.6/LICENSE` & `Pulse3D-0.33.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/PKG-INFO` & `Pulse3D-0.33.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.6
+Version: 0.33.0
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.6/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.0/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.0/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/setup.py` & `Pulse3D-0.33.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.32.6",
+    version="0.33.0",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.32.6/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.0/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.32.6
+Version: 0.33.0
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.32.6/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.0/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.0/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.0/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.0/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/constants.py` & `Pulse3D-0.33.0/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.0/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/exceptions.py` & `Pulse3D-0.33.0/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.0/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/metrics.py` & `Pulse3D-0.33.0/src/pulse3D/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import pandas as pd
 from pandas import DataFrame
 from pandas import Series
 from pulse3D.transforms import get_time_window_indices
 
 from .compression_cy import interpolate_x_for_y_between_two_points
 from .compression_cy import interpolate_y_for_x_between_two_points
+from .constants import DEFAULT_BASELINE_WIDTHS
 from .constants import DEFAULT_TWITCH_WIDTH_PERCENTS
 from .constants import INTERPOLATED_DATA_PERIOD_SECONDS
 from .constants import MICRO_TO_BASE_CONVERSION
 from .constants import PRIOR_VALLEY_INDEX_UUID
 from .constants import SUBSEQUENT_VALLEY_INDEX_UUID
 
 
@@ -109,87 +110,98 @@
         statistics_df = pd.DataFrame.from_dict(statistics)
         return statistics_df
 
 
 class TwitchAmplitude(BaseMetric):
     """Calculate the amplitude for each twitch."""
 
-    def __init__(self, rounded: bool = False, **kwargs: Dict[str, Any]):
+    def __init__(
+        self,
+        rounded: bool = False,
+        baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
+        **kwargs: Dict[str, Any],
+    ):
         super().__init__(rounded=rounded, **kwargs)
+        # C10 in the metric definition diagram is the C point at 90% twitch width
+        self.baseline_widths = [100 - baseline_widths_to_use[0], baseline_widths_to_use[1]]
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         **kwargs: Dict[str, Any],
     ) -> Series:
-
         amplitudes = self.calculate_amplitudes(
-            twitch_indices=twitch_indices, filtered_data=filtered_data, rounded=self.rounded
+            twitch_indices=twitch_indices,
+            filtered_data=filtered_data,
+            rounded=self.rounded,
+            baseline_widths=tuple(self.baseline_widths),
         )
 
         return amplitudes
 
     @staticmethod
     def calculate_amplitudes(
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         filtered_data: NDArray[(2, Any), int],
+        baseline_widths: Tuple[int, ...],
         rounded: bool = False,
     ) -> Series:
         """Get the amplitudes for all twitches.
 
         Given amplitude of current peak, and amplitude of prior/subsequent valleys, twitch amplitude
         is calculated as the mean distance from peak to both valleys.
 
         Args:
             twitch_indices: a dictionary in which the key is an integer representing (TODO fix this for every metric) of interest and the value is an inner dictionary with various UUID
                 of prior/subsequent peaks and valleys and their index values.
 
             filtered_data: a 2D array of the time and value (magnetic, voltage, displacement, force)
                 data after it has gone through noise filtering
 
+            baseline_widths: tuple twitch widths to use as baseline metrics
+
         Returns:
             Pandas Series of float values representing the amplitude of each twitch
         """
-        twitch_width = 90
-
         _, coordinates = TwitchWidth.calculate_twitch_widths(
             filtered_data=filtered_data,
             twitch_indices=twitch_indices,
-            twitch_width_percents=(twitch_width,),
+            twitch_width_percents=baseline_widths,
             rounded=rounded,
             as_dict=True,  # Tanner (1/20/23): using as_dict=True here to speed this up. This calculation is performed in the MA Controller, so it must be as fast as possible
         )
 
         estimates_dict: Dict[int, float] = dict()
 
         for twitch_peak_idx, twitch_data in coordinates.items():
             twitch_peak_x, twitch_peak_y = filtered_data[:, twitch_peak_idx]
 
-            # C10 in the metric definition diagram is the C point at 90% twitch width
-            c10x = twitch_data["time"]["contraction"][twitch_width]
-            c10y = twitch_data["force"]["contraction"][twitch_width]
-            r90x = twitch_data["time"]["relaxation"][twitch_width]
-            r90y = twitch_data["force"]["relaxation"][twitch_width]
+            c10x = twitch_data["time"]["contraction"][baseline_widths[0]]
+            c10y = twitch_data["force"]["contraction"][baseline_widths[0]]
+            r90x = twitch_data["time"]["relaxation"][baseline_widths[1]]
+            r90y = twitch_data["force"]["relaxation"][baseline_widths[1]]
 
             twitch_base_y = interpolate_y_for_x_between_two_points(twitch_peak_x, c10x, c10y, r90x, r90y)
             amplitude_y = twitch_peak_y - twitch_base_y
 
             estimates_dict[twitch_peak_idx] = amplitude_y
 
         estimates = pd.Series(estimates_dict)
         return estimates
 
 
 class TwitchFractionAmplitude(TwitchAmplitude):
     """Calculate the fraction of max amplitude for each twitch."""
 
-    def __init__(self, **kwargs: Dict[str, Any]):
-        super().__init__(rounded=False, **kwargs)
+    def __init__(
+        self, baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS, **kwargs: Dict[str, Any]
+    ):
+        super().__init__(rounded=False, baseline_widths_to_use=baseline_widths_to_use, **kwargs)
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         **kwargs: Dict[str, Any],
@@ -371,39 +383,37 @@
 class TwitchVelocity(BaseMetric):
     """Calculate velocity of each contraction or relaxation twitch."""
 
     def __init__(
         self,
         rounded: bool = False,
         is_contraction: bool = True,
-        twitch_width_percents: Tuple[int, ...] = DEFAULT_TWITCH_WIDTH_PERCENTS,
+        baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
         **kwargs: Dict[str, Any],
     ):
         super().__init__(rounded=rounded, **kwargs)
 
-        self.twitch_width_percents = twitch_width_percents
+        self.baseline_widths = baseline_widths_to_use
 
-        velocity_start = min(self.twitch_width_percents)
-        velocity_end = max(self.twitch_width_percents)
-        self.velocity_index_start = self.twitch_width_percents.index(velocity_start)
-        self.velocity_index_end = self.twitch_width_percents.index(velocity_end)
+        self.velocity_start = self.baseline_widths[0]
+        self.velocity_end = self.baseline_widths[1]
 
         self.is_contraction = is_contraction
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         **kwargs: Dict[str, Any],
     ) -> Series:
         _, coordinates = TwitchWidth.calculate_twitch_widths(
             filtered_data=filtered_data,
             twitch_indices=twitch_indices,
-            twitch_width_percents=tuple(self.twitch_width_percents),
+            twitch_width_percents=self.baseline_widths,
             rounded=self.rounded,
         )
 
         velocities = self.calculate_twitch_velocity(
             coordinate_df=coordinates, is_contraction=self.is_contraction
         )
 
@@ -427,35 +437,31 @@
                 twitch contraction or relaxation
 
         Returns:
             DataFrame floats that are the velocities of each twitch
         """
         coord_type = "contraction" if is_contraction else "relaxation"
 
-        twitch_base = self.twitch_width_percents[self.velocity_index_end]
-        twitch_top = self.twitch_width_percents[self.velocity_index_start]
-
-        Y_end = coordinate_df["force", coord_type, twitch_top]
-        Y_start = coordinate_df["force", coord_type, twitch_base]
+        Y_end = coordinate_df["force", coord_type, self.velocity_start]
+        Y_start = coordinate_df["force", coord_type, self.velocity_end]
 
-        X_end = coordinate_df["time", coord_type, twitch_top]
-        X_start = coordinate_df["time", coord_type, twitch_base]
+        X_end = coordinate_df["time", coord_type, self.velocity_start]
+        X_start = coordinate_df["time", coord_type, self.velocity_end]
 
         # change in force / change in time
         velocity = abs((Y_end - Y_start) / (X_end - X_start))
         velocity *= MICRO_TO_BASE_CONVERSION
 
         return velocity
 
 
 class TwitchIrregularity(BaseMetric):
     """Calculate irregularity of each twitch."""
 
     def __init__(self, rounded: bool = False, **kwargs: Dict[str, Any]):
-
         super().__init__(rounded=rounded, **kwargs)
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
@@ -513,46 +519,49 @@
 
 class TwitchAUC(BaseMetric):
     """Calculate area under each twitch."""
 
     def __init__(
         self,
         rounded: bool = False,
-        twitch_width_percents: Tuple[int, ...] = DEFAULT_TWITCH_WIDTH_PERCENTS,
+        baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
         **kwargs: Dict[str, Any],
     ):
-
         super().__init__(rounded=rounded, **kwargs)
-
-        self.twitch_width_percents = twitch_width_percents
+        # C10 in the metric definition diagram is the C point at 90% twitch width
+        self.baseline_widths = [100 - baseline_widths_to_use[0], baseline_widths_to_use[1]]
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         **kwargs: Dict[str, Any],
     ) -> Series:
         _, coordinates = TwitchWidth.calculate_twitch_widths(
             filtered_data=filtered_data,
             twitch_indices=twitch_indices,
-            twitch_width_percents=tuple(self.twitch_width_percents),
+            twitch_width_percents=tuple(self.baseline_widths),
             rounded=self.rounded,
         )
 
         auc = self.calculate_area_under_curve(
-            twitch_indices=twitch_indices, filtered_data=filtered_data, coordinate_df=coordinates
+            twitch_indices=twitch_indices,
+            filtered_data=filtered_data,
+            coordinate_df=coordinates,
+            baseline_widths=tuple(self.baseline_widths),
         )
         return auc
 
     def calculate_area_under_curve(
         self,
         twitch_indices: Dict[int, Dict[UUID, Optional[int]]],
         filtered_data: NDArray[(2, Any), int],
         coordinate_df: DataFrame,
+        baseline_widths: Tuple[int, ...],
     ) -> Series:
         """Calculate the area under the curve (AUC) for twitches.
 
         Args:
             twitch_indices: a dictionary in which the key is an integer representing the time points
                 of all the peaks of interest and the value is an inner dictionary with various UUIDs
                 of prior/subsequent peaks and valleys and their index values.
@@ -561,26 +570,27 @@
                 data after it has gone through noise filtering and interpolation
 
             per_twitch_widths: a list of dictionaries where the first key is the percentage of the
                 way down to the nearby valleys, the second key is a UUID representing either the
                 value of the width, or the rising or falling coordinates. The final value is either
                 an int representing the width value or a tuple of ints for the x/y coordinates
 
+            baseline_widths: tuple twitch widths to use as baseline metrics
+
         Returns:
             Pandas Series of floats representing area under the curve for each twitch
         """
-        width_percent = 90  # what percent of repolarization to use as the bottom limit for calculating AUC
         estimates_dict: Dict[int, Union[int, float]] = dict()
 
         rising_x_values = coordinate_df["time"]["contraction"].T.to_dict()
         falling_x_values = coordinate_df["time"]["relaxation"].T.to_dict()
 
         for iter_twitch_peak_idx in twitch_indices.keys():
-            start_timepoint = rising_x_values[iter_twitch_peak_idx][width_percent]
-            stop_timepoint = falling_x_values[iter_twitch_peak_idx][width_percent]
+            start_timepoint = rising_x_values[iter_twitch_peak_idx][baseline_widths[0]]
+            stop_timepoint = falling_x_values[iter_twitch_peak_idx][baseline_widths[1]]
 
             auc_window_indices = get_time_window_indices(filtered_data[0], start_timepoint, stop_timepoint)
             auc_total = np.trapz(filtered_data[1, auc_window_indices], dx=INTERPOLATED_DATA_PERIOD_SECONDS)
 
             if self.rounded:
                 auc_total = int(round(auc_total, 0))
 
@@ -700,20 +710,15 @@
 
         time_difference = self.calculate_twitch_time_diff(
             twitch_indices, filtered_data, coordinate_df=coordinates, is_contraction=self.is_contraction
         )
 
         return time_difference
 
-    def add_aggregate_metrics(
-        self,
-        aggregate_df: DataFrame,
-        metric_id: UUID,
-        metrics: DataFrame,
-    ) -> None:
+    def add_aggregate_metrics(self, aggregate_df: DataFrame, metric_id: UUID, metrics: DataFrame) -> None:
         for iter_percent in self.twitch_width_percents:
             estimates = metrics[iter_percent]
             aggregate_estimates = self.create_statistics_df(estimates, rounded=self.rounded)
             try:
                 aggregate_df[metric_id, iter_percent] = aggregate_estimates
             except ValueError:
                 # Exception occurs when used for C10 to Peak and Peak to R90 metrics due to init df shape
@@ -764,15 +769,14 @@
         coords = coords.T.to_dict()
 
         def diff_fn(x, y):
             return x - y if is_contraction else y - x
 
         estimates_dict = {twitch_index: {} for twitch_index in twitch_indices.keys()}  # type: ignore
         for iter_twitch_idx in twitch_indices.keys():
-
             for iter_percent in self.twitch_width_percents:
                 percent = iter_percent
                 if is_contraction:
                     percent = 100 - percent
 
                 percent_time = coords[iter_twitch_idx][percent]
                 peak_time = filtered_data[0, iter_twitch_idx]
@@ -782,20 +786,15 @@
 
         return estimates / MICRO_TO_BASE_CONVERSION
 
 
 class TwitchPeakToBaseline(BaseMetric):
     """Calculate full contraction or full relaxation time."""
 
-    def __init__(
-        self,
-        rounded: bool = False,
-        is_contraction: bool = True,
-        **kwargs: Dict[str, Any],
-    ):
+    def __init__(self, rounded: bool = False, is_contraction: bool = True, **kwargs: Dict[str, Any]):
         super().__init__(rounded=rounded, **kwargs)
         self.is_contraction = is_contraction
 
     def fit(
         self,
         peak_and_valley_indices: Tuple[NDArray[int], NDArray[int]],
         filtered_data: NDArray[(2, Any), int],
@@ -818,18 +817,15 @@
         estimates = pd.Series(estimates_list, index=twitch_indices.keys()) / MICRO_TO_BASE_CONVERSION
         return estimates
 
 
 class WellGroupMetric(BaseMetric):
     """Calculate aggregrate group metrics."""
 
-    def __init__(
-        self,
-        **kwargs: Dict[str, Any],
-    ):
+    def __init__(self, **kwargs: Dict[str, Any]):
         super().__init__(False, **kwargs)
 
     def add_group_aggregate_metrics(
         self, aggregate_df: DataFrame, metric_column: Tuple, metrics: pd.Series, metric_type
     ) -> None:
         """Get aggregate metrics for entire well group.
```

### Comparing `Pulse3D-0.32.6/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.0/src/pulse3D/peak_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,38 +221,40 @@
         "twitch_indices": twitch_indices,
     }
 
     dfs = init_dfs(twitch_indices.keys(), twitch_widths_range=twitch_width_percents)
 
     # Kristian (10/26/21): dictionary of metric functions. this could probably be made cleaner at some point
     metric_mapper: Dict[UUID, BaseMetric] = {
-        AMPLITUDE_UUID: TwitchAmplitude(rounded=rounded),
-        AUC_UUID: TwitchAUC(rounded=rounded, twitch_width_percents=twitch_width_percents),
+        AMPLITUDE_UUID: TwitchAmplitude(rounded=rounded, baseline_widths_to_use=baseline_widths_to_use),
+        AUC_UUID: TwitchAUC(rounded=rounded, baseline_widths_to_use=baseline_widths_to_use),
         BASELINE_TO_PEAK_UUID: TwitchPeakTime(
             rounded=rounded,
             is_contraction=True,
             twitch_width_percents=(baseline_widths_to_use[0], 100 - baseline_widths_to_use[0]),
         ),
         CONTRACTION_TIME_UUID: TwitchPeakTime(
             rounded=rounded, is_contraction=True, twitch_width_percents=twitch_width_percents
         ),
         CONTRACTION_VELOCITY_UUID: TwitchVelocity(
-            rounded=rounded, is_contraction=True, twitch_width_percents=twitch_width_percents
+            rounded=rounded, is_contraction=True, baseline_widths_to_use=baseline_widths_to_use
         ),
-        FRACTION_MAX_UUID: TwitchFractionAmplitude(),
+        FRACTION_MAX_UUID: TwitchFractionAmplitude(baseline_widths_to_use=baseline_widths_to_use),
         IRREGULARITY_INTERVAL_UUID: TwitchIrregularity(rounded=rounded),
         PEAK_TO_BASELINE_UUID: TwitchPeakTime(
             rounded=rounded,
             is_contraction=False,
             twitch_width_percents=(baseline_widths_to_use[1], 100 - baseline_widths_to_use[1]),
         ),
         RELAXATION_TIME_UUID: TwitchPeakTime(
             rounded=rounded, is_contraction=False, twitch_width_percents=twitch_width_percents
         ),
-        RELAXATION_VELOCITY_UUID: TwitchVelocity(rounded=rounded, is_contraction=False),
+        RELAXATION_VELOCITY_UUID: TwitchVelocity(
+            rounded=rounded, is_contraction=False, baseline_widths_to_use=baseline_widths_to_use
+        ),
         TWITCH_FREQUENCY_UUID: TwitchFrequency(rounded=rounded),
         TWITCH_PERIOD_UUID: TwitchPeriod(rounded=rounded),
         WIDTH_UUID: TwitchWidth(rounded=rounded, twitch_width_percents=twitch_width_percents),
     }
 
     # add scalar metrics to corresponding DataFrames
     for metric_type, metrics in CALCULATED_METRICS.items():
```

### Comparing `Pulse3D-0.32.6/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.0/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/plotting.py` & `Pulse3D-0.33.0/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/stimulation.py` & `Pulse3D-0.33.0/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/transforms.py` & `Pulse3D-0.33.0/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.32.6/src/pulse3D/utils.py` & `Pulse3D-0.33.0/src/pulse3D/utils.py`

 * *Files identical despite different names*

