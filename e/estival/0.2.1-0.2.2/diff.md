# Comparing `tmp/estival-0.2.1.tar.gz` & `tmp/estival-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.2.1.tar", max compression
+gzip compressed data, was "estival-0.2.2.tar", max compression
```

## Comparing `estival-0.2.1.tar` & `estival-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3010 2023-04-04 20:46:52.692604 estival-0.2.1/estival/calibration/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.1/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
--rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.1/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
--rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.1/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
--rw-r--r--   0        0        0    23292 2023-03-09 20:46:38.954745 estival-0.2.1/estival/calibration/mcmc/adaptive.py
--rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.1/estival/calibration/mcmc/covariance.py
--rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.1/estival/calibration/mcmc/transformations.py
--rw-r--r--   0        0        0     2665 2023-04-04 20:12:53.083034 estival-0.2.1/estival/calibration/pymc.py
--rw-r--r--   0        0        0     2394 2023-03-31 04:30:11.423321 estival-0.2.1/estival/model.py
--rw-r--r--   0        0        0     2194 2023-04-04 00:33:00.496685 estival-0.2.1/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     2401 2023-04-04 00:32:27.557819 estival-0.2.1/estival/optimization/nevergrad.py
--rw-r--r--   0        0        0     3801 2023-04-04 20:15:44.189728 estival-0.2.1/estival/priors.py
--rw-r--r--   0        0        0     8661 2023-03-31 23:16:53.300530 estival-0.2.1/estival/targets.py
--rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.1/estival/utils.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.1/LICENSE
--rw-r--r--   0        0        0      967 2023-04-05 00:37:01.357774 estival-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      236 2022-11-20 23:56:33.174170 estival-0.2.1/README.md
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 estival-0.2.1/setup.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 estival-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3010 2023-04-04 20:46:52.692604 estival-0.2.2/estival/calibration/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.2/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
+-rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.2/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
+-rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.2/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
+-rw-r--r--   0        0        0    23292 2023-03-09 20:46:38.954745 estival-0.2.2/estival/calibration/mcmc/adaptive.py
+-rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.2/estival/calibration/mcmc/covariance.py
+-rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.2/estival/calibration/mcmc/transformations.py
+-rw-r--r--   0        0        0     2665 2023-04-04 20:12:53.083034 estival-0.2.2/estival/calibration/pymc.py
+-rw-r--r--   0        0        0     2607 2023-05-03 04:10:46.170333 estival-0.2.2/estival/model.py
+-rw-r--r--   0        0        0     2194 2023-04-04 00:33:00.496685 estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     4492 2023-05-03 03:19:27.593270 estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
+-rw-r--r--   0        0        0     2627 2023-05-03 04:11:25.401575 estival-0.2.2/estival/optimization/nevergrad.py
+-rw-r--r--   0        0        0     3801 2023-04-04 20:15:44.189728 estival-0.2.2/estival/priors.py
+-rw-r--r--   0        0        0    10505 2023-05-03 04:13:24.998335 estival-0.2.2/estival/targets.py
+-rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.2/estival/utils.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.2/LICENSE
+-rw-r--r--   0        0        0      967 2023-05-03 04:15:13.046878 estival-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      236 2022-11-20 23:56:33.174170 estival-0.2.2/README.md
+-rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 estival-0.2.2/PKG-INFO
```

### Comparing `estival-0.2.1/estival/calibration/__pycache__/pymc.cpython-310.pyc` & `estival-0.2.2/estival/calibration/__pycache__/pymc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc` & `estival-0.2.2/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc` & `estival-0.2.2/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc` & `estival-0.2.2/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/mcmc/adaptive.py` & `estival-0.2.2/estival/calibration/mcmc/adaptive.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/mcmc/covariance.py` & `estival-0.2.2/estival/calibration/mcmc/covariance.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/mcmc/transformations.py` & `estival-0.2.2/estival/calibration/mcmc/transformations.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/calibration/pymc.py` & `estival-0.2.2/estival/calibration/pymc.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/model.py` & `estival-0.2.2/estival/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,91 @@
-from typing import List
-from dataclasses import dataclass
-
-from summer2 import CompartmentalModel
-
-from jax import jit
-
-import pandas as pd
-
-class BayesianCompartmentalModel:
-    def __init__(self, model: CompartmentalModel, parameters: dict, priors: list, targets: list, extra_ll=None):
-        self.model = model
-        self.parameters = parameters
-        self.targets = {t.name:t for t in targets}
-        
-        for t in targets:
-            priors = priors + t.get_priors()
-        self.priors = {p.name:p for p in priors}
-        
-        self.loglikelihood = self._build_logll_func(extra_ll)
-        
-        self._ref_idx = self.model._get_ref_idx()
-        
-    def _build_logll_func(self, extra_ll=None):
-        model_params = self.model.get_input_parameters()
-        dyn_params = list(model_params.intersection(set(self.priors)))
-        self.model.set_derived_outputs_whitelist(list(self.targets))
-        
-        ll_runner = self.model.get_runner(self.parameters, dyn_params)
-        
-        self.model.set_derived_outputs_whitelist([])
-        self._full_runner = self.model.get_runner(self.parameters, dyn_params)
-        
-        tidx = pd.Index(self.model.times)
-
-        evaluators = {}
-        for k, t in self.targets.items():
-            evaluators[k] = t.get_evaluator(tidx)
-
-        @jit
-        def logll(**kwargs):
-            dict_args = capture_model_kwargs(self.model, **kwargs)
-            res = ll_runner._run_func(dict_args)["derived_outputs"]
-
-            logdens = 0.0
-            for tk, te in evaluators.items():
-                modelled = res[tk]
-                logdens += te.evaluate(modelled, kwargs)
-
-            if extra_ll:
-                logdens += extra_ll(kwargs)
-            
-            return logdens
-
-        return logll
-    
-    def run(self, parameters):
-        results = self._full_runner._run_func(parameters)
-        return ResultsData(derived_outputs=pd.DataFrame(results["derived_outputs"],index=self._ref_idx))
-    
-    def run_jax(self, parameters):
-        return self._full_runner._run_func(parameters)
-
-
-@dataclass
-class ResultsData:
-    derived_outputs: pd.DataFrame
-
-def capture_model_kwargs(model: CompartmentalModel, **kwargs) -> dict:
-    model_params = model.get_input_parameters()
-    return {k: kwargs[k] for k in kwargs if k in model_params}
+from typing import List
+from dataclasses import dataclass
+
+from summer2 import CompartmentalModel
+
+from jax import jit
+
+import pandas as pd
+
+
+class BayesianCompartmentalModel:
+    def __init__(
+        self,
+        model: CompartmentalModel,
+        parameters: dict,
+        priors: list,
+        targets: list,
+        extra_ll=None,
+    ):
+        self.model = model
+        self.parameters = parameters
+        self.targets = {t.name: t for t in targets}
+
+        for t in targets:
+            priors = priors + t.get_priors()
+        self.priors = {p.name: p for p in priors}
+
+        self.loglikelihood = self._build_logll_func(extra_ll)
+
+        self._ref_idx = self.model._get_ref_idx()
+
+    def _build_logll_func(self, extra_ll=None):
+        model_params = self.model.get_input_parameters()
+        dyn_params = list(model_params.intersection(set(self.priors)))
+        self.model.set_derived_outputs_whitelist(list(self.targets))
+
+        ll_runner = self.model.get_runner(self.parameters, dyn_params)
+
+        self.model.set_derived_outputs_whitelist([])
+        self._full_runner = self.model.get_runner(self.parameters, dyn_params)
+
+        tidx = pd.Index(self.model.times)
+
+        evaluators = {}
+        for k, t in self.targets.items():
+            evaluators[k] = t.get_evaluator(tidx)
+
+        @jit
+        def logll(**kwargs):
+            dict_args = capture_model_kwargs(self.model, **kwargs)
+            res = ll_runner._run_func(dict_args)["derived_outputs"]
+
+            logdens = 0.0
+            for tk, te in evaluators.items():
+                modelled = res[tk]
+                logdens += te.evaluate(modelled, kwargs)
+
+            if extra_ll:
+                logdens += extra_ll(kwargs)
+
+            return logdens
+
+        return logll
+
+    def logprior(self, **parameters):
+        lp = 0.0
+        for k, p in self.priors.items():
+            lp += p.logpdf(parameters[k])
+        return lp
+
+    def logposterior(self, **parameters):
+        return self.loglikelihood(**parameters) + self.logprior(**parameters)
+
+    def run(self, parameters):
+        results = self._full_runner._run_func(parameters)
+        return ResultsData(
+            derived_outputs=pd.DataFrame(results["derived_outputs"], index=self._ref_idx)
+        )
+
+    def run_jax(self, parameters):
+        return self._full_runner._run_func(parameters)
+
+
+@dataclass
+class ResultsData:
+    derived_outputs: pd.DataFrame
+
+
+def capture_model_kwargs(model: CompartmentalModel, **kwargs) -> dict:
+    model_params = model.get_input_parameters()
+    return {k: kwargs[k] for k in kwargs if k in model_params}
```

### Comparing `estival-0.2.1/estival/optimization/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.2.2/estival/optimization/__pycache__/nevergrad.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/priors.py` & `estival-0.2.2/estival/priors.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/estival/targets.py` & `estival-0.2.2/estival/targets.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,54 +8,55 @@
 import numpy as np
 
 from jax import jit, scipy as jsp, numpy as jnp
 
 from .priors import DistriParam, BasePrior
 
 
-
-
 class BaseTarget(ABC):
-
     name: str
     data: pd.Series
     _data_attrs: List = []
 
-    def __init__(self, name: str, data: pd.Series, time_weights: pd.Series = None):
+    def __init__(
+        self, name: str, data: pd.Series, weight: float = 1.0, time_weights: pd.Series = None
+    ):
         # Make things easier for calibration by sanitizing the data here
         self.name = name
         self.data = data
 
         # Should do some validation on this - ie make sure indices match data
-        #if time_weights is None:
+        # if time_weights is None:
         #    time_weights = pd.Series(index=data.index, data=np.repeat(1.0 / len(data), len(data)))
 
         self.time_weights = time_weights
+        self.weight = weight
 
     def get_priors(self):
         return []
 
     def filtered(self, index: pd.Index) -> BaseTarget:
         out_target = copy(self)
         valid_idx = index.intersection(self.data.index)
         out_target.data = out_target.data[valid_idx]
-        
+
         for da in self._data_attrs:
             data = getattr(out_target, da)
             setattr(out_target, da, data[valid_idx])
 
         if self.time_weights is not None:
             new_time_weights = out_target.time_weights[valid_idx]
             out_target.time_weights = new_time_weights / new_time_weights.sum()
         return out_target
 
     @abstractmethod
     def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
         raise NotImplementedError()
 
+
 class TargetEvaluator(ABC):
     def __init__(self, target: BaseTarget, model_times: pd.Index):
         self.target = target.filtered(model_times)
         self.data = self.target.data.to_numpy()
         for da in target._data_attrs:
             data = getattr(self.target, da)
             setattr(self, da, data.to_numpy())
@@ -84,35 +85,36 @@
         mu = modelled[self.index]
         # work out parameter p to match the distribution mean with the model output
         p = mu / (mu + n)
         # Attempt to minimize -inf showing up
         p = jnp.where(p == 0.0, 1e-16, p)
         # ll = np.sum(stats.nbinom.logpmf(self.data, n, 1.0 - p) * self.time_weights)
         ll = jsp.stats.nbinom.logpmf(self.data, n, 1.0 - p)
-        
+
         if self.time_weights is not None:
             ll = ll * self.time_weights
-            return jnp.sum(ll)
+            return jnp.sum(ll) * self.target.weight
         else:
-            return jnp.mean(ll)
+            return jnp.mean(ll) * self.target.weight
 
 
 class NegativeBinomialTarget(BaseTarget):
     """
     A calibration target sampled from a negative binomial distribution
     """
 
     def __init__(
         self,
         name: str,
         data: pd.Series,
         dispersion_param: DistriParam,
+        weight: float = 1.0,
         time_weights: pd.Series = None,
     ):
-        super().__init__(name, data, time_weights)
+        super().__init__(name, data, weight, time_weights)
         self.dispersion_param = dispersion_param
 
     def get_priors(self):
         if isinstance(self.dispersion_param, BasePrior):
             return [self.dispersion_param]
         else:
             return []
@@ -127,73 +129,78 @@
     """
 
     def __init__(
         self,
         name: str,
         data: pd.Series,
         sample_sizes: pd.Series,
+        weight: float = 1.0,
         time_weights: pd.Series = None,
     ):
-        super().__init__(name, data, time_weights)
+        super().__init__(name, data, weight, time_weights)
         self._data_attrs = ["sample_sizes"]
         self.sample_sizes = sample_sizes
 
     def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
         return BinomialEvaluator(self, model_times)
 
+
 class BinomialEvaluator(TargetEvaluator):
     def __init__(self, target: BaseTarget, model_times: pd.Index):
         super().__init__(target, model_times)
         # Enforce this here so TFP-jax picks the right output types
         self.sample_sizes = self.sample_sizes.astype(float)
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         from tensorflow_probability.substrates import jax as tfp
+
         # use a binomial (n, p) where n is the sample size observed in the data and p the modelled proportion
         # We then evaluate the binomial density for k, which represents the numerator observed in the data
         n = self.target.sample_sizes
         p = modelled
-        k = self.target.data * n           
+        k = self.target.data * n
 
-        bdist = tfp.distributions.Binomial(total_count=n, probs = p)
+        bdist = tfp.distributions.Binomial(total_count=n, probs=p)
         ll = bdist.log_prob(k)
 
         if self.time_weights is not None:
             ll = ll * self.time_weights
-            return jnp.sum(ll)
+            return jnp.sum(ll) * self.target.weight
         else:
-            return jnp.mean(ll)
+            return jnp.mean(ll) * self.target.weight
+
 
 class TruncatedNormalTarget(BaseTarget):
     """
     A calibration target sampled from a truncated normal distribution
     """
 
     def __init__(
         self,
         name: str,
         data: pd.Series,
         trunc_range: Tuple[float, float],
         stdev: DistriParam,
+        weight: float = 1.0,
         time_weights: pd.Series = None,
     ):
-        super().__init__(name, data, time_weights)
+        super().__init__(name, data, weight, time_weights)
         self.trunc_range = trunc_range
         self.stdev = stdev
 
     def get_priors(self):
         if isinstance(self.stdev, BasePrior):
             return [self.stdev]
         else:
             return []
-        
+
     def get_evaluator(self, model_times: pd.Index) -> TargetEvaluator:
         return TruncatedNormalTargetEvaluator(self, model_times)
 
-        
+
 class TruncatedNormalTargetEvaluator(TargetEvaluator):
     def __init__(self, target: TruncatedNormalTarget, model_times: pd.Index):
         super().__init__(target, model_times)
 
     def evaluate(self, modelled: np.array, parameters: dict) -> float:
         if isinstance(self.target.stdev, BasePrior):
             sd = parameters[self.target.stdev.name]
@@ -206,28 +213,33 @@
             "b": (self.target.trunc_range[1] - self.data) / sd,
         }
 
         ll = jsp.stats.truncnorm.logpdf(modelled[self.index], loc=self.data, **distri_params)
 
         if self.time_weights is not None:
             ll = ll * self.time_weights
-            return jnp.sum(ll)
+            return jnp.sum(ll) * self.target.weight
         else:
-            return jnp.mean(ll)
+            return jnp.mean(ll) * self.target.weight
 
 
 class NormalTarget(BaseTarget):
     """
     A calibration target sampled from a normal distribution
     """
 
     def __init__(
-        self, name: str, data: pd.Series, stdev: DistriParam, time_weights: pd.Series = None
+        self,
+        name: str,
+        data: pd.Series,
+        stdev: DistriParam,
+        weight: float = 1.0,
+        time_weights: pd.Series = None,
     ):
-        super().__init__(name, data, time_weights)
+        super().__init__(name, data, weight, time_weights)
         self.stdev = stdev
 
     def get_priors(self):
         if isinstance(self.stdev, BasePrior):
             return [self.stdev]
         else:
             return []
@@ -246,17 +258,56 @@
         else:
             sd = self.target.stdev
 
         ll = jsp.stats.norm.logpdf(modelled[self.index], loc=self.data, scale=sd)
 
         if self.time_weights is not None:
             ll = ll * self.time_weights
-            return jnp.sum(ll)
+            return jnp.sum(ll) * self.target.weight
         else:
-            return jnp.mean(ll)
+            return jnp.mean(ll) * self.target.weight
+
+
+class CustomTargetEvaluator(TargetEvaluator):
+    def __init__(self, target, model_times, eval_func):
+        super().__init__(target, model_times)
+        self._eval_func = eval_func
+
+    def evaluate(self, modelled, parameters):
+        return (
+            self._eval_func(modelled[self.index], self.data, parameters, self.time_weights)
+            * self.target.weight
+        )
+
+
+class CustomTarget(BaseTarget):
+    def __init__(self, name, data, eval_func, weight=1.0, time_weights=None):
+        """Build a Target that uses a custom evaluation function.
+        Indexing and multiplication by weight factor is handled automatically,
+        but time_weights are not (see below)
+
+        For example:
+
+        def least_squares(modelled, obs, parameters, time_weights):
+            return (((modelled - obs) ** 2.0) * time_weights).sum()
+
+        CustomTarget("example", example_data, least_squares)
+
+        Args:
+            name: Name (key) of output to evaluate against
+            data: Series of data using same indexing conventions as model
+            eval_func: Callable as described above
+            weight (optional): Scales resulting output
+            time_weights (optional): Passed to eval_func - Series with index matching data
+        """
+        super().__init__(name, data, weight, time_weights)
+        self.eval_func = eval_func
+
+    def get_evaluator(self, model_times):
+        return CustomTargetEvaluator(self, model_times, self.eval_func)
 
 
 def get_target_sd(data: pd.Series) -> float:
     """Return a value such that the 95% CI of the associated normal distribution covers a width
        equivalent to 25% of the maximum value of the target.
 
     Args:
```

### Comparing `estival-0.2.1/estival/utils.py` & `estival-0.2.2/estival/utils.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/LICENSE` & `estival-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.2.1/pyproject.toml` & `estival-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
```

### Comparing `estival-0.2.1/PKG-INFO` & `estival-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: estival
-Version: 0.2.1
+Version: 0.2.2
 Summary: A set of calibration and probabilistic programming tools for use with summerepi2
 Home-page: https://github.com/monash-emu/estival
 License: BSD-2-Clause
 Keywords: calibration,optimization,bayesian,compartmental modelling,summerepi
 Author: David Shipman
 Author-email: dshipman@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arviz (>=0.12.1)
 Requires-Dist: nevergrad (>=0.6.0)
 Requires-Dist: numpy (>=1.20.3)
 Requires-Dist: pymc (>=5.2.0)
 Requires-Dist: scipy (>=1.7.3)
 Requires-Dist: summerepi2 (>=1.2.1)
 Project-URL: Documentation, https://github.com/monash-emu/estival
```

