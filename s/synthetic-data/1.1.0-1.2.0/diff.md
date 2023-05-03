# Comparing `tmp/synthetic-data-1.1.0.tar.gz` & `tmp/synthetic-data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/brian/src/synthetic-data/dist/tmpxv91p354/synthetic-data-1.1.0.tar", last modified: Thu May  5 22:20:31 2022, max compression
+gzip compressed data, was "synthetic-data-1.2.0.tar", last modified: Wed May  3 18:26:15 2023, max compression
```

## Comparing `synthetic-data-1.1.0.tar` & `synthetic-data-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2022-05-05 22:20:31.648682 synthetic-data-1.1.0/
--rw-rw-r--   0 brian     (1000) brian     (1000)    11357 2022-04-09 18:01:06.000000 synthetic-data-1.1.0/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)     5305 2022-05-05 22:20:31.648682 synthetic-data-1.1.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     4891 2022-05-05 21:59:48.000000 synthetic-data-1.1.0/README.md
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2022-05-05 22:20:31.648682 synthetic-data-1.1.0/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1735 2022-05-05 22:20:25.000000 synthetic-data-1.1.0/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2022-05-05 22:20:31.648682 synthetic-data-1.1.0/synthetic_data/
--rw-rw-r--   0 brian     (1000) brian     (1000)        0 2022-04-09 18:01:06.000000 synthetic-data-1.1.0/synthetic_data/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2618 2022-05-05 21:59:48.000000 synthetic-data-1.1.0/synthetic_data/parser.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    13256 2022-05-05 21:59:48.000000 synthetic-data-1.1.0/synthetic_data/synthetic_data.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1112 2022-05-05 21:59:48.000000 synthetic-data-1.1.0/synthetic_data/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2022-05-05 22:20:31.648682 synthetic-data-1.1.0/synthetic_data.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)     5305 2022-05-05 22:20:31.000000 synthetic-data-1.1.0/synthetic_data.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      324 2022-05-05 22:20:31.000000 synthetic-data-1.1.0/synthetic_data.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2022-05-05 22:20:31.000000 synthetic-data-1.1.0/synthetic_data.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       50 2022-05-05 22:20:31.000000 synthetic-data-1.1.0/synthetic_data.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       15 2022-05-05 22:20:31.000000 synthetic-data-1.1.0/synthetic_data.egg-info/top_level.txt
+drwxr-xr-x   0 jnm703     (503) staff       (20)        0 2023-05-03 18:26:15.079460 synthetic-data-1.2.0/
+-rw-r--r--   0 jnm703     (503) staff       (20)    11357 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/LICENSE
+-rw-r--r--   0 jnm703     (503) staff       (20)     5274 2023-05-03 18:26:15.079281 synthetic-data-1.2.0/PKG-INFO
+-rw-r--r--   0 jnm703     (503) staff       (20)     4880 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/README.md
+-rw-r--r--   0 jnm703     (503) staff       (20)       38 2023-05-03 18:26:15.079512 synthetic-data-1.2.0/setup.cfg
+-rw-r--r--   0 jnm703     (503) staff       (20)     1626 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/setup.py
+drwxr-xr-x   0 jnm703     (503) staff       (20)        0 2023-05-03 18:26:15.075241 synthetic-data-1.2.0/synthetic_data/
+-rw-r--r--   0 jnm703     (503) staff       (20)        0 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/__init__.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     5433 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/graph_synthetic_data.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     4415 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/marginal_dist.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     2428 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/null_replication.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     2618 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/parser.py
+-rw-r--r--   0 jnm703     (503) staff       (20)    15769 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/synthetic_data.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     1112 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/synthetic_data/utils.py
+drwxr-xr-x   0 jnm703     (503) staff       (20)        0 2023-05-03 18:26:15.076709 synthetic-data-1.2.0/synthetic_data.egg-info/
+-rw-r--r--   0 jnm703     (503) staff       (20)     5274 2023-05-03 18:26:15.000000 synthetic-data-1.2.0/synthetic_data.egg-info/PKG-INFO
+-rw-r--r--   0 jnm703     (503) staff       (20)      642 2023-05-03 18:26:15.000000 synthetic-data-1.2.0/synthetic_data.egg-info/SOURCES.txt
+-rw-r--r--   0 jnm703     (503) staff       (20)        1 2023-05-03 18:26:15.000000 synthetic-data-1.2.0/synthetic_data.egg-info/dependency_links.txt
+-rw-r--r--   0 jnm703     (503) staff       (20)       65 2023-05-03 18:26:15.000000 synthetic-data-1.2.0/synthetic_data.egg-info/requires.txt
+-rw-r--r--   0 jnm703     (503) staff       (20)       15 2023-05-03 18:26:15.000000 synthetic-data-1.2.0/synthetic_data.egg-info/top_level.txt
+drwxr-xr-x   0 jnm703     (503) staff       (20)        0 2023-05-03 18:26:15.078978 synthetic-data-1.2.0/tests/
+-rw-r--r--   0 jnm703     (503) staff       (20)      479 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_cov_util.py
+-rw-r--r--   0 jnm703     (503) staff       (20)      828 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_distribution.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     3190 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_graph_synthetic.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     4604 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_marginal_dist.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     1800 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_noise.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     1808 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_null_replication.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     2885 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_redundant.py
+-rw-r--r--   0 jnm703     (503) staff       (20)     3246 2023-05-03 18:24:36.000000 synthetic-data-1.2.0/tests/test_synthetic_data.py
```

### Comparing `synthetic-data-1.1.0/LICENSE` & `synthetic-data-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthetic-data-1.1.0/PKG-INFO` & `synthetic-data-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: synthetic-data
-Version: 1.1.0
+Version: 1.2.0
 Summary: Generates complex, nonlinear datasets for use         with deep learning/black box models
 Home-page: https://github.com/capitalone/synthetic-data
 Maintainer: Brian Barr
 Maintainer-email: brian.barr@capitalone.com
 License: Apache License 2.0
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # synthetic-data
 Inspired by `sklearn.datasets.make_classification`, which in turn is based on work for the NIPS 2003 feature selection challenge [1] - targeting linear classifiers.  Here the focus is on generating more complex, nonlinear datasets appropriate for use with deep learning/black box models which 'need' nonlinearity - otherwise you would/should use a simpler model.
 
 
@@ -51,20 +50,20 @@
 ```
 
 ### Tests
 
 Test/Lint Dependencies
 
 ```bash
-$ pip install pandas pytest pytest-cov flake8
+pip install -r requirements-test.txt
 ```
 
 To run tests:
 ```bash
-$ make test_local
+make test_local
 ```
 
 ### Referencing this library
 If you use this library in your work, please cite our paper:  
 ```
 @inproceedings{barr:2020,
   author    = {Brian Barr and Ke Xu and Claudio Silva and Enrico Bertini and Robert Reilly and  C. Bayan Bruss and Jason D. Wittenbach},
@@ -84,9 +83,7 @@
 To run the examples, you should run:
 ```bash
 $ python -m pip install pandas pytest pytest-cov seaborn shap tensorflow "DataProfiler[full]"
 ```
 
 ### References
 [1] Guyon, “Design of experiments for the NIPS 2003 variable selection benchmark”, 2003.
-
-
```

### Comparing `synthetic-data-1.1.0/README.md` & `synthetic-data-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 ```
 
 ### Tests
 
 Test/Lint Dependencies
 
 ```bash
-$ pip install pandas pytest pytest-cov flake8
+pip install -r requirements-test.txt
 ```
 
 To run tests:
 ```bash
-$ make test_local
+make test_local
 ```
 
 ### Referencing this library
 If you use this library in your work, please cite our paper:  
 ```
 @inproceedings{barr:2020,
   author    = {Brian Barr and Ke Xu and Claudio Silva and Enrico Bertini and Robert Reilly and  C. Bayan Bruss and Jason D. Wittenbach},
```

### Comparing `synthetic-data-1.1.0/setup.py` & `synthetic-data-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,29 @@
 
 from setuptools import setup, find_packages
 
 
 def parse_requirements(filename):
     """Loads requirements file and outputs an array of dependencies"""
     lineiter = (line.strip() for line in open(filename))
-
     return [line for line in lineiter if line and not line.startswith('#')]
 
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='synthetic-data',
-    version='1.1.0',
+    version='1.2.0',
     maintainer='Brian Barr',
     maintainer_email='brian.barr@capitalone.com',
     license='Apache License 2.0',
     description='Generates complex, nonlinear datasets for use \
         with deep learning/black box models',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    #install_requires=parse_requirements('requirements.txt'),
-    install_requires=[
-        "numpy>=1.22.0rc1",
-        "scikit-learn==1.0.2",
-        "scipy==1.8.0"],
+    install_requires=parse_requirements('requirements.txt'),
     url='https://github.com/capitalone/synthetic-data',
     packages=find_packages(),
     include_package_data=True,
-    python_requires=">=3.6"
+    python_requires=">=3.8"
 )
```

### Comparing `synthetic-data-1.1.0/synthetic_data/parser.py` & `synthetic-data-1.2.0/synthetic_data/parser.py`

 * *Files identical despite different names*

### Comparing `synthetic-data-1.1.0/synthetic_data/synthetic_data.py` & `synthetic-data-1.2.0/synthetic_data/synthetic_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,37 +24,81 @@
 """
 
 import numpy as np
 import pandas as pd
 from scipy import stats
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import MinMaxScaler
+import scipy.interpolate as interpolate
 
+from synthetic_data.marginal_dist import detect_dist
+from synthetic_data.null_replication import replicate_null
 from synthetic_data.parser import MathParser
 
 
+def multinomial_ppf(x_uniform, my_dist, categories_info):
+    """
+    input:
+        x_uniform - uniform distribution random variable
+        my_dist - scipy.stats.multinomial object
+    output:
+        x_sampled - vector of samples from the multinomial
+    """
+    discrete_cdf = np.cumsum(my_dist.p)
+    #    print("pmf - ", my_dist.p)
+    #    print("cdf - ", discrete_cdf)
+    x_sampled = np.zeros_like(x_uniform)
+    # print(
+    #    "test uniformity - ",
+    #    x_uniform.min(),
+    #    x_uniform.max(),
+    #    x_uniform.mean(),
+    #    x_uniform.std(),
+    # )
+    # search discrete CDF
+    mapping_order = categories_info["mapping_order"]
+    category_mapping = categories_info["category_mapping"]
+    for j, x_u in enumerate(x_uniform):
+        if x_u <= discrete_cdf[0]:
+            x_sampled[j] = category_mapping[mapping_order[0]]
+        else:
+            for i, _ in enumerate(discrete_cdf[:-1]):
+                if (discrete_cdf[i] < x_u) and (x_u <= discrete_cdf[i + 1]):
+                    x_sampled[j] = category_mapping[mapping_order[i + 1]]
+                    break
+
+    return x_sampled
+
+
 def transform_to_distribution(x, adict):
     """
     Input:
         x - input uniform distributed random variable
         adict - dictionary corresponding to the desired distribution (name & params)
         e.g. {'col':[list], 'dist':'normal', 'kwargs':{'loc':0.0, 'scale':1.0, 'size'=n_samples}}
     Output:
         x_samples - the transformed vector with desired distribution
     """
 
-    if "args" not in adict.keys():
-        adict["args"] = {}
+    if "args" not in adict:
+        adict["args"] = []
 
-    if "kwargs" not in adict.keys():
+    if "kwargs" not in adict:
         adict["kwargs"] = {}
 
-    method_gen = getattr(stats, adict["dist"])
-    method_specific = method_gen(**adict["args"], **adict["kwargs"])
-    x_samples = method_specific.ppf(x)
+    # DP categoricals will be multinomial
+    if adict["dist"] in ["multinomial", "norm", "skewnorm"]:
+        method_gen = getattr(stats, adict["dist"])
+        method_specific = method_gen(*adict["args"], **adict["kwargs"])
+        if adict["dist"] == "multinomial":
+            x_samples = multinomial_ppf(x, method_specific, adict['categories_info'])
+        else:
+            x_samples = method_specific.ppf(x)
+    else:
+        x_samples = adict["args"].ppf(x)
 
     return x_samples
 
 
 def eval_expr_for_sample(x, col_map, expr):
     """
     Inputs:
@@ -134,17 +178,17 @@
     """
 
     if covariant is None:
         print("No covariant provided, generating one.")
         covariant = np.diag(np.ones(n_total))
 
     # test for symmetry on covariance matrix by comparing the matrix to its transpose
-    assert np.all(
-        covariant == covariant.T
-    ), "Assertion error - please check covariance matrix is symmetric."
+    np.testing.assert_almost_equal(
+        covariant, covariant.T, 1e-8
+        , "Assertion error - please check covariance matrix is symmetric.")
 
     return covariant
 
 
 def pre_data_generation_checks(n_informative, col_map, n_total):
     """This function is used to ensure input, and input combinations are correct before
     generating synthetic data
@@ -162,15 +206,14 @@
         n_total > 0
     ), "total number of samples (n_informative + n_nuisance) must be greater than 0"
 
 
 def generate_redundant_features(x, n_informative, n_redundant, seed):
     generator = np.random.RandomState(seed)
     B = 2 * generator.rand(n_informative, n_redundant) - 1
-    # B = 2 * random_state.rand(n_informative, n_redundant) - 1
     # print("in main script - b")
     # print(B)
     # print("in main script - x")
     # print(x)
     x_redundant = np.dot(x, B)
     # print("in synthetic_data - ")
     # print(x_redundant)
@@ -186,23 +229,36 @@
             and issubclass(scaler.__class__, TransformerMixin)
         )
         and scaler is not None
     ):
         raise TypeError("Please provide a valid sklearn scaler.")
 
 
+def marginal_dist_check(dist, num_cols):
+    """
+    Checks if dist argument passed to make_tabular_data is valid.
+    args:
+        dist - list of dicts for marginal distributions to apply to columns
+    """
+    if len(dist) != num_cols and len(dist) > 0:
+        raise ValueError(
+            "When providing a marginal distribution list, ensure the length of "
+            "the list is equal to n_informative columns."
+        )
+
+
 def make_tabular_data(
     n_samples=1000,
     n_informative=2,
     n_redundant=0,
     n_nuisance=0,
     n_classes=2,
-    dist=[],
+    dist=None,
     cov=None,
-    col_map={},
+    col_map=None,
     expr=None,
     sig_k=1.0,
     sig_x0=None,
     p_thresh=0.5,
     noise_level_x=0.0,
     noise_level_y=0.0,
     scaler=MinMaxScaler(feature_range=(-1, 1)),
@@ -222,60 +278,69 @@
             https://docs.scipy.org/doc/scipy/reference/stats.html
         cov - a symmetric matrix specifying covariance amongst features
         col_map - dictionary mapping str symbols to columns
         expr - str expression holding y = f(x)
         p_thresh - probability threshold for assigning class labels
         noise_level_x (float) - level of white noise (jitter) added to x
         noise_level_y (float) - level of white noise added to y (think flip_y)
-        scaler (sklearn scaler) - sklearn style scaler. Defaults to MinMaxScaler(feature_range = (-1,1)).
-                              If None, no feature scaling is performed.
+        scaler (sklearn scaler) - sklearn style scaler.
+            Defaults to MinMaxScaler(feature_range = (-1,1)).
+            If None, no feature scaling is performed.
         seed - numpy random state object for repeatability
 
 
 
 
     returns X: array of shape [n_samples, n_total] where n_total = n_inform + n_nuisance, etc.
             y: array of shape [n_samples] with our labels
             y_reg: array of shape [n_samples] with regression values which get split for labels
     """
+    if dist is None:
+        dist = []
 
     n_total = n_informative + n_redundant + n_nuisance
     x_final = np.zeros((n_samples, n_total))
 
     pre_data_generation_checks(
         n_informative=n_informative, col_map=col_map, n_total=n_total
     )
     scaler_check(scaler)
+    marginal_dist_check(dist, n_informative)
 
     # generate covariance matrix if not handed one
     cov = resolve_covariant(n_informative, covariant=cov)
 
     # initialize X array
     means = np.zeros(n_informative)
-    mvnorm = stats.multivariate_normal(mean=means, cov=cov)
+    # if coming from make_data_from_report - that data won't be standardized...
+
+    for i, a_dist in enumerate(dist):
+        if a_dist.get("mean") is not None:
+            means[i] = a_dist["mean"]
+
+    mvnorm = stats.multivariate_normal(mean=means, cov=cov, allow_singular=True)
     x = mvnorm.rvs(n_samples, random_state=seed)
-    # x_cont = np.zeros_like(x)
 
     # now tranform marginals back to uniform distribution
-    norm = stats.norm()
-    x_cont = norm.cdf(x)
+    x_cont = np.zeros_like(x)
+    for i in range(x.shape[1]):
+        x_tmp = x[:, i]
+        # print(i, x_tmp.mean(), x_tmp.std())
+        tmp_norm = stats.norm(loc=x_tmp.mean(), scale=x_tmp.std())
+        x_cont[:, i] = tmp_norm.cdf(x_tmp)
 
     # print("x_cont.shape - ", x.shape)
     # print("x_cont - ")
     # print(x_cont)
     # at this point x_cont has columns with correlation & uniform dist
 
     # apply marginal distributions
-
     for a_dist in dist:
         col = a_dist["column"]
-        # method = getattr(stats, a_dist["dist"])
-        # x_cont[:, col] = method.ppf(x_unif[:, col])
         x_cont[:, col] = transform_to_distribution(x_cont[:, col], a_dist)
-    # print(x_cont.max())
     x_final[:, :n_informative] = x_cont
 
     # add redundant - lines 224-228
     # https://github.com/scikit-learn/scikit-learn/blob/fd237278e/sklearn/datasets/_samples_generator.py#L37
 
     if n_redundant > 0:
         x_redundant = generate_redundant_features(
@@ -307,17 +372,15 @@
     y_labels = y_prob >= p_thresh
 
     #
     # post processing steps - e.g. add noise
     #
 
     if noise_level_x > 0.0:
-        x_noise = generate_x_noise(
-            x_final[:, :n_informative], noise_level_x, seed=seed
-        )
+        x_noise = generate_x_noise(x_final[:, :n_informative], noise_level_x, seed=seed)
         x_final[:, :n_informative] = x_final[:, :n_informative] + x_noise
 
     return x_final, y_reg, y_prob, y_labels
 
 
 def make_data_from_report(
     report: dict,
@@ -354,52 +417,50 @@
     # build covariance matrix
     R = report["global_stats"]["correlation_matrix"]
 
     stddevs = [stat["statistics"]["stddev"] for stat in report["data_stats"]]
     D = np.diag(stddevs)
 
     cov = D @ R @ D
-    cov = cov.round(decimals=8)  # round to avoid failing symmetry check
+    # cov = cov.round(decimals=8)  # round to avoid failing symmetry check
 
     # create col_map of appropriate length to pass pre_data_generation_checks
     col_map = {}
     for i in range(n_informative):
         col_map[f"x{i+1}"] = i
 
+    dist = detect_dist(report)
+
     x_final, _, _, _ = make_tabular_data(
         n_samples=n_samples,
         n_informative=n_informative,
         cov=cov,
         col_map=col_map,
         noise_level_x=noise_level,
         seed=seed,
+        dist=dist,
+        scaler=None,
     )
 
-    # generate scalers by range of values in original data
-    scalers = {}
-    for col, stat in enumerate(report["data_stats"]):
-        _min = stat["statistics"]["min"]
-        _max = stat["statistics"]["max"]
-        scalers[col] = MinMaxScaler(feature_range=(_min, _max))
-
-    # rescale to feature range
-    for col in scalers:
-        x_final[:, col] = (
-            scalers[col]
-            .fit_transform(x_final[:, col].reshape(-1, 1))
-            .flatten()
-        )
-
-    # find number of decimals for each column and round the data to match
-    precisions = [
-        stat["samples"][0][::-1].find(".") for stat in report["data_stats"]
-    ]
-
-    for i, precision in enumerate(precisions):
-        x_final[:, i] = np.around(
-            x_final[:, i], precision if precision > 0 else 0
-        )
+    # Approximate the original data format given its precision / # of digits
+    for i, col_stat in enumerate(report["data_stats"]):
+        digits = 0
+        if col_stat['data_type'] not in ['int', 'float']:
+            continue
+        if col_stat['data_type'] in ['float']:
+            precision = col_stat.get('statistics', {}).get('precision', {}).get('max', 0)
+            digits = precision - np.ceil(np.log10(np.abs(x_final[:, i])))
+            digits = int((digits[np.isfinite(digits)]).max())
+        x_final[:, i] = np.around(x_final[:, i], digits)
+
+    # replicate null values if null replication metrics exist in the original report
+    col_to_null_metrics = {}
+    for col_id, col_data_stats in enumerate(report["data_stats"]):
+        if "null_replication_metrics" not in col_data_stats:
+            continue
+        col_to_null_metrics[col_id] = col_data_stats["null_replication_metrics"]
+    x_final = replicate_null(x_final, col_to_null_metrics, cov)
 
     # return x_final in a DataFrame with the original column names
     return pd.DataFrame(
         x_final, columns=[stat["column_name"] for stat in report["data_stats"]]
     )
```

### Comparing `synthetic-data-1.1.0/synthetic_data/utils.py` & `synthetic-data-1.2.0/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `synthetic-data-1.1.0/synthetic_data.egg-info/PKG-INFO` & `synthetic-data-1.2.0/synthetic_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: synthetic-data
-Version: 1.1.0
+Version: 1.2.0
 Summary: Generates complex, nonlinear datasets for use         with deep learning/black box models
 Home-page: https://github.com/capitalone/synthetic-data
 Maintainer: Brian Barr
 Maintainer-email: brian.barr@capitalone.com
 License: Apache License 2.0
-Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # synthetic-data
 Inspired by `sklearn.datasets.make_classification`, which in turn is based on work for the NIPS 2003 feature selection challenge [1] - targeting linear classifiers.  Here the focus is on generating more complex, nonlinear datasets appropriate for use with deep learning/black box models which 'need' nonlinearity - otherwise you would/should use a simpler model.
 
 
@@ -51,20 +50,20 @@
 ```
 
 ### Tests
 
 Test/Lint Dependencies
 
 ```bash
-$ pip install pandas pytest pytest-cov flake8
+pip install -r requirements-test.txt
 ```
 
 To run tests:
 ```bash
-$ make test_local
+make test_local
 ```
 
 ### Referencing this library
 If you use this library in your work, please cite our paper:  
 ```
 @inproceedings{barr:2020,
   author    = {Brian Barr and Ke Xu and Claudio Silva and Enrico Bertini and Robert Reilly and  C. Bayan Bruss and Jason D. Wittenbach},
@@ -84,9 +83,7 @@
 To run the examples, you should run:
 ```bash
 $ python -m pip install pandas pytest pytest-cov seaborn shap tensorflow "DataProfiler[full]"
 ```
 
 ### References
 [1] Guyon, “Design of experiments for the NIPS 2003 variable selection benchmark”, 2003.
-
-
```

