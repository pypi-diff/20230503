# Comparing `tmp/pydts-0.7.1.tar.gz` & `tmp/pydts-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydts-0.7.1.tar", max compression
+gzip compressed data, was "pydts-0.7.2.tar", max compression
```

## Comparing `pydts-0.7.1.tar` & `pydts-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.1/LICENSE
--rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.1/README.md
--rw-r--r--   0        0        0     1418 2023-05-02 17:26:11.158571 pydts-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.1/src/pydts/.DS_Store
--rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.1/src/pydts/__init__.py
--rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.1/src/pydts/base_fitters.py
--rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.1/src/pydts/config.py
--rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.1/src/pydts/cross_validation.py
--rw-r--r--   0        0        0    15112 2023-05-02 16:52:14.563267 pydts-0.7.1/src/pydts/data_generation.py
--rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.1/src/pydts/datasets/.DS_Store
--rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.1/src/pydts/datasets/LOS_simulated_data.csv
--rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.1/src/pydts/evaluation.py
--rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.1/src/pydts/examples_utils/__init__.py
--rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.1/src/pydts/examples_utils/datasets.py
--rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.1/src/pydts/examples_utils/generate_simulations_data.py
--rw-r--r--   0        0        0    31389 2022-08-02 12:29:25.353387 pydts-0.7.1/src/pydts/examples_utils/plots.py
--rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.1/src/pydts/examples_utils/simulations_data_config.py
--rw-r--r--   0        0        0    31641 2023-05-02 17:17:43.984979 pydts-0.7.1/src/pydts/fitters.py
--rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.1/src/pydts/model_selection.py
--rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.1/src/pydts/utils.py
--rw-r--r--   0        0        0     3853 2023-05-02 17:54:37.406435 pydts-0.7.1/setup.py
--rw-r--r--   0        0        0     3981 2023-05-02 17:54:37.406734 pydts-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.2/README.md
+-rw-r--r--   0        0        0     1418 2023-05-03 10:43:02.017614 pydts-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.2/src/pydts/.DS_Store
+-rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.2/src/pydts/__init__.py
+-rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.2/src/pydts/base_fitters.py
+-rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.2/src/pydts/config.py
+-rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.2/src/pydts/cross_validation.py
+-rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.2/src/pydts/data_generation.py
+-rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.2/src/pydts/datasets/.DS_Store
+-rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.2/src/pydts/datasets/LOS_simulated_data.csv
+-rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.2/src/pydts/evaluation.py
+-rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.2/src/pydts/examples_utils/__init__.py
+-rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.2/src/pydts/examples_utils/datasets.py
+-rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.2/src/pydts/examples_utils/generate_simulations_data.py
+-rw-r--r--   0        0        0    31389 2022-08-02 12:29:25.353387 pydts-0.7.2/src/pydts/examples_utils/plots.py
+-rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.2/src/pydts/examples_utils/simulations_data_config.py
+-rw-r--r--   0        0        0    31641 2023-05-02 17:17:43.984979 pydts-0.7.2/src/pydts/fitters.py
+-rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.2/src/pydts/model_selection.py
+-rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.2/src/pydts/utils.py
+-rw-r--r--   0        0        0     3853 2023-05-03 10:44:09.186211 pydts-0.7.2/setup.py
+-rw-r--r--   0        0        0     3981 2023-05-03 10:44:09.186504 pydts-0.7.2/PKG-INFO
```

### Comparing `pydts-0.7.1/LICENSE` & `pydts-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/README.md` & `pydts-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/pyproject.toml` & `pydts-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydts"
-version = "0.7.1"
+version = "0.7.2"
 description = "Discrete time survival analysis with competing risks"
 authors = ["Tomer Meir <tomer1812@gmail.com>", "Rom Gutman <rom.gutman1@gmail.com>", "Malka Gorfine <malkago12@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/tomer1812/pydts"
 repository = "https://github.com/tomer1812/pydts"
 keywords = ["Discrete Time", "Time to Event" ,"Survival Analysis", "Competing Events"]
```

### Comparing `pydts-0.7.1/src/pydts/.DS_Store` & `pydts-0.7.2/src/pydts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/base_fitters.py` & `pydts-0.7.2/src/pydts/base_fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/cross_validation.py` & `pydts-0.7.2/src/pydts/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/data_generation.py` & `pydts-0.7.2/src/pydts/data_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         assert (administrative_censoring_prob >= 0), "Check the sum of prob_lof_at_t argument."
         assert (administrative_censoring_prob <= 1), "Check the sum of prob_lof_at_t argument."
 
         prob_lof_at_t = np.append(prob_lof_at_t, administrative_censoring_prob)
         sampled_df = pd.DataFrame(np.random.choice(a=self.times, size=len(observations_df), p=prob_lof_at_t),
                                   index=observations_df.index, columns=['C'])
         # No follow-up censoring, C=d+2 such that T wins when building X column:
-        sampled_df.loc[sampled_df['C'] == self.times[-1], 'C'] = self.d_times + 2
+        #sampled_df.loc[sampled_df['C'] == self.times[-1], 'C'] = self.d_times + 2
         if 'C' in observations_df.columns:
             observations_df.drop('C', axis=1, inplace=True)
         observations_df = pd.concat([observations_df, sampled_df], axis=1)
         return observations_df
 
     def sample_hazard_lof_censoring(self, observations_df: pd.DataFrame, censoring_hazard_coefs: dict,
                                     seed: Union[int, None] = None,
@@ -230,15 +230,15 @@
             covariates = [c for c in observations_df.columns if c not in ['X', 'T', 'C', 'J']]
         cov_df = observations_df[covariates]
         tmp_ets = EventTimesSampler(d_times=self.d_times, j_event_types=1)
         sampled_df = tmp_ets.sample_event_times(cov_df, censoring_hazard_coefs, seed=seed, covariates=covariates,
                                                 events=[0])
 
         # No follow-up censoring, C=d+2 such that T wins when building X column:
-        sampled_df.loc[sampled_df['J'] == 0, 'T'] = self.d_times + 2
+        #sampled_df.loc[sampled_df['J'] == 0, 'T'] = self.d_times + 2
         sampled_df = sampled_df[['T']]
         sampled_df.columns = ['C']
         if 'C' in observations_df.columns:
             observations_df.drop('C', axis=1, inplace=True)
         observations_df = pd.concat([observations_df, sampled_df], axis=1)
         return observations_df
```

### Comparing `pydts-0.7.1/src/pydts/datasets/.DS_Store` & `pydts-0.7.2/src/pydts/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/datasets/LOS_simulated_data.csv` & `pydts-0.7.2/src/pydts/datasets/LOS_simulated_data.csv`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/evaluation.py` & `pydts-0.7.2/src/pydts/evaluation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/examples_utils/generate_simulations_data.py` & `pydts-0.7.2/src/pydts/examples_utils/generate_simulations_data.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/examples_utils/plots.py` & `pydts-0.7.2/src/pydts/examples_utils/plots.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/examples_utils/simulations_data_config.py` & `pydts-0.7.2/src/pydts/examples_utils/simulations_data_config.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/fitters.py` & `pydts-0.7.2/src/pydts/fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/model_selection.py` & `pydts-0.7.2/src/pydts/model_selection.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/src/pydts/utils.py` & `pydts-0.7.2/src/pydts/utils.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.1/setup.py` & `pydts-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'statsmodels>=0.13.2,<0.14.0',
  'tqdm>=4.63.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'pydts',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'Discrete time survival analysis with competing risks',
     'long_description': "[![pypi version](https://img.shields.io/pypi/v/pydts)](https://pypi.org/project/pydts/)\n[![Tests](https://github.com/tomer1812/pydts/workflows/Tests/badge.svg)](https://github.com/tomer1812/pydts/actions?workflow=Tests)\n[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://tomer1812.github.io/pydts)\n[![codecov](https://codecov.io/gh/tomer1812/pydts/branch/main/graph/badge.svg)](https://codecov.io/gh/tomer1812/pydts)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6466158.svg)](https://doi.org/10.5281/zenodo.6466158)\n\n# Discrete Time Survival Analysis  \nA Python package for discrete-time survival data analysis with competing risks.\n\n![PyDTS](docs/icon.png)  \n\n[Tomer Meir](https://tomer1812.github.io/), [Rom Gutman](https://github.com/RomGutman), [Malka Gorfine](https://www.tau.ac.il/~gorfinem/) 2022\n\n[Documentation](https://tomer1812.github.io/pydts/)  \n\n## Installation\n```console\npip install pydts\n```\n\n## Quick Start\n\n```python\nfrom pydts.fitters import TwoStagesFitter\nfrom pydts.examples_utils.generate_simulations_data import generate_quick_start_df\n\npatients_df = generate_quick_start_df(n_patients=10000, n_cov=5, d_times=14, j_events=2, pid_col='pid', seed=0)\n\nfitter = TwoStagesFitter()\nfitter.fit(df=patients_df.drop(['C', 'T'], axis=1))\nfitter.print_summary()\n```\n\n## Examples\n1. [Usage Example](https://tomer1812.github.io/pydts/UsageExample-Intro/)\n2. [Hospital Length of Stay Simulation Example](https://tomer1812.github.io/pydts/SimulatedDataset/)\n\n## Citations\nIf you found PyDTS software useful to your research, please cite the papers:\n\n```bibtex\n@article{Meir_PyDTS_2022,\n    author = {Meir, Tomer and Gutman, Rom, and Gorfine, Malka},\n    doi = {10.48550/arXiv.2204.05731},\n    title = {{PyDTS: A Python Package for Discrete Time Survival Analysis with Competing Risks}},\n    url = {https://arxiv.org/abs/2204.05731},\n    year = {2022}\n}\n\n@article{Meir_Gorfine_DTSP_2023,\n    author = {Meir, Tomer and Gorfine, Malka},\n    doi = {10.48550/arXiv.2303.01186},\n    title = {{Discrete-time Competing-Risks Regression with or without Penalization}},\n    url = {https://arxiv.org/abs/2303.01186},\n    year = {2023}\n}\n```\n\nand please consider starring the project [on GitHub](https://github.com/tomer1812/pydts)\n\n## How to Contribute\n1. Open Github issues to suggest new features or to report bugs\\errors\n2. Contact Tomer or Rom if you want to add a usage example to the documentation \n3. If you want to become a developer (thank you, we appreciate it!) - please contact Tomer or Rom for developers' on-boarding \n\nTomer Meir: tomer1812@gmail.com, Rom Gutman: rom.gutman1@gmail.com",
     'author': 'Tomer Meir',
     'author_email': 'tomer1812@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/tomer1812/pydts',
```

### Comparing `pydts-0.7.1/PKG-INFO` & `pydts-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydts
-Version: 0.7.1
+Version: 0.7.2
 Summary: Discrete time survival analysis with competing risks
 Home-page: https://github.com/tomer1812/pydts
 License: GNU GPLv3
 Keywords: Discrete Time,Time to Event,Survival Analysis,Competing Events
 Author: Tomer Meir
 Author-email: tomer1812@gmail.com
 Requires-Python: >=3.8,<3.11
```

