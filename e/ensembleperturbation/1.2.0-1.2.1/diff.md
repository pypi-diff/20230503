# Comparing `tmp/ensembleperturbation-1.2.0.tar.gz` & `tmp/ensembleperturbation-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembleperturbation-1.2.0.tar", max compression
+gzip compressed data, was "ensembleperturbation-1.2.1.tar", max compression
```

## Comparing `ensembleperturbation-1.2.0.tar` & `ensembleperturbation-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     7048 2023-04-26 19:18:20.650799 ensembleperturbation-1.2.0/LICENSE
--rw-r--r--   0        0        0     1554 2023-04-26 19:18:20.650799 ensembleperturbation-1.2.0/README.md
--rw-r--r--   0        0        0        3 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/__init__.py
--rw-r--r--   0        0        0     3803 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/combine_results.py
--rw-r--r--   0        0        0     1952 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/make_storm_ensemble.py
--rw-r--r--   0        0        0     5792 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/perturb_tracks.py
--rw-r--r--   0        0        0     2566 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/client/plot_results.py
--rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/__init__.py
--rw-r--r--   0        0        0    32929 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/adcirc.py
--rw-r--r--   0        0        0    24828 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/comparison.py
--rw-r--r--   0        0        0    46714 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/schism.py
--rw-r--r--   0        0        0      545 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/parsing/utilities.py
--rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/perturbation/__init__.py
--rw-r--r--   0        0        0    74453 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/perturbation/atcf.py
--rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/__init__.py
--rw-r--r--   0        0        0    10510 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/gdal_dataset.py
--rw-r--r--   0        0        0     5453 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/geometry.py
--rw-r--r--   0        0        0     1590 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/map.py
--rw-r--r--   0        0        0     9135 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/nodes.py
--rw-r--r--   0        0        0    13796 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/perturbation.py
--rw-r--r--   0        0        0    20101 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/surrogate.py
--rw-r--r--   0        0        0     4623 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/taylor_diagram.py
--rw-r--r--   0        0        0      908 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/plotting/utilities.py
--rw-r--r--   0        0        0        0 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/__init__.py
--rw-r--r--   0        0        0     2663 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/ensemble_array.py
--rw-r--r--   0        0        0    11112 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
--rw-r--r--   0        0        0     5332 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
--rw-r--r--   0        0        0    23410 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/surrogate.py
--rw-r--r--   0        0        0     5066 2023-04-26 19:18:20.662799 ensembleperturbation-1.2.0/ensembleperturbation/utilities.py
--rw-r--r--   0        0        0     2310 2023-04-26 19:18:27.026868 ensembleperturbation-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3723 2023-04-26 19:18:27.933598 ensembleperturbation-1.2.0/setup.py
--rw-r--r--   0        0        0     3731 2023-04-26 19:18:27.934111 ensembleperturbation-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-03 16:37:41.880276 ensembleperturbation-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1554 2023-05-03 16:37:41.880276 ensembleperturbation-1.2.1/README.md
+-rw-r--r--   0        0        0        3 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/__init__.py
+-rw-r--r--   0        0        0     3803 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/combine_results.py
+-rw-r--r--   0        0        0     1952 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/make_storm_ensemble.py
+-rw-r--r--   0        0        0     5792 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/perturb_tracks.py
+-rw-r--r--   0        0        0     2566 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/client/plot_results.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/__init__.py
+-rw-r--r--   0        0        0    32929 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/adcirc.py
+-rw-r--r--   0        0        0    24828 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/comparison.py
+-rw-r--r--   0        0        0    46714 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/schism.py
+-rw-r--r--   0        0        0      545 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/parsing/utilities.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/perturbation/__init__.py
+-rw-r--r--   0        0        0    74561 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/perturbation/atcf.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/__init__.py
+-rw-r--r--   0        0        0    10510 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/gdal_dataset.py
+-rw-r--r--   0        0        0     5453 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/geometry.py
+-rw-r--r--   0        0        0     1590 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/map.py
+-rw-r--r--   0        0        0     9135 2023-05-03 16:37:41.892277 ensembleperturbation-1.2.1/ensembleperturbation/plotting/nodes.py
+-rw-r--r--   0        0        0    13796 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/perturbation.py
+-rw-r--r--   0        0        0    20101 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/surrogate.py
+-rw-r--r--   0        0        0     4623 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/taylor_diagram.py
+-rw-r--r--   0        0        0      908 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/plotting/utilities.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/__init__.py
+-rw-r--r--   0        0        0     2663 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/ensemble_array.py
+-rw-r--r--   0        0        0    11112 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
+-rw-r--r--   0        0        0     5332 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
+-rw-r--r--   0        0        0    23410 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/surrogate.py
+-rw-r--r--   0        0        0     5066 2023-05-03 16:37:41.896278 ensembleperturbation-1.2.1/ensembleperturbation/utilities.py
+-rw-r--r--   0        0        0     2310 2023-05-03 16:37:48.808743 ensembleperturbation-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3723 2023-05-03 16:37:49.861170 ensembleperturbation-1.2.1/setup.py
+-rw-r--r--   0        0        0     3731 2023-05-03 16:37:49.861724 ensembleperturbation-1.2.1/PKG-INFO
```

### Comparing `ensembleperturbation-1.2.0/LICENSE` & `ensembleperturbation-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/README.md` & `ensembleperturbation-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/client/combine_results.py` & `ensembleperturbation-1.2.1/ensembleperturbation/client/combine_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/client/make_storm_ensemble.py` & `ensembleperturbation-1.2.1/ensembleperturbation/client/make_storm_ensemble.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/client/perturb_tracks.py` & `ensembleperturbation-1.2.1/ensembleperturbation/client/perturb_tracks.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/client/plot_results.py` & `ensembleperturbation-1.2.1/ensembleperturbation/client/plot_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/parsing/adcirc.py` & `ensembleperturbation-1.2.1/ensembleperturbation/parsing/adcirc.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/parsing/comparison.py` & `ensembleperturbation-1.2.1/ensembleperturbation/parsing/comparison.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/parsing/schism.py` & `ensembleperturbation-1.2.1/ensembleperturbation/parsing/schism.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/parsing/utilities.py` & `ensembleperturbation-1.2.1/ensembleperturbation/parsing/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/perturbation/atcf.py` & `ensembleperturbation-1.2.1/ensembleperturbation/perturbation/atcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
             values *= self.unit
 
         all_values = variable_values - values
         # ensure that we don't change zero values
         all_values[variable_values.magnitude < 1] = 0 * all_values.units
         vortex_dataframe[self.name] = [
             min(self.upper_bound, max(value, self.lower_bound)).magnitude
-            if value.magnitude >= 1
+            if value.magnitude != 0
             else 0
             for value in all_values
         ] * self.unit
 
         return vortex_dataframe
 
     def storm_errors(self, data_frame: DataFrame, loc_index: int = 0) -> DataFrame:
@@ -1916,15 +1916,19 @@
 
     if storm is None:
         storm = directory / 'original.22'
 
     try:
         if Path(storm).exists():
             perturber = VortexPerturber.from_file(
-                storm, start_date=start_date, end_date=end_date,
+                storm,
+                start_date=start_date,
+                end_date=end_date,
+                file_deck=file_deck,
+                advisories=advisories,
             )
         else:
             raise FileNotFoundError
     except:
         if storm is None:
             raise ValueError('no storm ID specified')
```

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/gdal_dataset.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/geometry.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/geometry.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/map.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/map.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/nodes.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/nodes.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/perturbation.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/perturbation.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/surrogate.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/taylor_diagram.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/taylor_diagram.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/plotting/utilities.py` & `ensembleperturbation-1.2.1/ensembleperturbation/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/ensemble_array.py` & `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/ensemble_array.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py` & `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py` & `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/uncertainty_quantification/surrogate.py` & `ensembleperturbation-1.2.1/ensembleperturbation/uncertainty_quantification/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/ensembleperturbation/utilities.py` & `ensembleperturbation-1.2.1/ensembleperturbation/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.0/pyproject.toml` & `ensembleperturbation-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'ensembleperturbation'
-version = "1.2.0"
+version = "1.2.1"
 description = 'perturbation of coupled model input over a space of input variables'
 authors = ['Zach Burnett <zachary.burnett@noaa.gov>']
 license = 'CC0-1.0'
 readme = 'README.md'
 repository = 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git'
 documentation = 'https://ensembleperturbation.readthedocs.io'
```

### Comparing `ensembleperturbation-1.2.0/setup.py` & `ensembleperturbation-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                      'perturb_tracks = '
                      'ensembleperturbation.client.perturb_tracks:main',
                      'plot_results = '
                      'ensembleperturbation.client.plot_results:main']}
 
 setup_kwargs = {
     'name': 'ensembleperturbation',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'perturbation of coupled model input over a space of input variables',
     'long_description': '# Ensemble Perturbation\n\n[![tests](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/tests/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Atests)\n[![codecov](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation/branch/main/graph/badge.svg?token=4DwZePHp18)](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation)\n[![build](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/build/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Abuild)\n[![version](https://img.shields.io/pypi/v/EnsemblePerturbation)](https://pypi.org/project/EnsemblePerturbation)\n[![license](https://img.shields.io/github/license/noaa-ocs-modeling/EnsemblePerturbation)](https://creativecommons.org/share-your-work/public-domain/cc0)\n[![style](https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw)](https://sourceforge.net/p/oitnb/code)\n[![documentation](https://readthedocs.org/projects/ensembleperturbation/badge/?version=latest)](https://ensembleperturbation.readthedocs.io/en/latest/?badge=latest)\n\nPython library for perturbing coupled model inputs into ensemble runs. Provides\nperturbation and results comparison.\n\n```bash\npip install ensembleperturbation\n```\n\nDocumentation can be found at https://ensembleperturbation.readthedocs.io\n\n## Command-line interface\n\n`ensembleperturbation` exposes the following CLI commands:\n\n- `make_storm_ensemble`\n- `perturb_tracks`\n- `combine_results`\n- `plot_results`\n',
     'author': 'Zach Burnett',
     'author_email': 'zachary.burnett@noaa.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git',
```

### Comparing `ensembleperturbation-1.2.0/PKG-INFO` & `ensembleperturbation-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembleperturbation
-Version: 1.2.0
+Version: 1.2.1
 Summary: perturbation of coupled model input over a space of input variables
 Home-page: https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 License: CC0-1.0
 Author: Zach Burnett
 Author-email: zachary.burnett@noaa.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

