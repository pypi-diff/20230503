# Comparing `tmp/summerepi-4.1.0a0.tar.gz` & `tmp/summerepi-4.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summerepi-4.1.0a0.tar", max compression
+gzip compressed data, was "summerepi-4.2.0a0.tar", max compression
```

## Comparing `summerepi-4.1.0a0.tar` & `summerepi-4.2.0a0.tar`

### file list

```diff
@@ -1,37 +1,33 @@
--rw-r--r--   0        0        0     1538 2021-03-29 22:36:34.645793 summerepi-4.1.0a0/LICENSE.txt
--rw-r--r--   0        0        0     1461 2022-08-10 02:15:18.188529 summerepi-4.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     5838 2022-08-10 02:15:07.891442 summerepi-4.1.0a0/README.md
--rw-r--r--   0        0        0      262 2022-08-02 01:31:58.473638 summerepi-4.1.0a0/summer/__init__.py
--rw-r--r--   0        0        0     4081 2022-08-10 01:41:47.737983 summerepi-4.1.0a0/summer/adjust.py
--rw-r--r--   0        0        0     4766 2022-08-01 02:59:00.358145 summerepi-4.1.0a0/summer/compartment.py
--rw-r--r--   0        0        0     3682 2021-08-10 01:09:22.062072 summerepi-4.1.0a0/summer/compute.py
--rw-r--r--   0        0        0    11644 2022-08-01 02:59:00.359145 summerepi-4.1.0a0/summer/derived_outputs.py
--rw-r--r--   0        0        0     2744 2022-08-09 07:05:19.505921 summerepi-4.1.0a0/summer/experimental/abstract_parameter.py
--rw-r--r--   0        0        0     8490 2022-08-10 00:59:06.362177 summerepi-4.1.0a0/summer/experimental/model_builder.py
--rw-r--r--   0        0        0    20355 2022-08-10 02:01:03.155039 summerepi-4.1.0a0/summer/flows.py
--rw-r--r--   0        0        0     4812 2022-08-01 02:59:00.360145 summerepi-4.1.0a0/summer/inspect.py
--rw-r--r--   0        0        0     1977 2022-08-02 01:31:39.985348 summerepi-4.1.0a0/summer/jaxify.py
--rw-r--r--   0        0        0    56753 2022-08-10 02:08:34.045046 summerepi-4.1.0a0/summer/model.py
--rw-r--r--   0        0        0       21 2022-08-01 02:59:00.371144 summerepi-4.1.0a0/summer/parameters/__init__.py
--rw-r--r--   0        0        0    12559 2022-08-10 02:11:25.495263 summerepi-4.1.0a0/summer/parameters/param_impl.py
--rw-r--r--   0        0        0     7966 2022-08-10 00:28:54.964404 summerepi-4.1.0a0/summer/parameters/params.py
--rw-r--r--   0        0        0     2609 2022-08-01 02:59:00.372645 summerepi-4.1.0a0/summer/population.py
--rw-r--r--   0        0        0       96 2021-08-10 01:09:22.064070 summerepi-4.1.0a0/summer/runner/__init__.py
--rw-r--r--   0        0        0      410 2022-08-01 02:59:00.373145 summerepi-4.1.0a0/summer/runner/jax/__init__.py
--rw-r--r--   0        0        0     5025 2022-08-09 04:33:31.399125 summerepi-4.1.0a0/summer/runner/jax/derived_outputs.py
--rw-r--r--   0        0        0    16540 2022-08-10 00:58:50.177963 summerepi-4.1.0a0/summer/runner/jax/model_impl.py
--rw-r--r--   0        0        0    11299 2022-08-01 04:08:11.240378 summerepi-4.1.0a0/summer/runner/jax/ode.py
--rw-r--r--   0        0        0     6491 2022-08-01 04:08:11.241378 summerepi-4.1.0a0/summer/runner/jax/runner.py
--rw-r--r--   0        0        0     1940 2022-08-02 01:53:47.180522 summerepi-4.1.0a0/summer/runner/jax/solvers.py
--rw-r--r--   0        0        0     4215 2022-08-09 04:06:57.564723 summerepi-4.1.0a0/summer/runner/jax/stratify.py
--rw-r--r--   0        0        0      947 2022-08-10 02:03:01.237720 summerepi-4.1.0a0/summer/runner/jax/util.py
--rw-r--r--   0        0        0    19319 2022-08-10 01:24:49.339298 summerepi-4.1.0a0/summer/runner/model_runner.py
--rw-r--r--   0        0        0     4312 2022-08-01 02:59:00.376145 summerepi-4.1.0a0/summer/runner/reference_runner.py
--rw-r--r--   0        0        0    17428 2022-08-01 04:08:11.246369 summerepi-4.1.0a0/summer/runner/vectorized_runner.py
--rw-r--r--   0        0        0     5973 2021-08-10 01:09:22.066567 summerepi-4.1.0a0/summer/solver.py
--rw-r--r--   0        0        0     6446 2021-05-06 00:36:31.254335 summerepi-4.1.0a0/summer/stochastic.py
--rw-r--r--   0        0        0    15833 2022-08-10 01:21:02.899034 summerepi-4.1.0a0/summer/stratification.py
--rw-r--r--   0        0        0      472 2022-08-01 02:59:00.378145 summerepi-4.1.0a0/summer/tracker.py
--rw-r--r--   0        0        0     1337 2021-08-11 20:34:46.933654 summerepi-4.1.0a0/summer/utils.py
--rw-r--r--   0        0        0     7112 2022-08-10 02:15:34.252656 summerepi-4.1.0a0/setup.py
--rw-r--r--   0        0        0     6969 2022-08-10 02:15:34.253156 summerepi-4.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1538 2021-03-29 22:36:34.645793 summerepi-4.2.0a0/LICENSE.txt
+-rw-r--r--   0        0        0     1462 2022-08-29 20:18:46.879161 summerepi-4.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5888 2022-08-29 20:19:36.859238 summerepi-4.2.0a0/README.md
+-rw-r--r--   0        0        0      203 2022-08-22 23:46:06.222019 summerepi-4.2.0a0/summer/__init__.py
+-rw-r--r--   0        0        0     4093 2022-08-26 02:42:24.810752 summerepi-4.2.0a0/summer/adjust.py
+-rw-r--r--   0        0        0     4782 2022-08-27 00:36:07.384668 summerepi-4.2.0a0/summer/compartment.py
+-rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi-4.2.0a0/summer/compute/__init__.py
+-rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi-4.2.0a0/summer/compute/compute_jax.py
+-rw-r--r--   0        0        0     2398 2022-08-27 21:19:57.120499 summerepi-4.2.0a0/summer/compute/compute_numba.py
+-rw-r--r--   0        0        0    11679 2022-08-26 00:29:04.327086 summerepi-4.2.0a0/summer/derived_outputs.py
+-rw-r--r--   0        0        0     8834 2022-08-24 08:55:58.556345 summerepi-4.2.0a0/summer/experimental/model_builder.py
+-rw-r--r--   0        0        0    19216 2022-08-27 00:53:23.198601 summerepi-4.2.0a0/summer/flows.py
+-rw-r--r--   0        0        0     5947 2022-08-27 20:41:23.307202 summerepi-4.2.0a0/summer/inspect.py
+-rw-r--r--   0        0        0    57811 2022-08-28 23:16:06.415353 summerepi-4.2.0a0/summer/model.py
+-rw-r--r--   0        0        0       21 2022-08-01 02:59:00.371144 summerepi-4.2.0a0/summer/parameters/__init__.py
+-rw-r--r--   0        0        0     9895 2022-08-25 06:21:26.013645 summerepi-4.2.0a0/summer/parameters/param_impl.py
+-rw-r--r--   0        0        0     4361 2022-08-26 03:11:32.457146 summerepi-4.2.0a0/summer/parameters/params.py
+-rw-r--r--   0        0        0     4770 2022-08-26 03:05:48.767753 summerepi-4.2.0a0/summer/population.py
+-rw-r--r--   0        0        0       40 2022-08-28 23:12:52.615804 summerepi-4.2.0a0/summer/runner/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-26 06:12:33.489045 summerepi-4.2.0a0/summer/runner/jax/__init__.py
+-rw-r--r--   0        0        0     5010 2022-08-22 23:30:40.889931 summerepi-4.2.0a0/summer/runner/jax/derived_outputs.py
+-rw-r--r--   0        0        0    15746 2022-08-28 23:13:15.564487 summerepi-4.2.0a0/summer/runner/jax/model_impl.py
+-rw-r--r--   0        0        0    11299 2022-08-22 19:53:53.633792 summerepi-4.2.0a0/summer/runner/jax/ode.py
+-rw-r--r--   0        0        0     1940 2022-08-22 19:53:53.635291 summerepi-4.2.0a0/summer/runner/jax/solvers.py
+-rw-r--r--   0        0        0     3997 2022-08-26 00:01:23.217242 summerepi-4.2.0a0/summer/runner/jax/stratify.py
+-rw-r--r--   0        0        0    23669 2022-08-29 00:31:31.008284 summerepi-4.2.0a0/summer/runner/model_runner.py
+-rw-r--r--   0        0        0     5973 2021-08-10 01:09:22.066567 summerepi-4.2.0a0/summer/solver.py
+-rw-r--r--   0        0        0     6446 2021-05-06 00:36:31.254335 summerepi-4.2.0a0/summer/stochastic.py
+-rw-r--r--   0        0        0    16223 2022-08-26 03:00:16.332668 summerepi-4.2.0a0/summer/stratification.py
+-rw-r--r--   0        0        0      472 2022-08-01 02:59:00.378145 summerepi-4.2.0a0/summer/tracker.py
+-rw-r--r--   0        0        0     1799 2022-08-26 02:30:41.406235 summerepi-4.2.0a0/summer/utils.py
+-rw-r--r--   0        0        0     7184 2022-08-29 20:21:38.299672 summerepi-4.2.0a0/setup.py
+-rw-r--r--   0        0        0     7020 2022-08-29 20:21:38.300171 summerepi-4.2.0a0/PKG-INFO
```

### Comparing `summerepi-4.1.0a0/LICENSE.txt` & `summerepi-4.2.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `summerepi-4.1.0a0/pyproject.toml` & `summerepi-4.2.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "summerepi"
-version = "4.1.0a"
+version = "4.2.0a"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "http://summerepi.com/"
 documentation = "http://summerepi.com/"
 repository = "https://github.com/monash-emu/summer"
 keywords = [
     "epidemiology",
@@ -21,15 +21,15 @@
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
 numpy = ">=1.20.3"
 networkx = ">=2.6.2"
 scipy = ">=1.7.1"
 numba = ">=0.54.0"
 pandas = ">=1.3.2"
-computegraph = ">=0.2.2"
+computegraph = ">=0.3.0b"
 jax =  [
     {extras = ["cpu"], version = "^0.3.14", platform = "linux"},
     {extras = ["cpu"], version = "^0.3.14", platform = "darwin"}
 ]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
```

### Comparing `summerepi-4.1.0a0/README.md` & `summerepi-4.2.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,16 @@
   - Bugfix and minor improvements search for parameters
 - 3.1.6
   - Support lists of adjustments and flow params
 - 4.0.0a
   - Full jax support with ModelBuilder wrapper
 - 4.1.0a
   - Abstract and lazy parameters
+- 4.2.0a
+  - Refactor parameters, combine runners
 
 ## Release process
 
 To do a release:
 
 - Commit any code changes and push them to GitHub
 - Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)
```

### Comparing `summerepi-4.1.0a0/summer/adjust.py` & `summerepi-4.2.0a0/summer/adjust.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # resolved_self = get_model_param_value(self.param, time, computed_values, parameters, True)
         if isinstance(self.param, ModelParameter):
             resolved_self = self.param.get_value(time, computed_values, parameters)
         elif callable(self.param):
             resolved_self = self.param(time, computed_values)
         else:
             resolved_self = self.param
-        resolved_input = get_static_param_value(value, parameters, True)
+        resolved_input = get_static_param_value(value, parameters, passthrough=True)
         return resolved_self * resolved_input
 
 
 class Overwrite(BaseAdjustment):
     """
     Am overwrite-based adjustment of a parameter.
     The new parameter value is the supplied parameter, overwriting any previous values.
```

### Comparing `summerepi-4.1.0a0/summer/compartment.py` & `summerepi-4.2.0a0/summer/compartment.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,22 @@
 
     """
 
     def __init__(
         self,
         name: str,
         strata: Optional[Dict[str, str]] = None,
-        tags: Optional[list] = None
+        idx: Optional[int] = None,
+        tags: Optional[list] = None,
     ):
         assert type(name) is str, "Name must be a string, not %s." % type(name)
         self.name = name
         self.strata = strata or {}
         self._str = self.serialize()
-        self.idx = None
+        self.idx = idx
         self._strata = frozenset(self.strata.items())
         self.tags = tags or []
 
     def is_match(self, name: str, strata: dict) -> bool:
         """
         Determines whether this compartment matches the supplied name and strata.
         A partial strata match, where this compartment has more strata than are supplied returns True.
@@ -89,18 +90,15 @@
             stratification_name: The name (or purpose) of the new stratification.
             stratum_name: The stratum to be assigned to the new Compartment.
         Returns:
             Compartment: The new, stratified compartment.
 
         """
         new_strata = {**self.strata, stratification_name: stratum_name}
-        return Compartment(
-            name=self.name,
-            strata=new_strata,
-        )
+        return Compartment(name=self.name, strata=new_strata, tags=self.tags)
 
     def serialize(self) -> str:
         """Returns a string representation of the compartment"""
         strata_strings = [f"{k}_{v}" for k, v in self.strata.items()]
         return "X".join([self.name, *strata_strings])
 
     @staticmethod
```

### Comparing `summerepi-4.1.0a0/summer/derived_outputs.py` & `summerepi-4.2.0a0/summer/derived_outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,29 @@
     COMPARTMENT = "comp"
     AGGREGATE = "agg"
     CUMULATIVE = "cum"
     FUNCTION = "func"
     COMPUTED_VALUE = "computed_value"
     PARAM_FUNCTION = "param_func"
 
+
 def calculate_derived_outputs(
     requests: List[dict],
     graph: networkx.DiGraph,
     outputs: np.ndarray,
     times: np.ndarray,
     timestep: float,
     flows: List[BaseFlow],
     compartments: List[Compartment],
     get_flow_rates: Callable[[np.ndarray, float], np.ndarray],
     model,
     whitelist: Optional[List[str]],
-    baseline = None,
-    idx_cache = None,
-    parameters: dict = None
+    baseline=None,
+    idx_cache=None,
+    parameters: dict = None,
 ) -> Dict[str, np.ndarray]:
     """
     Calculates all requested derived outputs from the calculated compartment sizes.
 
     Args:
         requests: Descriptions of the new outputs we should create.
         graph: A DAG describing how the requests depend on each other.
@@ -104,22 +105,24 @@
 
     # FIXME: Another question for Matt - has my changes to the time requests stuffed this up?
     # Because the timestep for the last time interval can now be different from the earlier ones.
     # So do we need to assert that the duration is an exact multiple of the timestep?
     # Could cause silent problems, because presumably we have previously been specifying durations as multiples of the timestep.
     for time_idx, time in enumerate(times):
         # Flow rates are instantaneous; we need to provide an integrated value over timestep
-        flow_rates = get_flow_rates(outputs[time_idx], time)
-        flow_values[time_idx, :] = flow_rates * timestep
+        flow_rates_t, computed_values_t = get_flow_rates(outputs[time_idx], time)
+        flow_values[time_idx, :] = flow_rates_t * timestep
         # Collect these as lists then build DataFrames afterwards
-        computed_values.append(model._backend._calc_computed_values(outputs[time_idx], time))
-    
+        computed_values.append(computed_values_t)
+
     # Collate list values into DataFrames
-    computed_values = pd.DataFrame(columns=model.get_computed_value_keys(), data = computed_values, index=times)
-    
+    computed_values = pd.DataFrame(
+        columns=model.get_computed_value_keys(), data=computed_values, index=times
+    )
+
     # Convert tracked flow values into a matrix where the 1st dimension is flow type, 2nd is time
     flow_values = np.array(flow_values).T
 
     # Calculate all the outputs in the correct order so that each output has its dependencies fulfilled.
     for name in networkx.topological_sort(graph):
         request = requests[name]
         request_type = request["request_type"]
@@ -127,18 +130,22 @@
 
         if not request["save_results"]:
             # Delete the results of this output once the calcs are done.
             outputs_to_delete_after.append(name)
 
         if request_type == DerivedOutputRequest.FLOW:
             # User wants to track a set of flow rates over time.
-            output, idx_cache = _get_flow_output(request, name, times, flows, flow_values, idx_cache)
+            output, idx_cache = _get_flow_output(
+                request, name, times, flows, flow_values, idx_cache
+            )
         elif request_type == DerivedOutputRequest.COMPARTMENT:
             # User wants to track a set of compartment sizes over time.
-            output, idx_cache = _get_compartment_output(request, name, outputs, compartments, idx_cache)
+            output, idx_cache = _get_compartment_output(
+                request, name, outputs, compartments, idx_cache
+            )
         elif request_type == DerivedOutputRequest.AGGREGATE:
             # User wants to track the sum of a set of outputs over time.
             output = _get_aggregate_output(request, derived_outputs)
         elif request_type == DerivedOutputRequest.CUMULATIVE:
             # User wants to track cumulative value of an output over time.
             if baseline:
                 baseline_offset = baseline.derived_outputs[name][baseline_start_index]
@@ -164,15 +171,15 @@
 
 
 def _get_flow_output(request, name, times, flows, flow_values, idx_cache=None):
     this_flow_values = np.zeros_like(times)
 
     if not idx_cache:
         idx_cache = {}
-        
+
     if not name in idx_cache:
         idx_cache[name] = []
         for flow_idx, flow in enumerate(flows):
             is_matching_flow = (
                 flow.name == request["flow_name"]
                 and ((not flow.source) or flow.source.has_strata(request["source_strata"]))
                 and ((not flow.dest) or flow.dest.has_strata(request["dest_strata"]))
@@ -199,31 +206,31 @@
         midpoint_output[1:] = (this_flow_values[1:] + this_flow_values[:-1]) * 0.5
         return midpoint_output, idx_cache
 
 
 def _get_compartment_output(request, name, outputs, compartments, idx_cache=None):
     if not idx_cache:
         idx_cache = {}
-        
+
     if not name in idx_cache:
         req_compartments = request["compartments"]
         strata = request["strata"]
         comps = ((i, c) for i, c in enumerate(compartments) if c.has_name_in_list(req_compartments))
         idx_cache[name] = [i for i, c in comps if c.is_match(c.name, strata)]
-    
+
     idxs = idx_cache[name]
     return outputs[:, idxs].sum(axis=1), idx_cache
 
 
 def _get_aggregate_output(request, derived_outputs):
     source_names = request["sources"]
     return sum([derived_outputs[s] for s in source_names])
 
 
-def _get_cumulative_output(request, name, times, derived_outputs,baseline_offset=None):
+def _get_cumulative_output(request, name, times, derived_outputs, baseline_offset=None):
     source_name = request["source"]
     start_time = request["start_time"]
     max_time = times.max()
     if start_time and start_time > max_time:
         # Handle case where the derived output starts accumulating after the last model timestep.
         msg = f"Cumulative output '{name}' start time {start_time} is greater than max model time {max_time}, defaulting to {max_time}"
         logger.warn(msg)
@@ -244,25 +251,30 @@
 
 
 def _get_func_output(request, derived_outputs):
     func = request["func"]
     source_names = request["sources"]
     inputs = [derived_outputs[s] for s in source_names]
     return func(*inputs)
-    
+
+
 def _get_param_func_output(request, derived_outputs, computed_values, parameters):
     mfunc = request["func"]
-    sources = dict(derived_outputs=derived_outputs, parameters=parameters, computed_values=computed_values)
+    sources = dict(
+        derived_outputs=derived_outputs, parameters=parameters, computed_values=computed_values
+    )
     args, kwargs = build_args(mfunc.args, mfunc.kwargs, sources)
     return mfunc.func(*args, **kwargs)
 
+
 def _get_computed_value_output(request, computed_values):
     name = request["name"]
     return computed_values[name].to_numpy(dtype=float)
 
+
 def get_scenario_start_index(base_times, start_time):
     """
     Returns the index of the closest time step that is at, or before the scenario start time.
     """
     assert (
         base_times[0] <= start_time
     ), f"Scenario start time {start_time} is before baseline has started"
```

### Comparing `summerepi-4.1.0a0/summer/experimental/model_builder.py` & `summerepi-4.2.0a0/summer/experimental/model_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,36 +13,27 @@
 # from pydantic import BaseModel
 # from pydantic.main import ModelMetaclass
 
 from summer.parameters import Parameter, Function, Data
 from computegraph import ComputeGraph
 from computegraph.utils import expand_nested_dict, is_var
 
-from .abstract_parameter import AbstractParameter
-
 GraphObj = Union[Function, Data]
 
 
 class ParamStruct:
     pass
 
 
 class ModelBuilder:
-    def __init__(self, params: dict, param_class: ParamStruct):
+    def __init__(self, params: dict, param_class: type):
         self._params = params
         self._params_expanded = expand_nested_dict(params, include_parents=True)
         self.params = self._pyd_params = param_class(**params)
-        self.input_graph = {}
-
-        self.required_outputs = set()
-
-    def add_output(self, key: str, graph_obj: GraphObj):
-        if key in self.input_graph:
-            raise Exception(f"Key {key} already exists in graph as {self.input_graph[key]}")
-        self.input_graph[key] = graph_obj
+        label_parameters(self.params, params)
 
     def set_model(self, model: CompartmentalModel):
         self.model = model
         model.builder = self
 
     def _get_func_args(self, key):
         return [Parameter(k) for k in [*self._params_expanded[key]]]
@@ -60,15 +51,15 @@
         """Get a Parameter (computegraph Variable) for the given key
         If this key is not contained in the initial parameters, register it
         as a required additional parameter (or raise an Exception if create is False)
 
         Args:
             key: Key of the parameter
             create: Add this parameter as an output if required - will raise an exception
-                    if False if key is not already present in the input parameters
+                    if False and key is not already present in the input parameters
 
         Returns:
             computegraph Parameter
         """
         if isinstance(key, str):
             key = key
         elif is_var(key, "parameters"):
@@ -79,19 +70,14 @@
             if create:
                 if key not in self.required_outputs:
                     self.required_outputs.add(key)
             else:
                 raise KeyError(f"Parameter {key} not found in input parameters")
         return Parameter(key)
 
-    def get_output(self, key):
-        if key not in self.input_graph:
-            raise KeyError(f"{key} does not exist in builder outputs")
-        return Parameter(key)
-
     def _get_value(self, key: str):
         """Return the initial parameter value for the given key
 
         Args:
             key (str): Parameter key
         """
         if key in self._params_expanded:
@@ -111,35 +97,70 @@
             [hasattr(param_obj, arg) for arg in argspec.args if arg not in supplied_argkeys]
         ), msg
         base_key = self.find_key_from_obj(param_obj)
         mapped_args = {arg: Parameter(f"{base_key}.{arg}") for arg in argspec.args}
         mapped_args.update(kwargs)
         return Function(func, [], mapped_args)
 
-    def get_jax_runner(self, jit=True):
+    def get_jax_runner(self, jit=True, solver=None):
         self.model.finalize()
-        run_everything, run_inputs, _, _ = get_full_runner(self, True)
+        run_everything, _, _ = get_full_runner(self, True, solver=solver)
         if jit:
             from jax import jit as _jit
 
             run_everything = _jit(run_everything)
         return run_everything
 
+    def get_input_parameters(self):
+        return self.model.get_input_parameters()
+
+    def get_default_parameters(self) -> dict:
+        default_params = {
+            k: v for k, v in self._params_expanded.items() if k in self.get_input_parameters()
+        }
+        return default_params
+
+
+def label_parameters(pstruct: ParamStruct, pdict: dict, layer: list = None):
+    """Walk the parameter dictionary pdict, alongside the ParamStruct,
+       setting concrete parameter names for each AbstractParameter encountered
+
+    Args:
+        pstruct (ParamStruct): The ParamStruct describing the model
+        pdict (dict): The parameter dictionary used as constructor for pstruct
+        layer: The current naming layer (used internally, do not set)
+    """
+    if layer is None:
+        layer = []
+    for k, v in pdict.items():
+        if isinstance(pstruct, dict):
+            cur_pstruct = pstruct[k]
+        else:
+            cur_pstruct = getattr(pstruct, k)
+        if isinstance(cur_pstruct, Parameter):
+            param_key = ".".join(layer + [k])
+            cur_pstruct.set_key(param_key)
+        elif isinstance(cur_pstruct, dict):
+            label_parameters(cur_pstruct, v, layer + [k])
+        elif isinstance(cur_pstruct, ParamStruct):
+            assert isinstance(v, dict)
+            label_parameters(cur_pstruct, v, layer + [k])
+
 
 def find_key_from_obj(obj: Any, pydparams: ParamStruct, params: dict, layer=None, is_dict=False):
     if layer is None:
         layer = []
     for k, v in params.items():
 
         if is_dict:
             cur_pydobj = pydparams[k]
         else:
             cur_pydobj = getattr(pydparams, k)
         if cur_pydobj is obj:
-            if isinstance(cur_pydobj, ParamStruct) or isinstance(cur_pydobj, AbstractParameter):
+            if isinstance(cur_pydobj, ParamStruct) or isinstance(cur_pydobj, Parameter):
                 return ".".join(layer + [k])
             else:
                 raise TypeError("Cannot match against type", type(obj))
         if isinstance(cur_pydobj, dict):
             res = find_key_from_obj(obj, cur_pydobj, v, layer + [k], True)
             if res is not None:
                 return res
@@ -173,82 +194,66 @@
         elif isinstance(cur_obj, Iterable):
             cur_obj = cur_obj[layer]
         else:
             raise TypeError("Cannot resolve for type", key, cur_obj, type(cur_obj))
     return cur_obj
 
 
-def get_full_runner(builder, use_jax=False):
-    graph_run = ComputeGraph(builder.input_graph).get_callable()
-
+def get_full_runner(builder, use_jax=False, solver=None):
     if use_jax:
         from summer.runner.jax.util import get_runner
         from summer.runner.jax.model_impl import build_run_model
 
         jrunner = get_runner(builder.model)
-        jax_run_func, jax_runner_dict = build_run_model(jrunner)
+        jax_run_func, jax_runner_dict = build_run_model(jrunner, solver=solver)
 
     model_input_p = builder.model.get_input_parameters()
 
     def run_everything(parameters=None, **kwargs):
 
         params_base = builder._params_expanded.copy()
         if parameters is not None:
             params_base.update(parameters)
 
-        graph_outputs = graph_run(parameters=params_base)
-        params_base.update(graph_outputs)
-
         model_params = {k: v for k, v in params_base.items() if k in model_input_p}
 
         if use_jax:
             return jax_run_func(parameters=model_params)
         else:
             builder.model.run(parameters=model_params, **kwargs)
             return builder.model
 
-    def run_inputs(param_updates=None):
-        parameters = builder._params_expanded.copy()
-        if param_updates is not None:
-            parameters.update(param_updates)
-
-        graph_outputs = graph_run(parameters=parameters)
-        parameters.update(graph_outputs)
-
-        model_params = {k: v for k, v in parameters.items() if k in model_input_p}
-        return model_params
-
     if use_jax:
-        return run_everything, run_inputs, jax_run_func, jax_runner_dict
+        return run_everything, jax_run_func, jax_runner_dict
     else:
         return run_everything
 
 
 def is_real(v):
     return isinstance(v, Real)
 
 
-def parameter_class(constraint_func=is_real, description: str = None):
+def parameter_class(constraint_func=is_real, desc: str = None, full_desc: str = None):
 
-    _description = description
+    _desc = desc
+    _full_desc = full_desc
 
-    class ConcreteParameter(AbstractParameter):
+    class ConcreteParameter(Parameter):
 
         constraint = constraint_func
-        description = _description
+        description = _desc
+        full_description = _full_desc
 
         def __init__(self, value):
+            super().__init__(key=None)
             self.value = value
 
         def __repr__(self):
-            if self.description:
-                desc_str = f" {self.description} "
-            else:
-                desc_str = ""
-            return f"Parameter:{desc_str}({self.value})"
+            pkey = self.key or self.description or "param"
+            return f"{pkey}({self.value})"
 
         @classmethod
         def __get_validators__(cls):
             yield cls.validate
 
         @classmethod
         def validate(cls, v):
```

### Comparing `summerepi-4.1.0a0/summer/flows.py` & `summerepi-4.2.0a0/summer/flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module contains the classes which are used to calculate inter-compartmental flow rates.
 As a user of the framework you should not have to use these classes directly.
 """
 from abc import ABC, abstractmethod
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, Set
 
 import numpy as np
 
 from summer.adjust import BaseAdjustment, FlowParam, Multiply
 from summer.compartment import Compartment
 from summer.parameters import is_func
 from summer.parameters.param_impl import ModelParameter
@@ -29,14 +29,15 @@
 
     name = None
     source = None
     dest = None
     param = None
     adjustments = None
     is_death_flow = False
+    tags = None
 
     def _is_equal(self, flow):
         """For testing"""
         return (
             type(self) is type(flow)
             and self.name == flow.name
             and self.source == flow.source
@@ -75,29 +76,14 @@
         else:
             flow_rate = self.param
         for adjustment in self.adjustments:
             flow_rate = adjustment.get_new_value(flow_rate, computed_values, time, parameters)
 
         return flow_rate
 
-    def weight_type(self) -> str:
-        """Returns a WeightType enum value
-
-            'static': Fixed floating point value
-            'function': Calculated from a callable function
-
-        Returns:
-            bool: False if weight is time-varying, otherwise True
-        """
-        is_time_varying = is_func(self.param) or sum([is_func(a.param) for a in self.adjustments])
-        if not is_time_varying:
-            return WeightType.STATIC
-        else:
-            return WeightType.FUNCTION
-
     def update_compartment_indices(self, mapping: Dict[str, float]):
         """
         Update index which maps flow compartments to compartment value array.
         """
         if self.source:
             self.source.idx = mapping[self.source]
         if self.dest:
@@ -148,20 +134,23 @@
 
     def __init__(
         self,
         name: str,
         dest: Compartment,
         param: FlowParam,
         adjustments: List[BaseAdjustment] = None,
+        tags: Set[str] = None,
     ):
         assert type(dest) is Compartment
         self.name = name
         self.adjustments = [a for a in (adjustments or []) if a and a.param is not None]
         self.dest = dest
         self.param = param
+        tags = tags or set()
+        self.tags = tags
 
     def stratify(self, strat: Stratification) -> List[BaseFlow]:
         """
         Returns a list of new, stratified entry flows to replace the current flow.
         """
         if not self.dest.has_name_in_list(strat.compartments):
             # Flow destination is not stratified, do not stratify this flow.
@@ -198,14 +187,15 @@
 
             new_dest = self.dest.stratify(strat.name, stratum)
             new_flow = self.copy(
                 name=self.name,
                 dest=new_dest,
                 param=self.param,
                 adjustments=new_adjustments,
+                tags=self.tags,
             )
             new_flows.append(new_flow)
 
         return new_flows
 
     def __repr__(self):
         return f"<{self.__class__.__name__} '{self.name}' to {self.dest}>"
@@ -220,20 +210,23 @@
 
     def __init__(
         self,
         name: str,
         source: Compartment,
         param: FlowParam,
         adjustments: List[BaseAdjustment] = None,
+        tags: Set[str] = None,
     ):
         assert type(source) is Compartment
         self.name = name
         self.adjustments = [a for a in (adjustments or []) if a and a.param is not None]
         self.source = source
         self.param = param
+        tags = tags or set()
+        self.tags = tags
 
     def stratify(self, strat: Stratification) -> List[BaseFlow]:
         """
         Returns a list of new, stratified exit flows to replace the current flow.
         """
         if not self.source.has_name_in_list(strat.compartments):
             # Flow source is not stratified, do not stratify this flow.
@@ -255,14 +248,15 @@
 
             new_source = self.source.stratify(strat.name, stratum)
             new_flow = self.copy(
                 name=self.name,
                 source=new_source,
                 param=self.param,
                 adjustments=new_adjustments,
+                tags=self.tags,
             )
             new_flows.append(new_flow)
 
         return new_flows
 
     def __repr__(self):
         return f"<{self.__class__.__name__} '{self.name}' from {self.source}>"
@@ -278,22 +272,25 @@
     def __init__(
         self,
         name: str,
         source: Compartment,
         dest: Compartment,
         param: FlowParam,
         adjustments: List[BaseAdjustment] = None,
+        tags: Set[str] = None,
     ):
         assert type(source) is Compartment
         assert type(dest) is Compartment
         self.name = name
         self.adjustments = [a for a in (adjustments or []) if a and a.param is not None]
         self.source = source
         self.dest = dest
         self.param = param
+        tags = tags or set()
+        self.tags = tags
 
     def stratify(self, strat: Stratification) -> List[BaseFlow]:
         """
         Returns a list of new, stratified flows to replace the current flow.
         """
         is_source_compartment_stratified = self.source.has_name_in_list(strat.compartments)
         is_dest_compartment_stratified = self.dest.has_name_in_list(strat.compartments)
@@ -354,14 +351,15 @@
 
             new_flow = self.copy(
                 name=self.name,
                 source=new_source,
                 dest=new_dest,
                 param=self.param,
                 adjustments=new_adjustments,
+                tags=self.tags,
             )
             new_flows.append(new_flow)
 
         return new_flows
 
     def __repr__(self):
         return f"<{self.__class__.__name__} '{self.name}' from {self.source} to {self.dest}>"
@@ -495,74 +493,48 @@
         parameters: dict = None,
     ) -> float:
         parameter_value = self.get_weight_value(time, computed_values, parameters)
         population = compartment_values[self.source.idx]
         return parameter_value * population
 
 
-class FunctionFlow(BaseTransitionFlow):
-    """
-    A flow that transfers people from a source to a destination based on a user-defined function.
-    Note that the rate is NOT multiplied by the size of the source compartment.
-    This can be used to define more complex flows if required.
-    Important to be careful that compartment sizes do not go negative with these flows, as this is
-    not guaranteed.
-
-    Args:
-        name: The flow name.
-        source: The source compartment.
-        dest: The destination compartment.
-        param: A function that returns the flow rate, before adjustments. See `get_net_flow` for
-        this function's arguments.
-        adjustments: Adjustments to the flow rate.
-
-    """
-
+class AbsoluteFlow(BaseTransitionFlow):
     def get_net_flow(
         self,
-        compartments: List[Compartment],
         compartment_values: np.ndarray,
-        flows: List[BaseFlow],
-        flow_rates: np.ndarray,
         computed_values: dict,
         time: float,
+        parameters: dict = None,
     ) -> float:
-        if callable(self.param):
-            # Plain python function
-            param = self.param
-        else:
-            # PyFunction ModelParameter object
-            param = self.param.func
-        flow_rate = param(
-            self, compartments, compartment_values, flows, flow_rates, computed_values, time
-        )
-        for adjustment in self.adjustments:
-            flow_rate = adjustment.get_new_value(flow_rate, time, computed_values)
-
-        return flow_rate
+        parameter_value = self.get_weight_value(time, computed_values, parameters)
+        return parameter_value
 
 
 class BaseInfectionFlow(BaseTransitionFlow):
     def __init__(
         self,
         name: str,
         source: Compartment,
         dest: Compartment,
         param: FlowParam,
         find_infectious_multiplier: Callable[[Compartment, Compartment], float],
         adjustments: List[BaseAdjustment] = None,
+        tags: Set[str] = None,
     ):
         assert type(source) is Compartment
         assert type(dest) is Compartment
         self.name = name
         self.adjustments = [a for a in (adjustments or []) if a and a.param is not None]
         self.source = source
         self.dest = dest
         self.param = param
         self.find_infectious_multiplier = find_infectious_multiplier
+        tags = tags or set()
+        tags.add("infection")
+        self.tags = tags
 
     def get_net_flow(
         self,
         compartment_values: np.ndarray,
         computed_values: dict,
         time: float,
         parameters: dict = None,
```

### Comparing `summerepi-4.1.0a0/summer/inspect.py` & `summerepi-4.2.0a0/summer/inspect.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,70 @@
 """Tools for probing, querying, inspecting and drawing CompartmentalModels
 
 The main entry point for this is the ModelProbe class
 """
 
 import re
-from typing import Iterable, Set
+from typing import Iterable, Set, List
 
 import networkx as nx
+import numpy as np
 
 from summer import CompartmentalModel
 from summer.compartment import Compartment
 from summer.flows import BaseFlow
 
 
-def query_compartments(m: CompartmentalModel, query: dict):
+def query_compartments(m: CompartmentalModel, query: dict = None, tags: List = None, as_idx=False):
+    query = query or {}
+    tags = tags or []
+    if isinstance(tags, str):
+        tags = [tags]
     if "name" in query:
         query = query.copy()
         name = query.pop("name")
-        return m.get_matching_compartments(name, query)
+        matching = m.get_matching_compartments(name, query)
+        if as_idx:
+            return np.array(
+                [c.idx for c in matching if all([t in c.tags for t in tags])], dtype=int
+            )
+        else:
+            return [c for c in matching if all([t in c.tags for t in tags])]
     else:
         _strata = frozenset(query.items())
-        return [c for c in m.compartments if c._has_strata(_strata)]
+        if as_idx:
+            return np.array(
+                [
+                    c.idx
+                    for c in m.compartments
+                    if c._has_strata(_strata) and all([t in c.tags for t in tags])
+                ],
+                dtype=int,
+            )
+        else:
+            return [
+                c
+                for c in m.compartments
+                if c._has_strata(_strata) and all([t in c.tags for t in tags])
+            ]
 
 
 def query_flows(
-    m: CompartmentalModel, flow_name: str = None, source: dict = None, dest: dict = None
+    m: CompartmentalModel,
+    flow_name: str = None,
+    source: dict = None,
+    dest: dict = None,
+    tags: List = None,
 ):
     if flow_name is not None:
-        re_pat = re.compile(flow_name)
-        flows = [f for f in m._flows if re_pat.match(f.name)]
+        if isinstance(flow_name, str):
+            re_pat = re.compile(flow_name)
+            flows = [f for f in m._flows if re_pat.match(f.name)]
+        else:
+            flows = flow_name
     else:
         flows = m._flows
 
     if source:
         if "name" in source:
             source = source.copy()
             name = source.pop("name")
@@ -46,14 +78,19 @@
             dest = dest.copy()
             name = dest.pop("name")
             flows = [f for f in flows if f.dest and f.dest.name == name]
         else:
             dest = frozenset(dest.items())
             flows = [f for f in flows if f.dest and f.dest._has_strata(source)]
 
+    if tags:
+        if isinstance(tags, str):
+            tags = [tags]
+        flows = [f for f in flows if all([t in f.tags for t in tags])]
+
     return flows
 
 
 def flows_to_compartments(m: CompartmentalModel, flows: Iterable[BaseFlow]):
     comps = []
     for f in flows:
         if f.source:
@@ -83,20 +120,21 @@
         for c in compartments:
             flows += self._compartment_flow_map[c]
         return set(flows)
 
     def flows_to_compartments(self, flows: Iterable[BaseFlow]) -> Set[Compartment]:
         return flows_to_compartments(self.model, flows)
 
-    def query_compartments(self, query: dict = None):
-        query = query or {}
-        return query_compartments(self.model, query)
+    def query_compartments(self, query: dict = None, tags: List = None, as_idx=False):
+        return query_compartments(self.model, query, tags, as_idx)
 
-    def query_flows(self, flow_name: str = None, source: dict = None, dest: dict = None):
-        return query_flows(self.model, flow_name, source, dest)
+    def query_flows(
+        self, flow_name: str = None, source: dict = None, dest: dict = None, tags: List = None
+    ):
+        return query_flows(self.model, flow_name, source, dest, tags)
 
     def get_model_subset(self, comp_query: dict = None, flow_query: dict = None):
 
         comp_query = comp_query or {}
         flow_query = flow_query or {}
 
         comps = self.query_compartments(comp_query)
```

### Comparing `summerepi-4.1.0a0/summer/model.py` & `summerepi-4.2.0a0/summer/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,43 +8,38 @@
 from typing import Callable, Dict, List, Optional, Tuple
 from warnings import warn
 
 import networkx
 import numpy as np
 import pandas as pd
 
-from computegraph.utils import is_var
+from computegraph import ComputeGraph
 
 import summer.flows as flows
 from summer import stochastic
 from summer.adjust import BaseAdjustment, FlowParam, Multiply
 from summer.compartment import Compartment
-from summer.compute import ComputedValueProcessor
 from summer.derived_outputs import DerivedOutputRequest, calculate_derived_outputs
 from summer.parameters import params
 
-# from summer.parameters.param_impl import replace_with_typed_params
-from summer.parameters.params import find_all_parameters, Function
 from summer.parameters.param_impl import finalize_parameters
-from summer.runner import ReferenceRunner, VectorizedRunner
-from summer.runner.jax.runner import JaxRunner
+from summer.runner import ModelBackend
 from summer.solver import SolverType, solve_ode
 from summer.stratification import Stratification
-from summer.utils import get_scenario_start_index, ref_times_to_dti
+from summer.utils import get_scenario_start_index, ref_times_to_dti, clean_compartment_values
 from summer.population import get_unique_strat_groups, filter_by_strata
 from summer.tracker import ModelBuildTracker, ActionType
 
 logger = logging.getLogger()
 
 FlowRateFunction = Callable[[List[Compartment], np.ndarray, np.ndarray, float], np.ndarray]
 
 
 class BackendType:
-    REFERENCE = "reference"
-    VECTORIZED = "vectorized"
+    PYTHON = "python"
     JAX = "jax"
 
 
 class CompartmentalModel:
     """
     A compartmental disease model
 
@@ -74,15 +69,15 @@
             ``outputs`` for each timestep.
 
 
     """
 
     _DEFAULT_DISEASE_STRAIN = "default"
     _DEFAULT_MIXING_MATRIX = np.array([[1.0]])
-    _DEFAULT_BACKEND = BackendType.VECTORIZED
+    _DEFAULT_BACKEND = BackendType.PYTHON
 
     def __init__(
         self,
         times: Tuple[int, int],
         compartments: List[str],
         infectious_compartments: List[str],
         timestep: float = 1.0,
@@ -99,27 +94,33 @@
         assert num_steps % 1 == 0, msg
         self.times = np.linspace(start_t, end_t, num=int(num_steps))
         self.timestep = timestep
 
         # Set the ref_date; the datetime object equivalent to times[0]
         self.ref_date = ref_date
 
+        if isinstance(infectious_compartments, str):
+            infectious_compartments = [infectious_compartments]
         error_msg = "Infectious compartments must be a subset of compartments"
         assert all(n in compartments for n in infectious_compartments), error_msg
-        self.compartments = [Compartment(n) for n in compartments]
+        self.compartments = [Compartment(n, idx=i) for i, n in enumerate(compartments)]
+        for c in self.compartments:
+            if c in infectious_compartments:
+                c.tags.append("infectious")
 
         # Compartment name lookup; needs to be present before adding any flows
         self._update_compartment_name_map()
 
         self._infectious_compartments = [Compartment(n) for n in infectious_compartments]
         self.initial_population = np.zeros_like(self.compartments, dtype=np.float)
         # Keeps track of original, pre-stratified compartment names.
         self._original_compartment_names = [Compartment.deserialize(n) for n in compartments]
         # Keeps track of Stratifications that have been applied.
         self._stratifications = []
+        self.stratifications = {}
         # Flows to be applied to the model compartments
         self._flows = []
 
         # Turn on all runtime assertions by default; can be disabled for performance reasons
         # Setting to False still retains some checking, but turns off the most costly checks
         self.set_validation_enabled(True)
         self._derived_outputs_idx_cache = {}
@@ -131,15 +132,14 @@
         self._derived_output_requests = {}
         # Track 'derived output' request dependencies in a directed acylic graph (DAG).
         self._derived_output_graph = networkx.DiGraph()
         # Whitelist of 'derived outputs' to evaluate
         self._derived_outputs_whitelist = []
 
         # Map of (runtime) computed values
-        self._computed_value_processors = OrderedDict()
         self._computed_values_graph_dict = {}
 
         # Init baseline model to None; can be set via set_baseline if running as a scenario
         self._baseline = None
 
         # Mixing matrices: a list of square arrays, or functions, used to calculate
         # force of infection.
@@ -158,17 +158,14 @@
 
         if takes_params:
             self._defer_actions = True
         else:
             self._defer_actions = False
         self._finalized = False
 
-        self.builder = None
-        self._lazy_params = set()
-
     def _update_compartment_indices(self):
         """
         Update the mapping of compartment name to idx for quicker lookups.
         """
         compartment_idx_lookup = {}
         # Update the mapping of compartment name to idx for quicker lookups.
         for idx, c in enumerate(self.compartments):
@@ -178,45 +175,58 @@
         for flow in self._flows:
             flow.update_compartment_indices(compartment_idx_lookup)
 
     def _assert_not_finalized(self):
         error_msg = "Cannot make changes to model that is already finalized"
         assert not self._finalized, error_msg
 
-    def set_initial_population(self, distribution: Dict[str, float]):
+    def set_initial_population(self, distribution: Dict[str, float], force=False):
         """
         Sets the initial population of the model, which is zero by default.
 
         Args:
             distribution: A map of populations to be assigned to compartments.
 
         """
-        self._assert_not_finalized()
+        if not force:
+            self._assert_not_finalized()
+
+            error_msg = "Cannot set initial population after the model has been stratified"
+            assert not self._stratifications, error_msg
 
-        error_msg = "Cannot set initial population after the model has been stratified"
-        assert not self._stratifications, error_msg
-        self._initial_population_distribution = distribution
-
-        if isinstance(distribution, dict):
-            for idx, comp in enumerate(self.compartments):
-                pop = distribution.get(comp.name, 0)
-                assert pop >= 0, f"Population for {comp.name} cannot be negative: {pop}"
-                self.initial_population[idx] = pop
+        assert isinstance(distribution, dict)
 
-            self._original_init_population = self.initial_population.copy()
+        # Make sure we're not supplying any eroneous compartment names
+        for k, v in distribution.items():
+            assert k in self._original_compartment_names
 
-        elif not (is_var(distribution, "parameters") or isinstance(distribution, Function)):
-            raise TypeError("Initial population must be dict, Parameter, or Function", distribution)
+        self._init_pop_dist = distribution.copy()
+
+        # Ensure dictionary contains all comparments (default to 0 if not supplied)
+        for idx, comp in enumerate(self._original_compartment_names):
+            if comp not in self._init_pop_dist:
+                self._init_pop_dist[comp] = 0
 
     def finalize(self):
         if not self._finalized:
-            all_params = finalize_parameters(self, self.builder)
-            self._input_params = all_params
+            finalize_parameters(self)
             self._finalized = True
 
+    def get_object_graph(self, obj) -> ComputeGraph:
+        """Return the ComputeGraph for this object
+
+        Args:
+            obj: Any summer object with a graph_key
+        """
+        if isinstance(obj, dict):
+            targets = [v._graph_key for v in obj.values()]
+        else:
+            targets = obj._graph_key
+        return self.graph.filter(targets)
+
     def set_validation_enabled(self, validate: bool):
         """
         Set this to False in order to turn of some (potentially expensive) runtime validation
         E.g. In calibration, leave it enabled for the first iteration, to catch any structural
         model issues, but then disable for subsequent iterations
         """
         self._should_validate = validate
@@ -577,51 +587,14 @@
             source,
             dest,
             source_strata,
             dest_strata,
             expected_flow_count,
         )
 
-    def add_function_flow(
-        self,
-        name: str,
-        flow_rate_func: FlowRateFunction,
-        source: str,
-        dest: str,
-        source_strata: Optional[Dict[str, str]] = None,
-        dest_strata: Optional[Dict[str, str]] = None,
-        expected_flow_count: Optional[int] = None,
-    ):
-        """
-        A flow that transfers people from a source to a destination based on a user-defined function
-        This can be used to define more complex flows if required. See `flows.FunctionFlow` for more
-        details on the arguments to the function.
-
-        Args:
-            name: The name of the new flow.
-            flow_rate_func:  A function that returns the flow rate, before adjustments.
-            source: The name of the source compartment.
-            dest: The name of the destination compartment.
-            source_strata (optional): A whitelist of strata to filter the source compartments.
-            dest_strata (optional): A whitelist of strata to filter the destination compartments.
-            expected_flow_count (optional): Used to assert that a particular number of flows are
-                                            created.
-
-        """
-        self._add_transition_flow(
-            flows.FunctionFlow,
-            name,
-            flow_rate_func,
-            source,
-            dest,
-            source_strata,
-            dest_strata,
-            expected_flow_count,
-        )
-
     def _add_transition_flow(
         self,
         flow_cls,
         name: str,
         param: FlowParam,
         source: str,
         dest: str,
@@ -713,14 +686,15 @@
         """
         Apply the stratification to the model's flows and compartments.
 
         Args:
             strat: The stratification to apply.
 
         """
+
         self._assert_not_finalized()
         # Enable/disable runtime assertions for strat
         strat._validate = self._should_validate
 
         # Validate flow adjustments
         flow_names = [f.name for f in self._flows]
         for n in strat.flow_adjustments.keys():
@@ -815,14 +789,15 @@
                         dest=dest.name,
                         source_strata=source.strata,
                         dest_strata=dest.strata,
                         expected_flow_count=1,
                     )
 
         self._stratifications.append(strat)
+        self.stratifications[strat.name] = strat
 
         self.tracker.append_action(ActionType.STRATIFY, strat=strat)
 
     def _strata_exist(self, strata: dict):
         """
         Verify whether all the strata exist within the model
         Raises an Exception if not
@@ -832,14 +807,28 @@
             if k not in strat_names:
                 raise KeyError(f"Invalid stratification {k}")
             for s in self._stratifications:
                 if k == s.name:
                     if v not in s.strata:
                         raise ValueError(f"Invalid stratum {v} for {s}")
 
+    def get_stratification(self, name: str) -> Stratification:
+        """Return Stratification matching name, or None if not found
+
+        Args:
+            name: Name of stratificaton to get
+
+        Returns:
+            Stratification
+        """
+        for stratification in self._stratifications:
+            if stratification.name == name:
+                return stratification
+        return None
+
     def adjust_population_split(self, strat: str, dest_filter: dict, proportions: dict):
         """Adjust the initial population to redistribute the population for a particular
         stratification, over a subset of some other strata
 
         Args:
             strat (str): The stratification to redistribute over
             dest_filter (dict): Subset of (other) strata to filter the split by
@@ -881,14 +870,40 @@
             proportions=proportions,
         )
 
     """
     Running the model
     """
 
+    def get_runner(self, parameters: dict, dyn_params: List = None):
+        self._update_compartment_indices()
+        self.finalize()
+
+        from computegraph.jaxify import get_using_jax
+
+        if get_using_jax():
+            self._set_backend("jax")
+            # self._backend.prepare_to_run(parameters)
+            self._backend.prepare_structural()
+
+            from summer.runner.jax.model_impl import build_run_model
+
+            jax_run_func, jax_runner_dict = build_run_model(
+                self._backend, base_params=parameters, dyn_params=dyn_params
+            )
+            from jax import jit
+
+            return ModelResults(self, jit(jax_run_func))
+        else:
+            self._set_backend("python")
+            self._backend.prepare_structural()
+            self._backend.prepare_static_params(parameters, dyn_params)
+
+        
+
     def run(
         self,
         solver: str = SolverType.SOLVE_IVP,
         backend: str = _DEFAULT_BACKEND,
         backend_args: dict = None,
         parameters: dict = None,
         **kwargs,
@@ -914,30 +929,31 @@
 
         # Ensure we call this before model runs, since it is now disabled inside individual
         # flow constructors
         self._update_compartment_indices()
 
         self.finalize()
 
-        # replace_with_typed_params(self, self.builder)
-
         self._set_backend(backend, backend_args)
         # self._backend.prepare_to_run(parameters)
         self._backend.prepare_structural()
-        self._backend.prepare_dynamic(parameters)
 
         if backend == BackendType.JAX:
             from summer.runner.jax.model_impl import build_run_model
 
-            jax_run_func, jax_runner_dict = build_run_model(self._backend, solver)
+            jax_run_func, jax_runner_dict = build_run_model(self._backend, solver=solver)
             res = jax_run_func(parameters=parameters)
             self.outputs = np.array(res["outputs"])
             self.derived_outputs = {k: np.array(v) for k, v in res["derived_outputs"].items()}
             return self
 
+        # Non-Jax run - need to call prepare_* manually
+        self._backend.prepare_static_params(parameters)
+        self._backend.prepare_dynamic({})
+
         if solver == SolverType.STOCHASTIC:
             # Run the model in 'stochastic mode'.
             seed = kwargs.get("seed")
             self._solve_stochastic(seed)
         else:
             # Run the model as a deterministic ODE
             self._solve_ode(solver, kwargs)
@@ -947,20 +963,18 @@
 
         # Calculate any requested derived outputs, based on the calculated compartment sizes.
         self.derived_outputs, self._derived_outputs_idx_cache = self._calculate_derived_outputs()
         return self
 
     def _set_backend(self, backend: str, backend_args: dict = None):
         backend_args = backend_args or {}
-        if backend == BackendType.REFERENCE:
-            self._backend = ReferenceRunner(self, **backend_args)
-        elif backend == BackendType.VECTORIZED:
-            self._backend = VectorizedRunner(self, **backend_args)
+        if backend == BackendType.PYTHON:
+            self._backend = ModelBackend(self, **backend_args)
         elif backend == BackendType.JAX:
-            self._backend = JaxRunner(self, **backend_args)
+            self._backend = ModelBackend(self, **backend_args)
         else:
             msg = f"Invalid backend: {backend}"
             raise ValueError(msg)
 
     def run_stochastic(
         self,
         seed: Optional[int] = None,
@@ -1036,16 +1050,16 @@
             if time_idx == 0:
                 # Skip time zero, use initial conditions.
                 continue
 
             # Calculate the flow rates at this timestep.
             # These describe the rate (people/timeunit) at which people follow the flow.
             # Later we will convert these to probabilities.
-            comp_vals = self._backend._clean_compartment_values(self.outputs[time_idx - 1])
-            flow_rates = self._backend.get_flow_rates(comp_vals, time)
+            comp_vals = clean_compartment_values(self.outputs[time_idx - 1])
+            flow_rates, _ = self._backend.get_flow_rates(comp_vals, time)
 
             # We split the calculatd flow rates into entry or {transition, exit} flows,
             # because we handle them separately with different methods.
 
             # Transition (and exit) flow are stored in a 2D FxC ndarray where f is the flow idx
             # and c is the compartment idx, giving us a matrix of flows rates out of each
             # compartment.
@@ -1191,14 +1205,17 @@
             name: The name of the derived output.
             compartments: The name of the compartments to track.
             strata (optional): A whitelist of strata to filter the compartments.
             save_results (optional): Whether to save or discard the results.
         """
         strata = strata or {}
 
+        if isinstance(compartments, str):
+            compartments = [compartments]
+
         if self._should_validate:
             msg = f"A derived output named {name} already exists."
             assert name not in self._derived_output_requests, msg
             is_match_exists = any(
                 [
                     any([c.is_match(name, strata) for name in compartments])
                     for c in self.compartments
@@ -1343,15 +1360,15 @@
             save_results (bool, optional): _description_. Defaults to True.
         """
 
         msg = f"A derived output named {name} already exists."
         assert name not in self._derived_output_requests, msg
         for k, v in func.kwargs.items():
             if isinstance(v, params.DerivedOutput):
-                source = v.name
+                source = v.key
                 assert (
                     source in self._derived_output_requests
                 ), f"Source {source} has not been requested."
                 self._derived_output_graph.add_edge(source, name)
 
         self._derived_output_graph.add_node(name)
         self._derived_output_requests[name] = {
@@ -1374,41 +1391,36 @@
         self._derived_output_graph.add_node(name)
         self._derived_output_requests[name] = {
             "request_type": DerivedOutputRequest.COMPUTED_VALUE,
             "name": name,
             "save_results": save_results,
         }
 
-    def add_computed_value_process(self, name: str, processor: ComputedValueProcessor):
+    def add_computed_value_process(self, name: str, processor):
         """
         Calculate (at runtime) values derived from the current compartment values and/or
         functions/input data
         providing time varying shared values.  The output values of these processes can be used by
         function parameters, adjustments, and function flows.
 
         Args:
             name (str): Name (key) of derived value (use this when referencing it in functions)
             processor (DerivedValueProcessor): Object providing implementation
         """
         # FIXME: We might actually have to keep this for now, at least until modellers get sick of
         # seeing it and change over all the code
-        warn(
-            "Deprecated feature - use model.add_computed_value_func instead",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        self._computed_value_processors[name] = processor
+        raise DeprecationWarning("Use add_computed_value_func instead")
 
     def add_computed_value_func(self, name: str, func: params.Function):
         if name in self._computed_values_graph_dict:
             raise Exception(f"Computed value function with name {name} already exists")
         self._computed_values_graph_dict[name] = func
 
     def get_computed_value_keys(self):
-        return list(self._computed_value_processors) + list(self._computed_values_graph_dict)
+        return list(self._computed_values_graph_dict)
 
     def _get_ref_idx(self):
         if self.ref_date:
             times = ref_times_to_dti(self.ref_date, self.times)
         else:
             times = self.times
         return times
@@ -1421,8 +1433,45 @@
     def get_derived_outputs_df(self):
         idx = self._get_ref_idx()
         return pd.DataFrame(self.derived_outputs, index=idx)
 
     def get_input_parameters(self):
         if not self._finalized:
             raise Exception("Cannot trace input parameters before model is finalized")
-        return self._input_params
+        all_in_var = self.graph.get_input_variables()
+        return set([v.key for v in all_in_var if v.source == "parameters"])
+
+    def query_compartments(self, query: dict = None, tags: List = None, as_idx=False):
+        from summer.inspect import query_compartments
+
+        return query_compartments(self, query, tags, as_idx)
+
+    def query_flows(
+        self,
+        flow_name: str = None,
+        source: dict = None,
+        dest: dict = None,
+        tags: List = None,
+    ):
+        from summer.inspect import query_flows
+
+        return query_flows(self, flow_name, source, dest, tags)
+
+class ModelResults:
+    def __init__(self, model, run_func):
+        self.model = model
+        self._run_func = run_func
+        
+    def get_outputs_df(self):
+        return self.model.get_outputs_df()
+    
+    def get_derived_outputs_df(self):
+        return self.model.get_derived_outputs_df()
+
+    def run(self, parameters: dict):
+        results = self._run_func(parameters=parameters)
+        self.outputs = np.array(results["outputs"])
+        self.derived_outputs = {k: np.array(v) for k, v in results["derived_outputs"].items()}
+        self.model.outputs = self.outputs
+        self.model.derived_outputs = self.derived_outputs
+        return results
+
```

### Comparing `summerepi-4.1.0a0/summer/parameters/param_impl.py` & `summerepi-4.2.0a0/summer/parameters/param_impl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,42 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from summer import CompartmentalModel
+
 from typing import Tuple, List, Iterable, Any
 from numbers import Real
 
-from summer.parameters.params import build_args, is_var, Function, Variable, ComputedValue, Time
-from summer.experimental.model_builder import AbstractParameter, ModelBuilder
-from summer.experimental.abstract_parameter import LazyParameter, set_keys
+from computegraph.types import GraphObject, Data, Function
+from computegraph.utils import defer, invert_dict, assign
+from computegraph import ComputeGraph
+from computegraph.jaxify import get_modules
+
+fnp = get_modules()["numpy"]
+
+from summer.parameters.params import (
+    build_args,
+    ComputedValue,
+    ComputedValuesDict,
+    Time,
+)
 
 
 class ModelParameter:
     def get_value(self, time: float, computed_values: dict, parameters: dict):
         raise NotImplementedError
 
     def __eq__(self, other):
         return hash(other) == hash(self)
 
     def is_time_varying(self):
         return False
 
 
-class DataParameter(ModelParameter):
-    """Generic container for Python objects"""
-
-    def __init__(self, value):
-        self.value = value
-
-    def get_value(self, time: float, computed_values: dict, parameters: dict):
-        return self.value
-
-    def __hash__(self):
-        return hash(self.value)
-
-    def __repr__(self):
-        return f"DataParameter: {self.value}"
-
-
-class FloatParameter(ModelParameter):
-    def __init__(self, value):
-        self.value = value
-
-    def get_value(self, time: float, computed_values: dict, parameters: dict):
-        return self.value
-
-    def __hash__(self):
-        return hash(self.value)
-
-    def __repr__(self):
-        return f"FloatParameter: {self.value}"
-
-
-class GraphParameter(ModelParameter):
-    def __init__(self, name):
-        self.name = name
-
-    def get_value(self, time: float, computed_values: dict, parameters: dict):
-        return parameters[self.name]
-
-    def __hash__(self):
-        return hash((self.name, "parameters"))
-
-    def __repr__(self):
-        return f"GraphParameter: {self.name}"
-
-
-def build_lazy_parameter(param, builder):
-    model = builder.model
-    param_keys = set_keys(param, builder)
-    model._lazy_params.add(param)
-    return LazyGraphParameter(param), param_keys
-
-
-class LazyGraphParameter(ModelParameter):
-    def __init__(self, param):
-        self.param = param
-        self._pkey = f"_lazy_{hash(param)}"
-
-    def get_value(self, time: float, computed_values: dict, parameters: dict):
-        return parameters[self._pkey]
-
-    def __hash__(self):
-        return hash(self.param)
-
-
 class ComputedValueParameter(ModelParameter):
     def __init__(self, name):
         self.name = name
 
     def get_value(self, time: float, computed_values: dict, parameters: dict):
         return computed_values[self.name]
 
@@ -93,59 +46,14 @@
     def __repr__(self):
         return f"ComputedValue: {self.name}"
 
     def is_time_varying(self):
         return True
 
 
-def concretize_arg(arg: Any, builder: ModelBuilder) -> Tuple[Any, List[str]]:
-    """Resolve abstract and lazy parameters,
-    returning the resolved object, and any input parameter keys it references
-
-    Args:
-        arg (_type_): _description_
-        builder (_type_): _description_
-
-    Returns:
-        _type_: _description_
-    """
-    if isinstance(arg, AbstractParameter):
-        pkey = builder.find_key_from_obj(arg)
-        return Variable(pkey, "parameters"), [pkey]
-    elif isinstance(arg, LazyParameter):
-        lazy_p, pkeys = build_lazy_parameter(arg, builder)
-        return Variable(lazy_p._pkey, "parameters"), pkeys
-    elif is_var(arg, "parameters"):
-        return arg, [arg.name]
-    else:
-        return arg, []
-
-
-def concretize_function_args(
-    func_obj: Function, builder: ModelBuilder
-) -> Tuple[Function, List[str]]:
-    args = []
-    all_params = []
-    for a in func_obj.args:
-        arg, pkeys = concretize_arg(a, builder)
-        args.append(arg)
-        all_params += pkeys
-    kwargs = {}
-    for k, v in func_obj.kwargs.items():
-        arg, pkeys = concretize_arg(v, builder)
-        kwargs[k] = arg
-        all_params += pkeys
-    return Function(func_obj.func, args, kwargs), all_params
-
-
-def build_graph_function(func: Function, builder: ModelBuilder) -> Tuple[ModelParameter, List[str]]:
-    func, pkeys = concretize_function_args(func, builder)
-    return GraphFunction(func), pkeys
-
-
 class GraphFunction(ModelParameter):
     def __init__(self, func):
         self.func = func
 
     def get_value(self, time: float, computed_values: dict, parameters: dict):
         sources = dict(
             computed_values=computed_values, parameters=parameters, model_variables={"time": time}
@@ -165,209 +73,219 @@
         has_computed_value = has_computed_value or any(
             [isinstance(arg, ComputedValue) for arg in self.func.kwargs.values()]
         )
 
         return has_time_var or has_computed_value
 
 
-class PyFunction(ModelParameter):
-    def __init__(self, func):
-        self.func = func
+class GraphObjectParameter(ModelParameter):
+    def __init__(self, obj):
+        self.obj = obj
 
     def get_value(self, time: float, computed_values: dict, parameters: dict):
-        return self.func(time, computed_values)
+        sources = dict(
+            computed_values=computed_values,
+            parameters=parameters,
+            model_variables={"time": time, "computed_values": computed_values},
+        )
+        return self.obj.evaluate(**sources)
 
     def __hash__(self):
-        return hash(self.func)
+        return hash(self.obj)
 
-    def __repr__(self):
-        return f"PyFunction: {self.func}"
+    def __eq__(self, other):
+        return self.obj == other.obj
 
     def is_time_varying(self):
         return True
 
 
-def build_compound_parameter(param: Iterable, builder: ModelBuilder = None):
-    param_keys = []
-    subparams = []
-    for sub_param in param:
-        subp, subp_keys = get_modelparameter_from_param(sub_param, builder)
-        subparams += [subp]
-        param_keys += subp_keys
-    return CompoundParameter(subparams), subp_keys
-
-
-class CompoundParameter(ModelParameter):
-    def __init__(self, subparams: Tuple[ModelParameter], builder):
-        self.subparams = subparams
-
-    def get_value(self, time: float, computed_values: dict, parameters: dict):
-        value = self.subparams[0].get_value(time, computed_values, parameters)
-        for subp in self.subparams[1:]:
-            value *= subp.get_value(time, computed_values, parameters)
-        return value
-
-    def __hash__(self):
-        return hash(self.subparams)
-
-    def __repr__(self):
-        return f"CompoundParameter: {self.subparams}"
-
-    def is_time_varying(self):
-        return any([sp.is_time_varying() for sp in self.subparams])
-
-
-def get_modelparameter_from_param(
-    param, builder: ModelBuilder = None, allow_any=False
-) -> Tuple[ModelParameter, List[str]]:
+def get_modelparameter_from_param(param, allow_any=False) -> Tuple[ModelParameter, List[str]]:
     """Create a ModelParameter subclass object that can be called inside a model loop
     (ie time, computed_values and parameters are available)
     These are mostly flow params and adjustments
     Return this object, as well as a list of keys of all parameters found during its
     construction
 
     Args:
         param: Anything that might resolve to a single float
-        builder (ModelBuilder, optional): _description_. Defaults to None.
+        allow_any: Whether to allow any generic data and return as Data
 
     Raises:
         TypeError: Raised if the input param cannot be resolved
 
     Returns:
         The resolved ModelParameter, along with any parameter keys encountered in the resolution
     """
     if isinstance(param, ModelParameter):
         # We've already transformed this parameter
-        return param, []
-    elif isinstance(param, AbstractParameter):
-        if builder is not None:
-            pkey = builder.find_key_from_obj(param)
-            return GraphParameter(pkey), [pkey]
-        else:
-            raise Exception("AbstractParameter encountered with no ModelBuilder for lookup", param)
-    elif isinstance(param, LazyParameter):
-        if builder is not None:
-            return build_lazy_parameter(param, builder)
-        else:
-            raise Exception(
-                "Lazy AbstractParameter encountered with no ModelBuilder for lookup", param
-            )
-    elif is_var(param, "parameters"):
-        return GraphParameter(param.name), [param.name]
-    elif isinstance(param, Function):
-        return build_graph_function(param, builder)
+        return param
+    elif isinstance(param, GraphObject):
+        return GraphObjectParameter(param)
     elif isinstance(param, Real):
-        return FloatParameter(param), []
-    elif isinstance(param, list) or isinstance(param, tuple):
-        return build_compound_parameter(param, builder)
+        return GraphObjectParameter(Data(param))
     elif callable(param):
-        return PyFunction(param), []
+        return GraphObjectParameter(defer(param)(Time, ComputedValuesDict))
     elif isinstance(param, ComputedValue):
-        return ComputedValueParameter(param.name), []
+        raise Exception("Really?")
+        return ComputedValueParameter(param.key), []
     else:
         if allow_any:
-            return DataParameter(param), []
+            return GraphObjectParameter(Data(param))
         else:
             raise TypeError(f"Unsupported model parameter type {type(param)}", param)
 
 
-def replace_with_typed_params(m, builder):
-    # Inside flows
-    for f in m._flows:
-        f.param = get_modelparameter_from_param(f.param, builder)
+def get_reparameterized_dict(d):
+    return {k: get_modelparameter_from_param(v) for k, v in d.items()}
 
-        for adj in f.adjustments:
-            if adj is not None:
-                adj.param = get_modelparameter_from_param(adj.param, builder)
 
-    for k, v in m._derived_output_requests.items():
-        req_type = v["request_type"]
-        if req_type == "param_func":
-            v["func"] = concretize_function_args(v["func"], builder)
-
-    # Inside stratifications - we have retained some useful information...
-    for s in m._stratifications:
-        # Once a model is built, these become meaningless,
-        # so it needs to happen at the start...
-        # Keep this code here for now just in case we want to implement this in a different order
-
-        # Flow adjustments live here quite happily
-        # Flow _parameters_ however are stratified to oblivion, hence the section above ^^^^^
-        for fname, adjustments in s.flow_adjustments.items():
-            for adj, source_strata, dest_strata in adjustments:
-                for k, v in adj.items():
-                    if v is not None:
-                        # Do nothing, reinstate if we reorder this
-                        pass
-                        # v.param = get_modelparameter_from_param(v.param)
+def map_flow_keys(m: CompartmentalModel) -> dict:
+
+    from summer.adjust import Overwrite
+
+    realised_flows = {}
+
+    for i, f in enumerate(m._flows):
+        full_flow = [f.param.obj]
+        for a in f.adjustments:
+            if isinstance(a, Overwrite):
+                full_flow = [a.param.obj]
+            else:
+                full_flow.append(a.param.obj)
+        out_func = full_flow[0]
+        for fparam in full_flow[1:]:
+            out_func = out_func * fparam
+        realised_flows[i] = GraphObjectParameter(out_func)
 
+    return realised_flows
 
-def finalize_parameters(model, builder: ModelBuilder = None):
+
+def finalize_parameters(model):
     """Called as part of model.finalize
     This ensures all parameters (and function calls) have concrete computegraph.Variable
     realisations.  We can scan all possible parameterized sites, and replace params
     with appropriate types, as well as collecting all referenced named parameters
 
     Args:
-        builder: The ModelBuilder responsible for this model
+        model: The CompartmentalModel to finalize
     """
 
-    all_params = []
+    obj_table = {}
+
+    def register_obj_key(obj, base_name, unique=False):
+        if isinstance(obj, dict):
+            for k, v in obj.items():
+                register_obj_key(v, f"{base_name}_{k}")
+        elif isinstance(obj, GraphObjectParameter):
+            if obj.obj not in obj_table:
+                if unique:
+                    name = base_name
+                    if name in obj_table.values():
+                        raise KeyError("Object with name {name} already exists")
+                else:
+                    if base_name in obj_table.values():
+                        name = f"{base_name}_{len(obj_table)}"
+                    else:
+                        name = base_name
+                obj_table[obj.obj] = name
+            obj_key = obj_table[obj.obj]
+            obj._graph_key = obj_key
+            return obj_key
+        else:
+            raise TypeError(obj, base_name)
 
     # Flow parameters and adjustments
     for f in model._flows:
-        f.param, pkeys = get_modelparameter_from_param(f.param, builder)
-        all_params += pkeys
+        f.param = get_modelparameter_from_param(f.param)
 
         for adj in f.adjustments:
             if adj is not None:
-                adj.param, pkeys = get_modelparameter_from_param(adj.param, builder)
-                all_params += pkeys
+                adj.param = get_modelparameter_from_param(adj.param)
+
+    realised_flows = map_flow_keys(model)
+
+    for i, f in enumerate(model._flows):
+        fpkey = register_obj_key(realised_flows[i], f"{f.name}_rate")
+        f._graph_key = fpkey
 
     # Initial population
-    # Can be one of
-    # dict, ParamVariable (or AbstractParameter), or Function
-    if not isinstance(model._initial_population_distribution, dict):
-        param, pkeys = get_modelparameter_from_param(
-            model._initial_population_distribution, builder
-        )
-        model._initial_population_distribution = param
-        all_params += pkeys
+    model._init_pop_dist = get_reparameterized_dict(model._init_pop_dist)
+    register_obj_key(model._init_pop_dist, "init_pop_dist")
 
+    # Keep track of matrices so we can Kron them together later
+    mixing_matrices = []
     # Stratifications - population split, infectiousness adjustments, mixing matrix
     for s in model._stratifications:
-        if not isinstance(s.population_split, dict):
-            param, pkeys = get_modelparameter_from_param(s.population_split, builder)
-            s.population_split = param
-            all_params += pkeys
+        s.population_split = get_reparameterized_dict(s.population_split)
+        register_obj_key(s.population_split, f"{s.name}_pop_split")
 
         for comp, adjustments in s.infectiousness_adjustments.items():
-            for strain, adjustment in adjustments.items():
+            for stratum, adjustment in adjustments.items():
                 if adjustment is not None:
-                    param, pkeys = get_modelparameter_from_param(adjustment.param, builder)
+                    param = get_modelparameter_from_param(adjustment.param)
                     adjustment.param = param
-                    all_params += pkeys
+                    register_obj_key(adjustment.param, f"{s.name}_iadj_{comp}_{stratum}", True)
 
         if s.mixing_matrix is not None:
-            param, pkeys = get_modelparameter_from_param(s.mixing_matrix, builder, True)
+            param = get_modelparameter_from_param(s.mixing_matrix, True)
             s.mixing_matrix = param
-            all_params += pkeys
+            matrix_key = f"{s.name}_mixing_matrix"
+            register_obj_key(s.mixing_matrix, matrix_key, True)
+            mixing_matrices.append(param.obj)
+
+    if len(mixing_matrices) == 0:
+        param = get_modelparameter_from_param(Data(fnp.array([[1.0]])))
+        register_obj_key(param, "mixing_matrix", True)
+        model.mixing_matrix = param
+    elif len(mixing_matrices) == 1:
+        mm = mixing_matrices[0]
+        param = get_modelparameter_from_param(defer(assign)(mm))
+        register_obj_key(param, "mixing_matrix", True)
+        model.mixing_matrix = param
+    else:
 
-    # Computed values
-    cv_graph = {}
+        def compute_final_matrix(base_matrix, *args):
+            cur_matrix = base_matrix
+            for m in args:
+                cur_matrix = fnp.kron(cur_matrix, m)
+            return cur_matrix
+
+        final_mat_func = defer(compute_final_matrix)(*mixing_matrices)
+        param = get_modelparameter_from_param(final_mat_func)
+        model.mixing_matrix = param
+        register_obj_key(param, "mixing_matrix", True)
 
     for k, v in model._computed_values_graph_dict.items():
-        param, pkeys = concretize_function_args(v, builder)
-        cv_graph[k] = param
-        all_params += pkeys
+        name = f"computed_values.{k}"
+        register_obj_key(GraphObjectParameter(v), name, True)
 
-    model._computed_values_graph_dict = cv_graph
+    # Capture computed values in dictionary so that
+    # 'old-style' summer functions (t,cv) can use them
+    def capture_kwargs(*args, **kwargs):
+        return kwargs
 
-    # Derived outputs
-    for k, v in model._derived_output_requests.items():
-        req_type = v["request_type"]
-        if req_type == "param_func":
-            param, pkeys = concretize_function_args(v["func"], builder)
-            v["func"] = param
-            all_params += pkeys
+    cv_func = Function(capture_kwargs, kwargs=model._computed_values_graph_dict)
+    cv_func.node_name = "gather_cv"
+    register_obj_key(GraphObjectParameter(cv_func), "computed_values", True)
+
+    model_graph = invert_dict(obj_table)
+
+    model.graph = ComputeGraph(model_graph)
 
-    return set(all_params)
+    # Computed values
+    # cv_graph = {}
+
+    # for k, v in model._computed_values_graph_dict.items():
+    #    param, pkeys = concretize_function_args(v, builder)
+    #    cv_graph[k] = param
+    #    all_params += pkeys
+
+    # model._computed_values_graph_dict = cv_graph
+
+    # Derived outputs
+    # for k, v in model._derived_output_requests.items():
+    #    req_type = v["request_type"]
+    #    if req_type == "param_func":
+    #        param, pkeys = concretize_function_args(v["func"], builder)
+    #        v["func"] = param
+    #        all_params += pkeys
```

### Comparing `summerepi-4.1.0a0/summer/population.py` & `summerepi-4.2.0a0/summer/population.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     _strata = frozenset(strata.items())
     return [c for c in comps if c._has_strata(_strata)]
 
 
 def get_rebalanced_population(
     model,
     population: np.ndarray,
-    parameters: dict,
+    static_graph_values: dict,
     strat: str,
     dest_filter: dict,
     proportions: dict,
 ):
     """Adjust the initial population to redistribute the population for a particular
     stratification, over a subset of some other strata
 
@@ -54,15 +54,15 @@
     """
 
     msg = f"No stratification {strat} found in model"
     assert strat in [s.name for s in model._stratifications], msg
 
     model_strat = [s for s in model._stratifications if s.name == strat][0]
 
-    proportions = get_static_param_value(proportions, parameters)
+    proportions = get_static_param_value(proportions, static_graph_values)
 
     msg = "All strata must be specified in proportions"
     assert set(model_strat.strata) == set(proportions), msg
 
     msg = "Proportions must sum to 1.0"
     np.testing.assert_allclose(sum(proportions.values()), 1.0, err_msg=msg)
 
@@ -80,7 +80,55 @@
         total = population[idx].sum()
         for c in mcomps:
             k = c.strata[strat]
             target_prop = proportions[k]
             out_population[c.idx] = total * target_prop
 
     return out_population
+
+
+def calculate_initial_population(model, parameters=None) -> np.ndarray:
+    """
+    Called to recalculate the initial population from either fixed dictionary, or a dict
+    supplied as a parameter
+    """
+    if parameters is None:
+        parameters = {}
+    # FIXME:
+    # Work in progress; correctly recalculates non-parameterized
+    # populations, but does not include population rebalances etc
+    distribution = model._init_pop_dist
+    initial_population = np.zeros_like(model._original_compartment_names, dtype=float)
+
+    # if is_var(distribution, "parameters"):
+    #    distribution = self.parameters[distribution.name]
+    # elif isinstance(distribution, Function) or isinstance(distribution, ModelParameter):
+    #    distribution = get_static_param_value(distribution, parameters)
+
+    if isinstance(distribution, dict):
+        for idx, comp in enumerate(model._original_compartment_names):
+            pop = get_static_param_value(distribution[comp.name], parameters, True)
+            assert pop >= 0, f"Population for {comp.name} cannot be negative: {pop}"
+            initial_population[idx] = pop
+
+        comps = model._original_compartment_names
+
+        for action in model.tracker.all_actions:
+            if action.action_type == "stratify":
+                strat = action.kwargs["strat"]
+                # for strat in self.model._stratifications:
+                # Stratify compartments, split according to split_proportions
+                prev_compartment_names = comps  # copy.copy(self.compartments)
+                comps = strat._stratify_compartments(comps)
+                initial_population = strat._stratify_compartment_values(
+                    prev_compartment_names, initial_population, parameters
+                )
+            elif action.action_type == "adjust_pop_split":
+                initial_population = get_rebalanced_population(
+                    model, initial_population, parameters, **action.kwargs
+                )
+        return initial_population
+    else:
+        raise TypeError(
+            "Initial population distribution must be a dict",
+            distribution,
+        )
```

### Comparing `summerepi-4.1.0a0/summer/runner/jax/derived_outputs.py` & `summerepi-4.2.0a0/summer/runner/jax/derived_outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,8 +139,8 @@
             graph_dict[name] = build_computed_value_output(request, name)
         else:
             raise NotImplementedError(request)
         if request["save_results"]:
             out_keys.append(name)
 
     cg = ComputeGraph(graph_dict)
-    return cg.get_callable(False, False, out_keys=out_keys)
+    return cg.get_callable(targets=out_keys)
```

### Comparing `summerepi-4.1.0a0/summer/runner/jax/model_impl.py` & `summerepi-4.2.0a0/summer/runner/jax/model_impl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,100 +1,81 @@
-"""Implementation of CompartmentalModel and ModelRunner internals in Jax
+"""Implementation of CompartmentalModel and ModelBackend internals in Jax
 
 This is a mess right now!
 """
 
 from jax import numpy as jnp
 from summer.runner.jax import ode
 from summer.runner.jax import solvers
 
+from summer.adjust import Overwrite
+
+from summer.runner import ModelBackend
+
 from summer.solver import SolverType
 
 from .stratify import get_calculate_initial_pop
 from .derived_outputs import build_derived_outputs_runner
 
-from summer.parameters import get_model_param_value
-from summer.experimental.abstract_parameter import evaluate_lazy
-
 
 def clean_compartments(compartment_values: jnp.ndarray):
     return jnp.where(compartment_values < 0.0, 0.0, compartment_values)
 
 
-def build_get_mixing_matrix(runner):
-    def get_mixing_matrix(time: float, parameters) -> jnp.ndarray:
-        """
-        Returns the final mixing matrix for a given time.
-        """
-        # We actually have some matrices, let's do things with them...
-        if len(runner.model._mixing_matrices):
-            mixing_matrix = None
-            for mm_func in runner.model._mixing_matrices:
-                # Assume each mixing matrix is either an np.ndarray or
-                # a function of time that returns one.
-                # mm = mm_func(time) if callable(mm_func) else mm_func
-                mm = get_model_param_value(mm_func, time, None, parameters)
-                # mm = mm_func.get_value(time, {}, parameters)
-                # Get Kronecker product of old and new mixing matrices.
-                # Only do this if we actually need to
-                if mixing_matrix is None:
-                    mixing_matrix = mm
-                else:
-                    mixing_matrix = jnp.kron(mixing_matrix, mm)
-        else:
-            mixing_matrix = runner.model._DEFAULT_MIXING_MATRIX
-
-        return mixing_matrix
-
-    return get_mixing_matrix
-
-
 def get_strain_infection_values(
-    compartment_values,
+    strain_infectious_values,
     strain_compartment_infectiousness,
-    category_matrix,
+    strain_category_indexer,
     mixing_matrix,
     category_populations,
 ):
-    infected_values = compartment_values * strain_compartment_infectiousness
-    infectious_populations = category_matrix @ infected_values
+    infected_values = strain_infectious_values * strain_compartment_infectiousness
+    infectious_populations = jnp.sum(infected_values[strain_category_indexer], axis=1)
     infection_density = mixing_matrix @ infectious_populations
     category_prevalence = infectious_populations / category_populations
     infection_frequency = mixing_matrix @ category_prevalence
 
     return {"infection_density": infection_density, "infection_frequency": infection_frequency}
 
 
 def build_get_infectious_multipliers(runner):
-    category_matrix = runner._category_matrix
-    get_mixing_matrix = build_get_mixing_matrix(runner)
+    population_cat_indexer = jnp.array(runner._population_category_indexer)
 
     # FIXME: We are hardcoding this for frequency only right now
     if not runner._infection_frequency_only:
         raise NotImplementedError(
             "Model must have at least one infection frequency flow, and no infection density"
         )
 
     # FIXME: This could desparately use a tidy-up - all the indexing is a nightmare
     def get_infectious_multipliers(
-        time, compartment_values, parameters, compartment_infectiousness
+        time, compartment_values, cur_graph_outputs, compartment_infectiousness
     ):
 
         infection_frequency = {}
         infection_density = {}
 
         full_multipliers = jnp.ones(len(runner.infectious_flow_indices))
 
-        mm = get_mixing_matrix(time, parameters)
-        cat_pops = category_matrix @ compartment_values
+        mixing_matrix = cur_graph_outputs["mixing_matrix"]
+        category_populations = compartment_values[population_cat_indexer].sum(axis=1)
 
         for strain_idx, strain in enumerate(runner.model._disease_strains):
-            strain_infectiousness = compartment_infectiousness[strain]
+
+            strain_compartment_infectiousness = compartment_infectiousness[strain]
+            strain_infectious_idx = runner._strain_infectious_indexers[strain]
+            strain_category_indexer = runner._strain_category_indexers[strain]
+
+            strain_infectious_values = compartment_values[strain_infectious_idx]
             strain_values = get_strain_infection_values(
-                compartment_values, strain_infectiousness, category_matrix, mm, cat_pops
+                strain_infectious_values,
+                strain_compartment_infectiousness,
+                strain_category_indexer,
+                mixing_matrix,
+                category_populations,
             )
             infection_frequency[strain] = strain_values["infection_frequency"]
             infection_density[strain] = strain_values["infection_density"]
 
             strain_ifect = strain_values["infection_frequency"]
 
             # FIXME: So we produce strain infection values _per category_
@@ -125,27 +106,26 @@
             )
 
         return full_multipliers
 
     return get_infectious_multipliers
 
 
-def build_get_flow_weights(runner):
+def build_get_flow_weights(runner: ModelBackend):
+
+    m = runner.model
 
-    flow_block_maps = flatten_fbm(runner.flow_block_maps)
+    def get_flow_weights(cur_graph_outputs):
+
+        flow_weights = jnp.zeros(len(m._flows))
+
+        for i, f in enumerate(m._flows):
+            val = cur_graph_outputs[f._graph_key]
+            flow_weights = flow_weights.at[i].set(val)
 
-    def get_flow_weights(static_flow_weights, computed_values, parameters, time):
-        flow_weights = static_flow_weights.copy()
-        for (param, adjustments, flow_idx) in flow_block_maps:
-            value = param.get_value(time, computed_values, parameters)
-
-            # value = get_model_param_value(param, time, computed_values, parameters, True)
-            for a in adjustments:
-                value = a.get_new_value(value, computed_values, time, parameters)
-            flow_weights = flow_weights.at[flow_idx].set(value)
         return flow_weights
 
     return get_flow_weights
 
 
 def flatten_fbm(flow_block_map):
     out_map = []
@@ -163,58 +143,64 @@
         )
 
         return computed_values
 
     return calc_computed_values
 
 
-def build_get_flow_rates(runner):
+def build_get_flow_rates(runner, ts_graph_func):
 
     calc_computed_values = build_calc_computed_values(runner)
     get_flow_weights = build_get_flow_weights(runner)
     get_infectious_multipliers = build_get_infectious_multipliers(runner)
 
-    flow_weights_base = jnp.array(runner.flow_weights)
+    # flow_weights_base = jnp.array(runner.flow_weights)
 
     population_idx = jnp.array(runner.population_idx)
     infectious_flow_indices = jnp.array(runner.infectious_flow_indices)
 
-    def get_flow_rates(compartment_values: jnp.array, time, parameters, model_data):
+    def get_flow_rates(compartment_values: jnp.array, time, static_graph_vals, model_data):
 
         # COULD BE JITTED
         compartment_values = clean_compartments(compartment_values)
 
         # runner._prepare_time_step(time, compartment_vals)
+        sources = {
+            "model_variables": {"time": time, "compartment_values": compartment_values},
+            "static_inputs": static_graph_vals,
+        }
+
+        cur_graph_outputs = ts_graph_func(**sources)
 
         # JITTED
-        computed_values = calc_computed_values(compartment_values, time, parameters)
+        # computed_values = calc_computed_values(compartment_values, time, parameters)
 
         # JITTED
-        flow_weights = get_flow_weights(flow_weights_base, computed_values, parameters, time)
+        flow_weights = get_flow_weights(cur_graph_outputs)
 
         populations = compartment_values[population_idx]
 
         # Update for special cases (population-independent and CrudeBirth)
         if runner._has_non_pop_flows:
             populations = populations.at[runner._non_pop_flow_idx].set(1.0)
         if runner._has_crude_birth:
             populations = populations.at[runner._crude_birth_idx].set(compartment_values.sum())
 
         flow_rates = flow_weights * populations
 
         # Calculate infection flows
         # JITTED
         infect_mul = get_infectious_multipliers(
-            time, compartment_values, parameters, model_data["compartment_infectiousness"]
+            time, compartment_values, cur_graph_outputs, model_data["compartment_infectiousness"]
         )
         flow_rates = flow_rates.at[infectious_flow_indices].set(
             flow_rates[infectious_flow_indices] * infect_mul
         )
 
-        return flow_rates, computed_values
+        return flow_rates, cur_graph_outputs["computed_values"]
 
     return get_flow_rates
 
 
 def build_get_compartment_rates(runner):
     accum_maps = get_accumulation_maps(runner)
 
@@ -227,20 +213,20 @@
             comp_rates = comp_rates.at[comp_target].add(-flow_rates[flow_src])
 
         return comp_rates
 
     return get_compartment_rates
 
 
-def build_get_rates(runner):
-    get_flow_rates = build_get_flow_rates(runner)
+def build_get_rates(runner, ts_graph_func):
+    get_flow_rates = build_get_flow_rates(runner, ts_graph_func)
     get_compartment_rates = build_get_compartment_rates(runner)
 
-    def get_rates(compartment_values, time, parameters, model_data):
-        flow_rates, _ = get_flow_rates(compartment_values, time, parameters, model_data)
+    def get_rates(compartment_values, time, static_graph_vals, model_data):
+        flow_rates, _ = get_flow_rates(compartment_values, time, static_graph_vals, model_data)
         comp_rates = get_compartment_rates(compartment_values, flow_rates)
 
         return flow_rates, comp_rates
 
     return {"get_flow_rates": get_flow_rates, "get_rates": get_rates}
 
 
@@ -267,139 +253,153 @@
             sources, targets, remainder = peel_flow_map(remainder)
             full_map.append((sources, targets))
         return full_map
 
     return {"positive": recurse_unpeel(pos_map), "negative": recurse_unpeel(neg_map)}
 
 
-def build_get_compartment_infectiousness_for_strain(model, strain: str):
+def build_get_compartment_infectiousness(model):
     """
     Build a Jax function to return the compartment infectiousness (for all compartments),
     of the strain specified by strain
     """
-    # Figure out which compartments should be infectious
-
-    infectious_mask = jnp.array(
-        [c.has_name_in_list(model._infectious_compartments) for c in model.compartments]
-    )
 
     # This is run during prepare_dynamic
     # i.e. it is done once at the start of a model run, but
     # is parameterized (non-structural)
-    def get_compartment_infectiousness_for_strain(parameters):
+    def get_compartment_infectiousness(static_graph_values):
         # Find the infectiousness multipliers for each compartment being implemented in the model.
-        # Start from assumption that each compartment is not infectious.
-        compartment_infectiousness = jnp.zeros(len(model.compartments))
-        # Set all infectious compartments to be equally infectious.
-        compartment_infectiousness = compartment_infectiousness.at[infectious_mask].set(1.0)
-
-        # Apply infectiousness adjustments.
-        for idx, comp in enumerate(model.compartments):
-            inf_value = compartment_infectiousness[idx]
-            for strat in model._stratifications:
-                for comp_name, adjustments in strat.infectiousness_adjustments.items():
-                    if comp_name == comp.name:
-                        for stratum, adjustment in adjustments.items():
-                            should_apply_adjustment = adjustment and comp.has_stratum(
-                                strat.name, stratum
-                            )
-                            if should_apply_adjustment:
-                                # Cannot use time-varying functions for infectiousness adjustments,
-                                # because this is calculated before the model starts running.
-                                inf_value = adjustment.get_new_value(
-                                    inf_value, None, None, parameters
-                                )
-
-            compartment_infectiousness = compartment_infectiousness.at[idx].set(inf_value)
-
-        if strain != model._DEFAULT_DISEASE_STRAIN:
-            # FIXME: If there are multiple strains, but one of them is _DEFAULT_DISEASE_STRAIN
-            # there will almost certainly be incorrect masks applied
-            # Filter out all values that are not in the given strain.
-            strain_mask = jnp.zeros(len(model.compartments))
-            for idx, compartment in enumerate(model.compartments):
-                if compartment.has_stratum("strain", strain):
-                    strain_mask = strain_mask.at[idx].set(1.0)
-
-            compartment_infectiousness = compartment_infectiousness * strain_mask
-
-        return compartment_infectiousness
-
-    return get_compartment_infectiousness_for_strain
-
-
-def build_compartment_infectiousness_calc(model):
-    """Build a functioning return the compartment infectiousness for _all_ strains in the model"""
-    strain_funcs = {}
-    for strain in model._disease_strains:
-        strain_funcs[strain] = build_get_compartment_infectiousness_for_strain(model, strain)
+        compartment_infectiousness = jnp.ones(len(model.compartments))
+
+        # Apply infectiousness adjustments
+        for strat in model._stratifications:
+            for comp_name, adjustments in strat.infectiousness_adjustments.items():
+                for stratum, adjustment in adjustments.items():
+                    if adjustment:
+                        is_overwrite = isinstance(adjustment, Overwrite)
+                        adj_value = static_graph_values[adjustment.param._graph_key]
+                        adj_comps = model.get_matching_compartments(
+                            comp_name, {strat.name: stratum}
+                        )
+                        for c in adj_comps:
+                            if is_overwrite:
+                                compartment_infectiousness = compartment_infectiousness.at[
+                                    c.idx
+                                ].set(adj_value)
+                            else:
+                                orig_value = compartment_infectiousness[c.idx]
+                                compartment_infectiousness = compartment_infectiousness.at[
+                                    c.idx
+                                ].set(adj_value * orig_value)
+
+        strain_comp_inf = {}
 
-    def get_compartment_infectiousness(parameters):
-        compartment_infectiousness = {}
         for strain in model._disease_strains:
-            compartment_infectiousness[strain] = strain_funcs[strain](parameters)
-        return compartment_infectiousness
+            if "strain" in model.stratifications:
+                strain_filter = {"strain": strain}
+            else:
+                strain_filter = {}
+
+            # _Must_ be ordered here
+            strain_infect_comps = model.query_compartments(
+                strain_filter, tags="infectious", as_idx=True
+            )
+
+            strain_comp_inf[strain] = compartment_infectiousness[strain_infect_comps]
+
+        return strain_comp_inf
 
     return get_compartment_infectiousness
 
 
-def build_run_model(runner, solver=None):
-    rates_funcs = build_get_rates(runner)
+def build_run_model(runner, base_params=None, dyn_params=None, solver=None):
+
+    if dyn_params is None:
+        dyn_params = runner.model.graph.get_input_variables()
+    else:
+        dyn_params = [
+            f"parameters.{p}" if not p.startswith("parameters.") else p for p in dyn_params
+        ]
+
+    # Graph frozen for all non-calibration parameters
+    if base_params is None:
+        base_params = {}
+
+    source_inputs = {"parameters": base_params}
+
+    ts_vars = runner.model.graph.query("model_variables")
+
+    dyn_params = set(dyn_params).union(set(ts_vars))
+
+    param_frozen_cg = runner.model.graph.freeze(dyn_params, source_inputs)
+
+    # static_cg = param_frozen_cg.filter(exclude=ts_vars)
+    # static_graph_func = static_cg.get_callable()(parameters=base_params)
+
+    timestep_cg, static_cg = param_frozen_cg.freeze(ts_vars)
+
+    timestep_graph_func = timestep_cg.get_callable()
+    static_graph_func = static_cg.get_callable()
+
+    rates_funcs = build_get_rates(runner, timestep_graph_func)
     get_rates = rates_funcs["get_rates"]
     get_flow_rates = rates_funcs["get_flow_rates"]
 
     from jax import vmap
 
     get_flows_for_outputs = vmap(get_flow_rates, in_axes=(0, 0, None, None), out_axes=(0))
 
-    def get_comp_rates(comp_vals, t, parameters, model_data):
-        return get_rates(comp_vals, t, parameters, model_data)[1]
+    def get_comp_rates(comp_vals, t, static_graph_vals, model_data):
+        return get_rates(comp_vals, t, static_graph_vals, model_data)[1]
 
     if solver is None or solver == SolverType.SOLVE_IVP:
         solver = SolverType.ODE_INT
 
     if solver == SolverType.ODE_INT:
 
-        def get_ode_solution(initial_population, times, parameters, model_data):
-            return ode.odeint(get_comp_rates, initial_population, times, parameters, model_data)
+        def get_ode_solution(initial_population, times, static_graph_vals, model_data):
+            return ode.odeint(
+                get_comp_rates, initial_population, times, static_graph_vals, model_data
+            )
 
     elif solver == SolverType.RUNGE_KUTTA:
 
-        def get_ode_solution(initial_population, times, parameters, model_data):
-            return solvers.rk4(get_comp_rates, initial_population, times, parameters, model_data)
+        def get_ode_solution(initial_population, times, static_graph_vals, model_data):
+            return solvers.rk4(
+                get_comp_rates, initial_population, times, static_graph_vals, model_data
+            )
 
     elif solver == SolverType.EULER:
 
-        def get_ode_solution(initial_population, times, parameters, model_data):
-            return solvers.euler(get_comp_rates, initial_population, times, parameters, model_data)
+        def get_ode_solution(initial_population, times, static_graph_vals, model_data):
+            return solvers.euler(
+                get_comp_rates, initial_population, times, static_graph_vals, model_data
+            )
 
     else:
         raise NotImplementedError("Incompatible SolverType for Jax runner", solver)
 
     times = jnp.array(runner.model.times)
 
     calc_initial_pop = get_calculate_initial_pop(runner.model)
-    get_compartment_infectiousness = build_compartment_infectiousness_calc(runner.model)
+    get_compartment_infectiousness = build_get_compartment_infectiousness(runner.model)
 
     calc_derived_outputs = build_derived_outputs_runner(runner.model)
 
     def run_model(parameters):
-        lazy_parameters = {
-            f"_lazy_{hash(p)}": evaluate_lazy(p, parameters) for p in runner.model._lazy_params
-        }
 
-        parameters.update(lazy_parameters)
+        static_graph_vals = static_graph_func(parameters=parameters)
+        initial_population = calc_initial_pop(static_graph_vals)
 
-        initial_population = calc_initial_pop(parameters)
-        compartment_infectiousness = get_compartment_infectiousness(parameters)
+        compartment_infectiousness = get_compartment_infectiousness(static_graph_vals)
         model_data = {"compartment_infectiousness": compartment_infectiousness}
 
-        outputs = get_ode_solution(initial_population, times, parameters, model_data)
+        outputs = get_ode_solution(initial_population, times, static_graph_vals, model_data)
 
-        out_flows, out_cv = get_flows_for_outputs(outputs, times, parameters, model_data)
+        out_flows, out_cv = get_flows_for_outputs(outputs, times, static_graph_vals, model_data)
 
         model_variables = {"outputs": outputs, "flows": out_flows, "computed_values": out_cv}
 
         derived_outputs = calc_derived_outputs(
             parameters=parameters, model_variables=model_variables
         )
         # return {"outputs": outputs, "model_data": model_data}
@@ -409,10 +409,14 @@
         "get_rates": get_rates,
         "get_flow_rates": get_flow_rates,
         "get_comp_rates": get_comp_rates,
         "calc_initial_pop": calc_initial_pop,
         "get_compartment_infectiousness": get_compartment_infectiousness,
         "get_ode_solution": get_ode_solution,
         "calc_derived_outputs": calc_derived_outputs,
+        "timestep_graph_func": timestep_graph_func,
+        "timestep_cg": timestep_cg,
+        "static_cg": static_cg,
+        "static_graph_func": static_graph_func,
     }
 
     return run_model, runner_dict
```

### Comparing `summerepi-4.1.0a0/summer/runner/jax/ode.py` & `summerepi-4.2.0a0/summer/runner/jax/ode.py`

 * *Files identical despite different names*

### Comparing `summerepi-4.1.0a0/summer/runner/jax/solvers.py` & `summerepi-4.2.0a0/summer/runner/jax/solvers.py`

 * *Files identical despite different names*

### Comparing `summerepi-4.1.0a0/summer/runner/jax/stratify.py` & `summerepi-4.2.0a0/summer/runner/jax/stratify.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     """Build the equivalent of self._stratify_compartment_values for a given Stratification
 
     Args:
         strat (Stratification): The stratification to build this for
         input_comps (List[str]): The list of input compartments (pre-stratification)
     """
 
-    def stratify_compartment_values(comp_values: jnp.ndarray, parameters: dict = None):
+    def stratify_compartment_values(comp_values: jnp.ndarray, static_graph_values: dict = None):
         """
         Stratify the model compartments into sub-compartments, based on the strata names provided.
         Split the population according to the provided proportions.
         Only compartments specified in the stratification's definition will be stratified.
         Returns the new compartment values.
         """
         new_comp_values = []
 
-        population_split = get_static_param_value(strat.population_split, parameters)
+        population_split = get_static_param_value(strat.population_split, static_graph_values)
 
         for idx in range(len(comp_values)):
             should_stratify = input_comps[idx].has_name_in_list(strat.compartments)
             if should_stratify:
                 for stratum in strat.strata:
                     new_value = comp_values[idx] * population_split[stratum]
                     new_comp_values.append(new_value)
@@ -62,39 +62,34 @@
 
     strat_funcs = {}
     comps = model._original_compartment_names
     for strat in model._stratifications:
         strat_funcs[strat] = get_stratify_compartments_func(strat, comps)
         comps = strat._stratify_compartments(comps)
 
-    def calculate_initial_population(parameters: dict) -> jnp.ndarray:
+    def calculate_initial_population(static_graph_values: dict) -> jnp.ndarray:
         """
         Called to recalculate the initial population from either fixed dictionary, or a dict
         supplied as a parameter
         """
         # FIXME:
         # Work in progress; correctly recalculates non-parameterized
         # populations, but does not include population rebalances etc
-        distribution = model._initial_population_distribution
+        distribution = model._init_pop_dist
         initial_population = jnp.zeros(len(model._original_compartment_names))
 
-        if is_var(distribution, "parameters"):
-            distribution = parameters[distribution.name]
-        elif isinstance(distribution, Function) or isinstance(distribution, ModelParameter):
-            distribution = get_static_param_value(distribution, parameters)
-
         if isinstance(distribution, dict):
             for idx, comp in enumerate(model._original_compartment_names):
-                pop = distribution.get(comp.name, 0)
+                pop = get_static_param_value(distribution[comp.name], static_graph_values)
                 initial_population = initial_population.at[idx].set(pop)
 
             for action in model.tracker.all_actions:
                 if action.action_type == "stratify":
                     strat = action.kwargs["strat"]
-                    initial_population = strat_funcs[strat](initial_population, parameters)
+                    initial_population = strat_funcs[strat](initial_population, static_graph_values)
                 elif action.action_type == "adjust_pop_split":
                     # FIXME: Implement this
                     raise NotImplementedError
                     # initial_population = get_rebalanced_population(
                     #    model, initial_population, parameters, **action.kwargs
                     # )
             return initial_population
```

### Comparing `summerepi-4.1.0a0/summer/runner/model_runner.py` & `summerepi-4.2.0a0/summer/runner/model_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,323 +1,365 @@
-from abc import ABC, abstractmethod
 from typing import Tuple
 
 import numpy as np
-from computegraph.graph import ComputeGraph
 
-from computegraph.utils import is_var
-
-import summer.flows as flows
+from summer import Compartment
 from summer.adjust import Overwrite
-from summer.compute import binary_matrix_to_sparse_pairs, sparse_pairs_accum
-from summer.compartment import Compartment
-from summer.population import get_rebalanced_population
+import summer.flows as flows
 
-from summer.parameters import get_model_param_value, get_static_param_value, is_var, Function
-from summer.parameters.param_impl import ModelParameter
+from summer.population import get_rebalanced_population
+from summer.compute import (
+    accumulate_positive_flow_contributions,
+    accumulate_negative_flow_contributions,
+    find_sum,
+    get_strain_infection_values,
+)
+from summer.utils import clean_compartment_values
 
 
-class ModelRunner(ABC):
+class ModelBackend:
     """
-    Base runner.
-    Child classes may be used by the CompartmentalModel to calculate flow rates.
+    An optimized, but less accessible model runner.
     """
 
-    def __init__(self, model):
+    def __init__(self, model, jit=False):
         # Compartmental model
         self.model = model
 
+        self._jit = jit
+
         # Tracks total deaths per timestep for death-replacement birth flows
         self._timestep_deaths = None
 
         # Set our initial parameters to an empty dict - this is really just to appease tests
         self.parameters = {}
 
-    @abstractmethod
-    def get_flow_rates(self, compartment_values: np.ndarray, time: float) -> np.ndarray:
-        """
-        Returns the contribution of each flow to compartment rate of change for a given state and
-        time.
+    def prepare_structural(self):
+        # FIXME: Redundant
+        self._iter_non_function_flows = [(i, f) for i, f in enumerate(self.model._flows)]
 
-        Args:
-            compartment_values (np.ndarray): Current values of the model compartments
-            time (float): Time at which rates are evaluated (expected to be in range of model.times)
+        self._build_compartment_category_map()
 
-        Returns:
-            np.ndarray: Array of flow rates (size determined by number of model flows)
-        """
-        pass
+        self.infectious_flow_indices = np.array(
+            [i for i, f in self._iter_non_function_flows if isinstance(f, flows.BaseInfectionFlow)],
+            dtype=int,
+        )
+        self.death_flow_indices = np.array(
+            [i for i, f in self._iter_non_function_flows if f.is_death_flow], dtype=int
+        )
 
-    @abstractmethod
-    def get_compartment_rates(self, compartment_values: np.ndarray, time: float) -> np.ndarray:
-        """
-        Interface for the ODE solver: this function is passed to solve_ode func and defines the
-        dynamics of the model.
+        # Include dummy values in population_idx to account for Entry flows
+        non_func_pops = np.array(
+            [f.source.idx if f.source else 0 for i, f in self._iter_non_function_flows], dtype=int
+        )
 
+        self.population_idx = non_func_pops
 
-        Args:
-            compartment_values (np.ndarray): Current values of the model compartments
-            time (float): Time (in model.times coordinates) at which current step is being solved
+        # Store indices of flows that are not population dependent
+        self._non_pop_flow_idx = np.array(
+            [
+                i
+                for i, f in self._iter_non_function_flows
+                if (type(f) in (flows.ReplacementBirthFlow, flows.ImportFlow, flows.AbsoluteFlow))
+            ],
+            dtype=int,
+        )
+        self._has_non_pop_flows = bool(len(self._non_pop_flow_idx))
 
-        Returns:
-            np.ndarray: Rates of change for the compartment values for a given state and time.
-        """
-        pass
+        # Crude birth flows use population sum rather than a compartment; store indices here
+        self._crude_birth_idx = np.array(
+            [i for i, f in self._iter_non_function_flows if type(f) == flows.CrudeBirthFlow],
+            dtype=int,
+        )
+        self._has_crude_birth = bool(len(self._crude_birth_idx))
 
-    def _clean_compartment_values(self, compartment_values: np.ndarray):
-        """
-        Zero out -ve compartment sizes in flow rate calculations,
-        to prevent negative values from messing up the direction of flows.
-        We don't expect large -ve values, but there can be small ones due to numerical errors.
-        """
-        comp_vals = compartment_values.copy()
-        zero_mask = comp_vals < 0
-        comp_vals[zero_mask] = 0
-        return comp_vals
+        self._has_replacement = False
+        # Replacement flows must be calculated after death flows, store indices here
+        for i, f in self._iter_non_function_flows:
+            if type(f) == flows.ReplacementBirthFlow:
+                self._has_replacement = True
+                self._replacement_flow_idx = i
 
-    @abstractmethod
-    def prepare_structural(self):
-        # Re-order flows so that they are executed in the correct order:
-        #   - exit flows
-        #   - entry flows (depends on exit flows for 'replace births' functionality)
-        #   - transition flows
-        #   - function flows (depend on all other prior flows, since they take flow rate as an
-        # input)
-        num_flows = len(self.model._flows)
-        _exit_flows = [f for f in self.model._flows if issubclass(f.__class__, flows.BaseExitFlow)]
-        _entry_flows = [
-            f for f in self.model._flows if issubclass(f.__class__, flows.BaseEntryFlow)
-        ]
-        _transition_flows = [
-            f
-            for f in self.model._flows
-            if issubclass(f.__class__, flows.BaseTransitionFlow)
-            and not isinstance(f, flows.FunctionFlow)
-        ]
-        _function_flows = [f for f in self.model._flows if isinstance(f, flows.FunctionFlow)]
-        self._has_function_flows = bool(_function_flows)
-        self.model._flows = _exit_flows + _entry_flows + _transition_flows + _function_flows
-        # Check we didn't miss any flows
-        assert len(self.model._flows) == num_flows, "Some flows were lost when preparing to run."
-
-        # Simplify adjustments; if there are any overwrites, we can discard the previous
-        # adjustments
-        # FIXME: Currently only works if the last adjustment is an Overwrite
-        # Probably expand this to an optimizations module
-        for f in self.model._flows:
-            if len(f.adjustments) and isinstance(f.adjustments[-1], Overwrite):
-                f.adjustments = [f.adjustments[-1]]
-
-        # Split flows into two groups for runtime.
-        self._iter_function_flows = [
-            (i, f) for i, f in enumerate(self.model._flows) if isinstance(f, flows.FunctionFlow)
-        ]
-        self._iter_non_function_flows = [
-            (i, f) for i, f in enumerate(self.model._flows) if not isinstance(f, flows.FunctionFlow)
-        ]
+        self._precompute_flow_maps()
+        self._build_infectious_multipliers_lookup()
 
-        for k, proc in self.model._computed_value_processors.items():
-            proc.prepare_to_run(self.model.compartments, self.model._flows)
+    def prepare_static_params(self, parameters: dict, dyn_params: list = None):
+        """Do all precomputation here"""
 
-        cvcg = ComputeGraph(self.model._computed_values_graph_dict, "computed_values")
+        parameters = parameters or {}
+        self.parameters = parameters
 
-        self.computed_values_runner = cvcg.get_callable(nested_params=False)
+        #
+        source_inputs = {"parameters": parameters}
 
-        # Create a matrix that tracks which categories each compartment is in.
-        # A matrix with size (num_cats x num_comps).
-        # This is a very sparse static matrix, and there's almost certainly a much
-        # faster way of using it than naive matrix multiplication
-        num_comps = len(self.model.compartments)
-        self.num_categories = len(self.model._mixing_categories)
-        self._category_lookup = {}  # Map compartments to categories.
-        self._category_matrix = np.zeros((self.num_categories, num_comps))
-        for i, category in enumerate(self.model._mixing_categories):
-            for j, comp in enumerate(self.model.compartments):
-                if all(comp.has_stratum(k, v) for k, v in category.items()):
-                    self._category_matrix[i][j] = 1
-                    self._category_lookup[j] = i
-        self._compartment_category_map = binary_matrix_to_sparse_pairs(self._category_matrix)
+        # Can replace this with calibration parameters later
+        if dyn_params is None:
+            dyn_vars = self.model.graph.get_input_variables()
+        else:
+            dyn_vars = dyn_params
 
-    @abstractmethod
-    def prepare_dynamic(self, parameters: dict = None):
+        # Graph frozen for all non-calibration parameters
+        self.param_frozen_cg = self.model.graph.freeze(dyn_vars, source_inputs)
 
-        # Calculate initial population based on possible parameterization
-        self.parameters = parameters
-        self.model.initial_population = self.calculate_initial_population(self.parameters)
+        # Query model_variables (ie time-varying sources)
+        ts_vars = self.param_frozen_cg.query("model_variables")
 
-        """
-        Pre-run calculations to help determine force of infection multiplier at runtime.
+        # Subgraph that does not contain model_variables (ie anything time varying)
+        self.static_cg = self.param_frozen_cg.filter(exclude=ts_vars)
+        self.run_graph_static = self.static_cg.get_callable()
 
-        We start with a set of "mixing categories". These categories describe groups of
-        compartments.
-        For example, we might have the stratifications age {child, adult} and location {work, home}.
-        In this case, the mixing categories would be
-            {child x home, child x work, adult x home, adult x work}.
-        Mixing categories are only created when a mixing matrix is supplied during stratification.
-
-        There is a mapping from every compartment to a mixing category.
-        This is only true if mixing matrices are supplied only for complete stratifications.
-        There are `num_cats` categories and `num_comps` compartments.
-        The category matrix is a (num_cats x num_comps) matrix of 0s and 1s, with a 1 when the
-        compartment is in a given category.
-        We expect only one category per compartment, but there may be many compartments per
-        category.
-
-        We can multiply the category matrix by the vector of compartment sizes to get the total
-        number of people in each mixing category.
-
-        We also create a vector of values in [0, inf) which describes how infectious each
-        compartment is: compartment_infectiousness
-        We can use this vector plus the compartment sizes to get the 'effective' number of
-        infectious people per compartment.
-
-        We can use the 'effective infectious' compartment sizes, plus the mixing category matrix
-        to get the infected population per mixing category.
-
-        Now that we know:
-            - the total population per category
-            - the infected population per category
-            - the inter-category mixing coefficients (mixing matrix)
-
-        We can calculate infection density or infection frequency transition flows for each
-        category.
-        Finally, at runtime, we can lookup which category a given compartment is in and look up its
-        infectious multiplier (density or frequency).
-        """
-
-        # Find out the relative infectiousness of each compartment, for each strain.
-        # If no strains have been created, we assume a default strain name.
-        self._compartment_infectiousness = {
-            strain_name: self._get_compartment_infectiousness_for_strain(strain_name)
-            for strain_name in self.model._disease_strains
-        }
+    def prepare_dynamic(self, param_updates: dict = None):
+        """Do all precomputation here"""
+
+        param_updates = param_updates or {}
+
+        self.parameters.update(param_updates)
+
+        #
+        source_inputs = {"parameters": self.parameters}
+
+        # Query model_variables (ie time-varying sources)
+        ts_vars = self.param_frozen_cg.query("model_variables")
+
+        self._graph_values_static = self.run_graph_static(parameters=self.parameters)
+
+        # Subgraph whose only dynamic inputs are model_variables
+        self.timestep_cg = self.param_frozen_cg.freeze(ts_vars, source_inputs)
+
+        self.run_graph_ts = self.timestep_cg.get_callable()
+
+        # Must be run after self._graph_values_static is available
+        self.calculate_initial_population()
+
+        self._compartment_infectiousness = self._get_compartment_infectiousness()
+
+        # Initialize arrays for infectious multipliers
+        # FIXME Put this in its own function, this is getting messy again
+        num_cats = self.num_categories
+        num_strains = len(self.model._disease_strains)
+        self._infection_density = {}
+        self._infection_frequency = {}
+        self._infection_density_flat = np.empty((num_strains, num_cats), dtype=float)
+        self._infection_frequency_flat = np.empty((num_strains, num_cats), dtype=float)
 
-    # FIXME:
-    # This is now only used by tests, and should never called in any production code
     def prepare_to_run(self, parameters: dict = None):
+        # FIXME:
+        # This is now only used by tests, and should never called in any production code
+        if not hasattr(self.model, "_init_pop_dist"):
+            self.model.set_initial_population({}, force=True)
         self.model.finalize()
         self.prepare_structural()
-        self.prepare_dynamic(parameters)
+        self.prepare_static_params(parameters)
+        self.prepare_dynamic({})
 
-    def _get_compartment_infectiousness_for_strain(self, strain: str):
-        """
-        Returns a vector of floats, each representing the relative infectiousness of each
-        compartment.
-        If a strain name is provided, find the infectiousness factor *only for that strain*.
+    def _build_compartment_category_map(self):
+        # Create a matrix that tracks which categories each compartment is in.
+        self.num_categories = ncats = len(self.model._mixing_categories)
+
+        # Array that maps compartments to their mixing category
+        self._category_lookup = np.empty(len(self.model.compartments), dtype=int)
+
+        all_cat_idx = []
+        for i, category in enumerate(self.model._mixing_categories):
+            cat_idx = []
+            for j, comp in enumerate(self.model.compartments):
+                if all(comp.has_stratum(k, v) for k, v in category.items()):
+                    cat_idx.append(j)
+                    # self._category_matrix[i][j] = 1
+                    self._category_lookup[j] = i
+            all_cat_idx.append(np.array(cat_idx, dtype=int))
+
+        # Indexer for whole population (compartment_values), that will return a
+        # num_cats * (num_comps_per_cat) array that can be summed for category populations
+        self._population_category_indexer = pop_cat_idx = np.stack(all_cat_idx)
+
+        # Array (per-strain) of compartment indices for that strain's infectious compartments
+        self._strain_infectious_indexers = {}
+        # Array (per-strain) of len (strain infectious comps) that maps each
+        # strain infectious compartment to its mixing category
+        self._strain_category_indexers = {}
+        #
+        for strain in self.model._disease_strains:
+            strain_filter = {"strain": strain} if "strain" in self.model.stratifications else {}
+            strain_infectious_comps = self.model.query_compartments(
+                strain_filter, tags="infectious", as_idx=True
+            )
+            self._strain_infectious_indexers[strain] = strain_infectious_comps
+
+            # Function that tests each element of an ndarray to see if is contained within the
+            # current strain infectious compartments
+            vcat = np.vectorize(lambda c: c in strain_infectious_comps)
+            strain_cat_idx = pop_cat_idx[vcat(pop_cat_idx)]
+            # Localize the compartment indices to be within strain infectious comps,
+            # rather than the global compartment lookup
+            # We do this by creating an inverse global map (but only fill in the compartment
+            # indices we care about)
+            # It's just a bit easier to read that messing around with dictionaries etc
+            tlookup = np.empty(len(self.model.compartments), dtype=int)
+            tlookup[strain_infectious_comps] = range(len(strain_infectious_comps))
+            strain_cat_idx = tlookup[strain_cat_idx]
+
+            # Ensure this is a 2d array
+            # This necessary where there is only one compartment for each category
+            strain_cat_idx = strain_cat_idx.reshape((ncats, int(strain_cat_idx.size / ncats)))
+            self._strain_category_indexers[strain] = strain_cat_idx
+
+    def _get_compartment_infectiousness(self):
+        """
+        Returns an array of relative infectiousness weights for the supplied strain
+        The returned array is of size num_infectious_comps_for_strain, and is ordered
+        (ie can be multiplied directly against these infectious compartments)
         """
-        # Figure out which compartments should be infectious
-        infectious_mask = np.array(
-            [
-                c.has_name_in_list(self.model._infectious_compartments)
-                for c in self.model.compartments
-            ]
-        )
         # Find the infectiousness multipliers for each compartment being implemented in the model.
         # Start from assumption that each compartment is not infectious.
-        compartment_infectiousness = np.zeros(self.model.initial_population.shape)
+        compartment_infectiousness = np.ones(self.model.initial_population.shape)
         # Set all infectious compartments to be equally infectious.
-        compartment_infectiousness[infectious_mask] = 1
 
-        # Apply infectiousness adjustments.
-        for idx, comp in enumerate(self.model.compartments):
-            inf_value = compartment_infectiousness[idx]
-            for strat in self.model._stratifications:
-                # strat_fs = frozenset({strat.name})
-                for comp_name, adjustments in strat.infectiousness_adjustments.items():
-                    if comp_name == comp.name:
-                        for stratum, adjustment in adjustments.items():
-                            should_apply_adjustment = adjustment and comp.has_stratum(
-                                strat.name, stratum
-                            )
-                            if should_apply_adjustment:
-                                # Cannot use time-varying functions for infectiousness adjustments,
-                                # because this is calculated before the model starts running.
-                                inf_value = adjustment.get_new_value(
-                                    inf_value, None, None, self.parameters
-                                )
-
-            compartment_infectiousness[idx] = inf_value
-
-        if strain != self.model._DEFAULT_DISEASE_STRAIN:
-            # FIXME: If there are multiple strains, but one of them is _DEFAULT_DISEASE_STRAIN
-            # there will almost certainly be incorrect masks applied
-            # Filter out all values that are not in the given strain.
-            strain_mask = np.zeros(self.model.initial_population.shape)
-            for idx, compartment in enumerate(self.model.compartments):
-                if compartment.has_stratum("strain", strain):
-                    strain_mask[idx] = 1
+        for strat in self.model._stratifications:
+            for comp_name, adjustments in strat.infectiousness_adjustments.items():
+                for stratum, adjustment in adjustments.items():
+                    if adjustment:
+                        is_overwrite = isinstance(adjustment, Overwrite)
+                        adj_value = self._graph_values_static[adjustment.param._graph_key]
+                        adj_comps = self.model.get_matching_compartments(
+                            comp_name, {strat.name: stratum}
+                        )
+                        for c in adj_comps:
+                            if is_overwrite:
+                                compartment_infectiousness[c.idx] = adj_value
+                            else:
+                                orig_value = compartment_infectiousness[c.idx]
+                                compartment_infectiousness[c.idx] = adj_value * orig_value
+
+        strain_comp_inf = {}
+
+        for strain in self.model._disease_strains:
+            if "strain" in self.model.stratifications:
+                strain_filter = {"strain": strain}
+            else:
+                strain_filter = {}
+
+            # _Must_ be ordered here
+            strain_infect_comps = self.model.query_compartments(
+                strain_filter, tags="infectious", as_idx=True
+            )
+
+            strain_comp_inf[strain] = compartment_infectiousness[strain_infect_comps]
 
-            compartment_infectiousness *= strain_mask
+        return strain_comp_inf
 
-        return compartment_infectiousness
+    def _precompute_flow_maps(self):
+        """Build fast-access arrays of flow indices"""
+        f_pos_map = []
+        f_neg_map = []
+        for i, f in self._iter_non_function_flows:
+            if f.source:
+                f_neg_map.append((i, f.source.idx))
+            if f.dest:
+                f_pos_map.append((i, f.dest.idx))
 
-    def _calculate_strain_infection_values(
-        self, compartment_values: np.ndarray, mixing_matrix: np.ndarray
-    ):
-        num_cats = self.num_categories
-        num_strains = len(self.model._disease_strains)
-        # Calculate total number of people per category (for FoI).
-        # A vector with size (num_cats).
-        self._category_populations = sparse_pairs_accum(
-            self._compartment_category_map, compartment_values, num_cats
+        self._pos_flow_map = np.array(f_pos_map, dtype=np.int)
+        self._neg_flow_map = np.array(f_neg_map, dtype=np.int)
+
+    def _prepare_time_step(self, time: float, compartment_values: np.ndarray):
+        """
+        Pre-timestep setup. This should be run before `_get_rates`.
+        Here we set up any stateful updates that need to happen before we get the flow rates.
+        """
+
+        # Some flows (e.g birth replacement) expect this value to be defined
+        self._timestep_deaths = 0.0
+
+        model_variables = {
+            "time": time,
+            "compartment_values": compartment_values,
+            "computed_values": {},
+        }
+
+        self._graph_values_timestep = self.run_graph_ts(
+            parameters=self.parameters, model_variables=model_variables
         )
 
-        # Calculate infectious populations for each strain.
-        # Infection density/frequency is the infectious multiplier for each mixing category,
-        # calculated for each strain.
-        self._infection_density = {}
-        self._infection_frequency = {}
-        # Flat indices are used for fast vectorized lookups
-        # These are pure arrays rather than <dict, ndarray> types
-        # FIXME+++ We should eventually move everything to these, but the originals are maintained
-        # because they are much better tested, and we can demonstrate equivalence
-        self._infection_density_flat = np.empty((num_strains, num_cats), dtype=float)
-        self._infection_frequency_flat = np.empty((num_strains, num_cats), dtype=float)
+        # Find the effective infectious population for the force of infection (FoI) calculations.
+        self._mixing_matrix = mixing_matrix = self._graph_values_timestep["mixing_matrix"]
+        self._calculate_strain_infection_values(compartment_values, mixing_matrix)
 
-        for strain_idx, strain in enumerate(self.model._disease_strains):
-            strain_compartment_infectiousness = self._compartment_infectiousness[strain]
+    def _get_mixing_matrix(self, t):
+        # FIXME: Only used by tests, should never be called in real code
+        self.prepare_to_run()
+        self._prepare_time_step(t, self.model.initial_population)
+        return self._mixing_matrix
 
-            # Calculate the effective infectious people for each category, including adjustment
-            # factors.
-            # Returns a vector with size (num_cats x 1).
-            infected_values = compartment_values * strain_compartment_infectiousness
-            infectious_populations = sparse_pairs_accum(
-                self._compartment_category_map, infected_values, num_cats
-            )
-            self._infection_density[strain] = np.matmul(mixing_matrix, infectious_populations)
-            self._infection_density_flat[strain_idx] = self._infection_density[strain]
-            # Calculate the effective infectious person frequency for each category, including
-            # adjustment factors.
-            # A vector with size (num_cats x 1).
-            category_prevalence = infectious_populations / self._category_populations
-            self._infection_frequency[strain] = np.matmul(mixing_matrix, category_prevalence)
-            self._infection_frequency_flat[strain_idx] = self._infection_frequency[strain]
-
-    def _get_mixing_matrix(self, time: float) -> np.ndarray:
-        """
-        Returns the final mixing matrix for a given time.
-        """
-        # We actually have some matrices, let's do things with them...
-        if len(self.model._mixing_matrices):
-            mixing_matrix = None
-            for mm_func in self.model._mixing_matrices:
-                # Assume each mixing matrix is either an np.ndarray or a function of time that
-                # returns one.
-                # mm = mm_func(time) if callable(mm_func) else mm_func
-                mm = get_model_param_value(mm_func, time, None, self.parameters)
-                # Get Kronecker product of old and new mixing matrices.
-                # Only do this if we actually need to
-                if mixing_matrix is None:
-                    mixing_matrix = mm
-                else:
-                    mixing_matrix = np.kron(mixing_matrix, mm)
-        else:
-            mixing_matrix = self.model._DEFAULT_MIXING_MATRIX
+    def get_flow_weights(self):
+        """Collate weights for all model flows at the current timestep"""
+
+        flow_weights = np.zeros(len(self.model._flows))
+
+        for i, f in enumerate(self.model._flows):
+            flow_weights[i] = self._graph_values_timestep[f._graph_key]
+
+        return flow_weights
+
+    def _get_infectious_multipliers(self) -> np.ndarray:
+        """Get multipliers for all infectious flows
+
+        Returns:
+            np.ndarray: Array of infectiousness multipliers
+        """
+        # We can use a fast lookup version if we have only one type of infectious multiplier
+        # (eg only frequency, not mixed freq and density)
+        if self._infection_frequency_only:
+            return self._infection_frequency_flat[
+                self._infect_strain_lookup_idx, self._infect_cat_lookup_idx
+            ]
+        elif self._infection_density_only:
+            return self._infection_density_flat[
+                self._infect_strain_lookup_idx, self._infect_cat_lookup_idx
+            ]
+
+        multipliers = np.empty(len(self.infectious_flow_indices))
+        for i, idx in enumerate(self.infectious_flow_indices):
+            f = self.model._flows[idx]
+            multipliers[i] = f.find_infectious_multiplier(f.source, f.dest)
+        return multipliers
+
+    def _build_infectious_multipliers_lookup(self):
+        """Get multipliers for all infectious flows
+
+        These are used by _get_infectious_multipliers_flat (currently experimental)
 
-        return mixing_matrix
+        Returns:
+            np.ndarray: Array of infectiousness multipliers
+        """
+        lookups = []
+
+        has_freq = False
+        has_dens = False
+
+        for i, idx in enumerate(self.infectious_flow_indices):
+            f = self.model._flows[idx]
+            if isinstance(f, flows.InfectionFrequencyFlow):
+                has_freq = True
+            elif isinstance(f, flows.InfectionDensityFlow):
+                has_dens = True
+            cat_idx, strain = self._get_infection_multiplier_indices(f.source, f.dest)
+            strain_idx = self.model._disease_strains.index(strain)
+            lookups.append([strain_idx, cat_idx])
+        full_table = np.array(lookups, dtype=int)
+        self._full_table = full_table.reshape(len(self.infectious_flow_indices), 2)
+        self._infect_strain_lookup_idx = self._full_table[:, 0].flatten()
+        self._infect_cat_lookup_idx = self._full_table[:, 1].flatten()
+
+        self._infection_frequency_only = False
+        self._infection_density_only = False
+
+        if has_freq and not has_dens:
+            self._infection_frequency_only = True
+        elif has_dens and not has_freq:
+            self._infection_density_only = True
 
     def _get_force_idx(self, source: Compartment):
         """
         Returns the index of the source compartment in the infection multiplier vector.
         """
         return self._category_lookup[source.idx]
 
@@ -345,64 +387,172 @@
         """
         Get force of infection multiplier for a given compartment,
         using the 'infection density' calculation.
         """
         idx, strain = self._get_infection_multiplier_indices(source, dest)
         return self._infection_density[strain][idx]
 
-    def _calc_computed_values(self, compartment_vals: np.ndarray, time: float) -> dict:
-        computed_values = {}
-        for k, proc in self.model._computed_value_processors.items():
-            computed_values[k] = proc.process(compartment_vals, computed_values, time)
+    def _calculate_strain_infection_values(
+        self, compartment_values: np.ndarray, mixing_matrix: np.ndarray
+    ):
+        # Calculate total number of people per category (for FoI).
+        # A vector with size (num_cats).
+        self._category_populations = compartment_values[self._population_category_indexer].sum(
+            axis=1
+        )
+
+        for strain_idx, strain in enumerate(self.model._disease_strains):
 
-        model_variables = {"compartment_values": compartment_vals, "time": time}
+            strain_compartment_infectiousness = self._compartment_infectiousness[strain]
+            strain_infectious_idx = self._strain_infectious_indexers[strain]
+            strain_category_indexer = self._strain_category_indexers[strain]
 
-        computed_values.update(
-            self.computed_values_runner(parameters=self.parameters, model_variables=model_variables)
-        )
+            strain_infectious_values = compartment_values[strain_infectious_idx]
 
-        return computed_values
+            infection_density, infection_frequency = get_strain_infection_values(
+                strain_infectious_values,
+                strain_compartment_infectiousness,
+                strain_category_indexer,
+                mixing_matrix,
+                self._category_populations,
+            )
 
-    def calculate_initial_population(self, parameters) -> np.ndarray:
+            self._infection_density[strain] = infection_density
+            self._infection_density_flat[strain_idx] = infection_density
+
+            self._infection_frequency[strain] = infection_frequency
+            self._infection_frequency_flat[strain_idx] = infection_frequency
+
+    def _get_flow_rates(self, compartment_vals: np.ndarray, time: float) -> np.ndarray:
+        """Get current flow rates, equivalent to calling get_net_flow on all (non-function) flows
+
+        Args:
+            comp_vals (np.ndarray): Compartment values
+            time (float): Time in model.times coordinates
+
+        Returns:
+            np.ndarray: Array of all (non-function) flow rates
+        """
+
+        self._prepare_time_step(time, compartment_vals)
+
+        computed_values = self._graph_values_timestep["computed_values"]
+
+        flow_weights = self.get_flow_weights()
+
+        # These will be filled in afterwards
+        populations = compartment_vals[self.population_idx]
+        # Update for special cases (population-independent and CrudeBirth)
+        if self._has_non_pop_flows:
+            populations[self._non_pop_flow_idx] = 1.0
+        if self._has_crude_birth:
+            populations[self._crude_birth_idx] = find_sum(compartment_vals)
+
+        flow_rates = flow_weights * populations
+
+        # Calculate infection flows
+        infect_mul = self._get_infectious_multipliers()
+        flow_rates[self.infectious_flow_indices] *= infect_mul
+
+        # ReplacementBirthFlow depends on death flows already being calculated; update here
+        if self._has_replacement:
+            # Only calculate timestep_deaths if we use replacement, it's expensive...
+            self._timestep_deaths = flow_rates[self.death_flow_indices].sum()
+            flow_rates[self._replacement_flow_idx] = self._timestep_deaths
+
+        return flow_rates, computed_values
+
+    def _get_rates(self, comp_vals: np.ndarray, time: float) -> Tuple[np.ndarray, np.ndarray]:
+        """Calculates inter-compartmental flow rates for a given state and time, as well
+        as the updated compartment values once these rate deltas have been applied
+
+        Args:
+            comp_vals (np.ndarray): The current state of the model compartments
+                                    (ie. number of people)
+            time (float): Time in model.times coordinates
+
+        Returns:
+            Tuple[np.ndarray, np.ndarray]: (comp_rates, flow_rates) where
+                comp_rates is the rate of change of compartments, and
+                flow_rates is the contribution of each flow to compartment rate of change
+        """
+
+        comp_rates = np.zeros(len(comp_vals))
+        flow_rates, _ = self._get_flow_rates(comp_vals, time)
+
+        if self._pos_flow_map.size > 0:
+            comp_rates = accumulate_positive_flow_contributions(
+                flow_rates, comp_rates, self._pos_flow_map
+            )
+
+        if self._neg_flow_map.size > 0:
+            comp_rates = accumulate_negative_flow_contributions(
+                flow_rates, comp_rates, self._neg_flow_map
+            )
+
+        return comp_rates, flow_rates
+
+    def get_compartment_rates(self, compartment_values: np.ndarray, time: float):
+        """
+        Interface for the ODE solver: this function is passed to solve_ode func and defines the
+        dynamics of the model.
+        Returns the rate of change of the compartment values for a given state and time.
+        """
+        comp_vals = clean_compartment_values(compartment_values)
+        comp_rates, _ = self._get_rates(comp_vals, time)
+        return comp_rates
+
+    def get_flow_rates(self, compartment_values: np.ndarray, time: float):
+        """
+        Returns the contribution of each flow to compartment rate of change for a given state and
+        time.
+        """
+        comp_vals = clean_compartment_values(compartment_values)
+        return self._get_flow_rates(comp_vals, time)
+
+    def calculate_initial_population(self) -> np.ndarray:
         """
         Called to recalculate the initial population from either fixed dictionary, or a dict
         supplied as a parameter
         """
         # FIXME:
         # Work in progress; correctly recalculates non-parameterized
         # populations, but does not include population rebalances etc
-        distribution = self.model._initial_population_distribution
-        initial_population = np.zeros_like(self.model._original_compartment_names, dtype=float)
+        model = self.model
+
+        distribution = model._init_pop_dist
+        initial_population = np.zeros_like(model._original_compartment_names, dtype=float)
 
-        if is_var(distribution, "parameters"):
-            distribution = self.parameters[distribution.name]
-        elif isinstance(distribution, Function) or isinstance(distribution, ModelParameter):
-            distribution = get_static_param_value(distribution, parameters)
+        # if is_var(distribution, "parameters"):
+        #    distribution = self.parameters[distribution.name]
+        # elif isinstance(distribution, Function) or isinstance(distribution, ModelParameter):
+        #    distribution = get_static_param_value(distribution, parameters)
 
         if isinstance(distribution, dict):
-            for idx, comp in enumerate(self.model._original_compartment_names):
-                pop = distribution.get(comp.name, 0)
+            for idx, comp in enumerate(model._original_compartment_names):
+                pop_key = distribution[comp.name]._graph_key
+                pop = self._graph_values_static[pop_key]
                 assert pop >= 0, f"Population for {comp.name} cannot be negative: {pop}"
                 initial_population[idx] = pop
 
-            comps = self.model._original_compartment_names
+            comps = model._original_compartment_names
 
-            for action in self.model.tracker.all_actions:
+            for action in model.tracker.all_actions:
                 if action.action_type == "stratify":
                     strat = action.kwargs["strat"]
                     # for strat in self.model._stratifications:
                     # Stratify compartments, split according to split_proportions
                     prev_compartment_names = comps  # copy.copy(self.compartments)
                     comps = strat._stratify_compartments(comps)
                     initial_population = strat._stratify_compartment_values(
-                        prev_compartment_names, initial_population, parameters
+                        prev_compartment_names, initial_population, self._graph_values_static
                     )
                 elif action.action_type == "adjust_pop_split":
                     initial_population = get_rebalanced_population(
-                        self.model, initial_population, parameters, **action.kwargs
+                        model, initial_population, self._graph_values_static, **action.kwargs
                     )
-            return initial_population
         else:
             raise TypeError(
-                "Initial population distribution must be a dict or a Function that returns one",
+                "Initial population distribution must be a dict",
                 distribution,
             )
+        model.initial_population = initial_population
```

### Comparing `summerepi-4.1.0a0/summer/runner/vectorized_runner.py` & `summerepi-4.2.0a0/summer/stratification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,443 +1,416 @@
-from typing import Tuple
+"""
+This module presents classes which are used to define stratifications,
+which can be applied to the model.
+"""
+from typing import Callable, Dict, List, Optional, Union
+
+from numbers import Real
 
 import numpy as np
-import numba
+from computegraph.utils import is_var
+from computegraph.types import GraphObject
+
+from summer.adjust import Multiply, Overwrite, enforce_multiply
+from summer.compartment import Compartment
+from summer.parameters import is_func, get_static_param_value
+from summer.parameters.param_impl import get_modelparameter_from_param
 
-import summer.flows as flows
-from summer.compute import (
-    accumulate_positive_flow_contributions,
-    accumulate_negative_flow_contributions,
-    sparse_pairs_accum,
-    find_sum,
-)
+Adjustment = Union[Multiply, Overwrite]
+MixingMatrix = Union[np.ndarray, Callable[[float], np.ndarray]]
 
-from .model_runner import ModelRunner
+# Allowable error in requested compartment splits between one and the total requested
+COMP_SPLIT_REQUEST_ERROR = 1e-2
 
 
-class VectorizedRunner(ModelRunner):
+class Stratification:
     """
-    An optimized, but less accessible model runner.
+    A generic stratification applied to the compartmental model.
+
+    Args:
+        name: The name of the stratification.
+        strata: The new strata that will be created.
+        compartments: The compartments which will be stratified.
+
     """
 
-    def __init__(self, model):
-        super().__init__(model)
+    _is_ageing = False
+    _is_strain = False
 
-    def prepare_structural(self):
-        super().prepare_structural()
+    def __init__(
+        self,
+        name: str,
+        strata: List[str],
+        compartments: List[str],
+    ):
+        self.name = name
+        self.strata = list(map(str, strata))
+        self.compartments = [Compartment(c) if type(c) is str else c for c in compartments]
 
-        self.infectious_flow_indices = np.array(
-            [i for i, f in self._iter_non_function_flows if isinstance(f, flows.BaseInfectionFlow)],
-            dtype=int,
-        )
-        self.death_flow_indices = np.array(
-            [i for i, f in self._iter_non_function_flows if f.is_death_flow], dtype=int
-        )
-
-        # Include dummy values in population_idx to account for Entry flows
-        non_func_pops = np.array(
-            [f.source.idx if f.source else 0 for i, f in self._iter_non_function_flows], dtype=int
-        )
-
-        func_pops = np.array(
-            [f.source.idx if f.source else 0 for i, f in self._iter_function_flows], dtype=int
-        )
+        # Split population evenly by default.
+        num_strata = len(self.strata)
+        self.population_split = {s: 1 / num_strata for s in self.strata}
 
-        self.population_idx = np.concatenate((non_func_pops, func_pops))
+        # Flows are not adjusted by default.
+        self.flow_adjustments = {}
+        self.infectiousness_adjustments = {}
 
-        # Store indices of flows that are not population dependent
-        self._non_pop_flow_idx = np.array(
-            [
-                i
-                for i, f in self._iter_non_function_flows
-                if (type(f) in (flows.ReplacementBirthFlow, flows.ImportFlow))
-            ],
-            dtype=int,
-        )
-        self._has_non_pop_flows = bool(len(self._non_pop_flow_idx))
-
-        # Crude birth flows use population sum rather than a compartment; store indices here
-        self._crude_birth_idx = np.array(
-            [i for i, f in self._iter_non_function_flows if type(f) == flows.CrudeBirthFlow],
-            dtype=int,
-        )
-        self._has_crude_birth = bool(len(self._crude_birth_idx))
-
-        self._has_replacement = False
-        # Replacement flows must be calculated after death flows, store indices here
-        for i, f in self._iter_non_function_flows:
-            if type(f) == flows.ReplacementBirthFlow:
-                self._has_replacement = True
-                self._replacement_flow_idx = i
-
-    def prepare_dynamic(self, parameters: dict = None):
-        """Do all precomputation here"""
-
-        super().prepare_dynamic(parameters)
-
-        self.map_flows_flat()
-        self.precompute_flow_weights()
-        self._precompute_flow_maps()
-
-        self._build_infectious_multipliers_lookup()
-
-        # Initialize arrays for infectious multipliers
-        # FIXME Put this in its own function, this is getting messy again
-        num_cats = self.num_categories
-        num_strains = len(self.model._disease_strains)
-        self._infection_density = {}
-        self._infection_frequency = {}
-        self._infection_density_flat = np.empty((num_strains, num_cats), dtype=float)
-        self._infection_frequency_flat = np.empty((num_strains, num_cats), dtype=float)
-
-    def map_flows_flat(self):
-        """Builds a table of param: index for every unique flow (and flow adjustment) parameter
-
-        Raises:
-            NotImplementedError: Doesn't handle Overwrite adjustments, yet
-        """
-
-        from summer.parameters.param_impl import CompoundParameter
-        from summer.adjust import Overwrite
-
-        param_table = {}
-
-        def update_table(param, idx):
-            if param is None:
-                return
-            if isinstance(param, CompoundParameter):
-                for sp in param.subparams:
-                    update_table(sp, idx)
-            else:
-                if param not in param_table:
-                    param_table[param] = []
-                cur_idx_table = param_table[param]
-                cur_idx_table.append(idx)
-
-        for flow_idx, flow in self._iter_non_function_flows:
-            # Build a list of multiplicative effects for this flow,
-            # discarding previous effects if there is an Overwrite
-            flow_updates = [flow.param]
-            for adj in flow.adjustments:
-                if adj is not None:
-                    if isinstance(adj, Overwrite):
-                        flow_updates = [adj.param]
-                    else:
-                        flow_updates.append(adj.param)
-
-            # Add these to the update table
-            for fparam in flow_updates:
-                update_table(fparam, flow_idx)
-
-            # update_table(flow.param, flow_idx)
-            # for adj in flow.adjustments:
-            #    if isinstance(adj, Overwrite):
-            #        raise NotImplementedError()
-            #    update_table(adj.param, flow_idx)
-
-        self.param_idx_table = {}
-
-        for k, v in param_table.items():
-            self.param_idx_table[k] = np.array(v, dtype=int)
-
-    def precompute_flow_weights(self):
-        self.flow_weights = np.ones(len(self.model._flows), dtype=np.float64)
-        self.timevarying_param_idx = {}
-        for param, idx in self.param_idx_table.items():
-            if not param.is_time_varying():
-                self.flow_weights[idx] *= param.get_value(0.0, {}, self.parameters)
-            else:
-                self.timevarying_param_idx[param] = idx
+        # Store internal fast lookup table for flow adjustments using frozenset
+        self._flow_adjustments_fs = {}
 
-    def _precompute_flow_weights_DEP(self):
-        """Calculate all static flow weights before running,
-        and build indices for time-varying weights"""
-        self.flow_weights = np.zeros(len(self.model._flows))
-        time_varying_weight_indices = []
-        for i, f in self._iter_non_function_flows:
-            weight_type = f.weight_type()
-            if weight_type == flows.WeightType.STATIC:
-                weight = f.get_weight_value(0, None, self.parameters)
-                self.flow_weights[i] = weight
-            elif weight_type == flows.WeightType.FUNCTION:
-                time_varying_weight_indices.append(i)
-
-        self.time_varying_weight_indices = np.array(time_varying_weight_indices, dtype=int)
-
-        self._map_blocks()
-
-    def _map_blocks(self):
-
-        flow_block_maps = {}
-        for i in self.time_varying_weight_indices:
-            f = self.model._flows[i]
-            key = (f.param, tuple(f.adjustments))
-            if key not in flow_block_maps:
-                flow_block_maps[key] = []
-            flow_block_maps[key].append(i)
-
-        self.flow_block_maps = dict(
-            [(k, np.array(v, dtype=int)) for k, v in flow_block_maps.items()]
-        )
-
-    def _precompute_flow_maps(self):
-        """Build fast-access arrays of flow indices"""
-        f_pos_map = []
-        f_neg_map = []
-        for i, f in self._iter_non_function_flows:
-            if f.source:
-                f_neg_map.append((i, f.source.idx))
-            if f.dest:
-                f_pos_map.append((i, f.dest.idx))
-        for i, f in self._iter_function_flows:
-            if f.source:
-                f_neg_map.append((i, f.source.idx))
-            if f.dest:
-                f_pos_map.append((i, f.dest.idx))
-
-        self._pos_flow_map = np.array(f_pos_map, dtype=np.int)
-        self._neg_flow_map = np.array(f_neg_map, dtype=np.int)
-
-    def _prepare_time_step(self, time: float, compartment_values: np.ndarray):
-        """
-        Pre-timestep setup. This should be run before `_get_rates`.
-        Here we set up any stateful updates that need to happen before we get the flow rates.
-        """
-
-        # Some flows (e.g birth replacement) expect this value to be defined
-        self._timestep_deaths = 0.0
+        # No heterogeneous mixing matrix by default.
+        self.mixing_matrix = None
 
-        # Find the effective infectious population for the force of infection (FoI) calculations.
-        mixing_matrix = self._get_mixing_matrix(time)
+        # Enable/disable validation (runtime assertions)
+        # Not directly user accessable - is toggled by CompartmentalModel
+        self._validate = True
 
-        self._calculate_strain_infection_values(compartment_values, mixing_matrix)
+    def __repr__(self):
+        return f"Stratification: {self.name}"
 
-    def _apply_flow_weights_at_time(self, time, computed_values):
-        """Calculate time dependent flow weights and insert them into our weights array
+    def is_ageing(self) -> bool:
+        """Returns ``True`` if this stratification represents a set of age groups
+        with ageing dynamics"""
+        return self._is_ageing
+
+    def is_strain(self) -> bool:
+        """Returns ``True`` if this stratification represents a set of disease strains"""
+        return self._is_strain
+
+    def set_population_split(self, proportions: Dict[str, float]):
+        """
+        Sets how the stratification will split the population between the strata.
 
         Args:
-            time (float): Time in model.times coordinates
+            proportions: A map of proportions to be assigned to each strata.
+
+        The supplied proportions must:
+
+            - Specify all strata
+            - All be positive
+            - Sum to 1 +/- error defined above
+
+        """
+        if all([isinstance(v, Real) for v in proportions.values()]):
+            self.validate_population_split(proportions)
+
+        self.population_split = proportions
+
+    def validate_population_split(self, proportions: dict):
+        msg = f"All strata must be specified when setting population split: {proportions}"
+        assert set(list(proportions.keys())) == set(self.strata), msg
+        msg = f"All proportions must be >= 0 when setting population split: {proportions}"
+        assert all([v >= 0 for v in proportions.values()]), msg
+        msg = f"All proportions sum to 1+/-{COMP_SPLIT_REQUEST_ERROR} when setting \
+            population split: {proportions}"
+        assert abs(1 - sum(proportions.values())) < COMP_SPLIT_REQUEST_ERROR, msg
+
+    def set_flow_adjustments(
+        self,
+        flow_name: str,
+        adjustments: Dict[str, Adjustment],
+        source_strata: Optional[Dict[str, str]] = None,
+        dest_strata: Optional[Dict[str, str]] = None,
+    ):
         """
+        Set an adjustment of a flow to the stratification.
+        Adjustments from previous stratifications will be applied before this.
+        You can use time-varying functions for infectiousness adjustments.
+
+        It is possible to specify multiple flow adjustments for the same flow in a
+        given Stratification.
+        In this case, only the last-created applicable adjustment will be applied.
 
-        # Compute flow value blocks; these are 'chunked' blocks of flows that have a common
-        # flow param/adjustment structure,
-        # but are still specified as operating on individual flows
-        # for (param, adjustments), flow_idx in self.flow_block_maps.items():
-        #     # value = get_model_param_value(param, time, computed_values, self.parameters, True)
-        #     value = param.get_value(time, computed_values, self.parameters)
-        #     for a in adjustments:
-        #         value = a.get_new_value(value, computed_values, time, self.parameters)
-        #     self.flow_weights[flow_idx] = value
-        flow_weights = self.flow_weights.copy()
-
-        for param, idx in self.timevarying_param_idx.items():
-            flow_weights[idx] *= param.get_value(time, computed_values, self.parameters)
-
-        return flow_weights
-
-    def _get_infectious_multipliers(self) -> np.ndarray:
-        """Get multipliers for all infectious flows
-
-        Returns:
-            np.ndarray: Array of infectiousness multipliers
-        """
-        # We can use a fast lookup version if we have only one type of infectious multiplier
-        # (eg only frequency, not mixed freq and density)
-        if self._infection_frequency_only:
-            return self._infection_frequency_flat[
-                self._infect_strain_lookup_idx, self._infect_cat_lookup_idx
-            ]
-        elif self._infection_density_only:
-            return self._infection_density_flat[
-                self._infect_strain_lookup_idx, self._infect_cat_lookup_idx
+        Args:
+            flow_name: The name of the flow to adjust.
+            adjustments: A dict of adjustments to apply to the flow.
+            source_strata (optional): A whitelist of strata to filter the target flow's
+            source compartments.
+            dest_strata (optional): A whitelist of strata to filter the target flow's
+            destination compartments.
+
+        Example:
+            Create an adjustment for the 'recovery' flow based on location::
+
+                strat = Stratification(
+                    name="location",
+                    strata=["urban", "rural", "alpine"],
+                    compartments=["S", "I", "R"]
+                )
+                strat.set_flow_adjustments("recovery", {
+                    "urban": Multiply(1.5),
+                    "rural": Multiply(0.8),
+                    "alpine": None, # No adjustment
+                })
+
+        """
+        source_strata = source_strata or {}
+        dest_strata = dest_strata or {}
+        msg = "You must specify all strata when adding flow adjustments."
+        assert set(adjustments.keys()) == set(self.strata), msg
+
+        adjustments = {k: enforce_multiply(v) for k, v in adjustments.items()}
+
+        msg = "All flow adjustments must be Multiply, Overwrite or None."
+        assert all(
+            [
+                type(adj) is Overwrite or type(adj) is Multiply or adj is None
+                for adj in adjustments.values()
             ]
+        ), msg
 
-        multipliers = np.empty(len(self.infectious_flow_indices))
-        for i, idx in enumerate(self.infectious_flow_indices):
-            f = self.model._flows[idx]
-            multipliers[i] = f.find_infectious_multiplier(f.source, f.dest)
-        return multipliers
-
-    def _build_infectious_multipliers_lookup(self):
-        """Get multipliers for all infectious flows
-
-        These are used by _get_infectious_multipliers_flat (currently experimental)
-
-        Returns:
-            np.ndarray: Array of infectiousness multipliers
-        """
-        lookups = []
-
-        has_freq = False
-        has_dens = False
-
-        for i, idx in enumerate(self.infectious_flow_indices):
-            f = self.model._flows[idx]
-            if isinstance(f, flows.InfectionFrequencyFlow):
-                has_freq = True
-            elif isinstance(f, flows.InfectionDensityFlow):
-                has_dens = True
-            cat_idx, strain = self._get_infection_multiplier_indices(f.source, f.dest)
-            strain_idx = self.model._disease_strains.index(strain)
-            lookups.append([strain_idx, cat_idx])
-        full_table = np.array(lookups, dtype=int)
-        self._full_table = full_table.reshape(len(self.infectious_flow_indices), 2)
-        self._infect_strain_lookup_idx = self._full_table[:, 0].flatten()
-        self._infect_cat_lookup_idx = self._full_table[:, 1].flatten()
-
-        self._infection_frequency_only = False
-        self._infection_density_only = False
-
-        if has_freq and not has_dens:
-            self._infection_frequency_only = True
-        elif has_dens and not has_freq:
-            self._infection_density_only = True
+        msg = "Cannot add new flow adjustments after stratification has already been applied"
+        assert len(self._flow_adjustments_fs) == 0, msg
 
-    def _calculate_strain_infection_values(
-        self, compartment_values: np.ndarray, mixing_matrix: np.ndarray
-    ):
-        num_cats = self.num_categories
-        # Calculate total number of people per category (for FoI).
-        # A vector with size (num_cats).
-        self._category_populations = sparse_pairs_accum(
-            self._compartment_category_map, compartment_values, num_cats
-        )
-
-        for strain_idx, strain in enumerate(self.model._disease_strains):
-            strain_compartment_infectiousness = self._compartment_infectiousness[strain]
-
-            infection_density, infection_frequency = get_strain_infection_values(
-                compartment_values,
-                strain_compartment_infectiousness,
-                self._compartment_category_map,
-                num_cats,
-                mixing_matrix,
-                self._category_populations,
-            )
+        if flow_name not in self.flow_adjustments:
+            self.flow_adjustments[flow_name] = []
+
+        # FIXME Turn this into class or named tuple or something... we want to know what's going on
+        self.flow_adjustments[flow_name].append((adjustments, source_strata, dest_strata))
+
+    def get_flow_adjustment(self, flow) -> dict:
+        """
+        Note that the loop structure implies that if the user has requested multiple adjustments
+        that apply to a single combination of strata (across multiple stratifications), then only
+        the last one that is applicable will be used - because the last request will over-write the
+        earlier ones in the loop.
+        Therefore, the most recently added flow adjustment that matches a given flow will be
+        returned.
+
+        """
+        flow_adjustments = self.flow_adjustments.get(flow.name, [])
+        matching_adjustment = None
+
+        # Cache frozenset lookup
+        if flow.name not in self._flow_adjustments_fs:
+            self._flow_adjustments_fs[flow.name] = cur_fadj_fs = []
+            for adjustment, source_strata, dest_strata in flow_adjustments:
+                cur_fadj_fs.append(
+                    (
+                        adjustment,
+                        source_strata,
+                        frozenset(source_strata.items()),
+                        dest_strata,
+                        frozenset(dest_strata.items()),
+                    )
+                )
+
+        flow_adj_fs = self._flow_adjustments_fs[flow.name]
 
-            self._infection_density[strain] = infection_density
-            self._infection_density_flat[strain_idx] = infection_density
+        # Loop over all the requested adjustments.
+        for adjustment, source_strata, _source_strata, dest_strata, _dest_strata in flow_adj_fs:
 
-            self._infection_frequency[strain] = infection_frequency
-            self._infection_frequency_flat[strain_idx] = infection_frequency
+            # These are expensive assertions and can be disabled in multi-run situations
+            if self._validate:
+                # For entry flows:
+                msg = f"Source strata requested in flow adjustment of {self.name}, but {flow.name} \
+                    does not have a source"
+                assert not (source_strata and not flow.source), msg
+
+                # For exit flows:
+                msg = f"Dest strata requested in flow adjustment of {self.name}, but {flow.name} \
+                    does not have a dest"
+                assert not (dest_strata and not flow.dest), msg
+
+            # Make sure that the source request applies to this flow because it has all of the
+            # requested strata.
+            # Note that these can be specified in the current or any previous stratifications.
+            is_source_no_match = (
+                source_strata and flow.source and not flow.source._has_strata(_source_strata)
+            )
+            if is_source_no_match:
+                continue
+            is_dest_no_match = dest_strata and flow.dest and not flow.dest._has_strata(_dest_strata)
+            if is_dest_no_match:
+                continue
 
-    def _get_flow_rates(self, compartment_vals: np.ndarray, time: float) -> np.ndarray:
-        """Get current flow rates, equivalent to calling get_net_flow on all (non-function) flows
+            matching_adjustment = adjustment
 
-        Args:
-            comp_vals (np.ndarray): Compartment values
-            time (float): Time in model.times coordinates
+        return matching_adjustment
 
-        Returns:
-            np.ndarray: Array of all (non-function) flow rates
+    def add_infectiousness_adjustments(
+        self, compartment_name: str, adjustments: Dict[str, Adjustment]
+    ):
         """
+        Add an adjustment of a compartment's infectiousness to the stratification.
+        You cannot currently use time-varying functions for infectiousness adjustments.
+        All strata in this stratification must be specified as keys in the adjustments argument,
+        if no adjustment required for a stratum, specify None as the value to the request for
+        that stratum.
+
+        Args:
+            compartment_name: The name of the compartment to adjust.
+            adjustments: An dict of adjustments to apply to the compartment.
 
-        computed_values = self._calc_computed_values(compartment_vals, time)
+        Example:
+            Create an adjustment for the 'I' compartment based on location::
 
-        flow_weights = self._apply_flow_weights_at_time(time, computed_values)
-
-        # These will be filled in afterwards
-        populations = compartment_vals[self.population_idx]
-        # Update for special cases (population-independent and CrudeBirth)
-        if self._has_non_pop_flows:
-            populations[self._non_pop_flow_idx] = 1.0
-        if self._has_crude_birth:
-            populations[self._crude_birth_idx] = find_sum(compartment_vals)
-
-        flow_rates = flow_weights * populations
-
-        # Calculate infection flows
-        infect_mul = self._get_infectious_multipliers()
-        flow_rates[self.infectious_flow_indices] *= infect_mul
-
-        # ReplacementBirthFlow depends on death flows already being calculated; update here
-        if self._has_replacement:
-            # Only calculate timestep_deaths if we use replacement, it's expensive...
-            self._timestep_deaths = flow_rates[self.death_flow_indices].sum()
-            flow_rates[self._replacement_flow_idx] = self._timestep_deaths
-
-        self._apply_function_flow_rates(compartment_vals, flow_rates, computed_values, time)
-
-        return flow_rates
-
-    def _apply_function_flow_rates(self, comp_vals, flow_rates, computed_values, time):
-        if self._iter_function_flows:
-            # Evaluate the function flows.
-            for flow_idx, flow in self._iter_function_flows:
-                net_flow = flow.get_net_flow(
-                    self.model.compartments,
-                    comp_vals,
-                    self.model._flows,
-                    flow_rates,
-                    computed_values,
-                    time,
+                strat = Stratification(
+                    name="location",
+                    strata=["urban", "rural", "alpine"],
+                    compartments=["S", "I", "R"]
                 )
-                flow_rates[flow_idx] = net_flow
+                strat.add_infectiousness_adjustments("I", {
+                    "urban": adjust.Multiply(1.5),
+                    "rural": adjust.Multiply(0.8),
+                    "alpine": None, # No adjustment
+                })
+
+        """
+        msg = "You must specify all strata when adding infectiousness adjustments."
+        assert set(adjustments.keys()) == set(self.strata), msg
+
+        adjustments = {k: enforce_multiply(v) for k, v in adjustments.items()}
+
+        # for k, v in adjustments.items():
+        #    if v is not None:
+        #        v.param = get_modelparameter_from_param(v.param)
+
+        msg = "All infectiousness adjustments must be Multiply, Overwrite or None."
+        assert all(
+            [type(a) is Overwrite or type(a) is Multiply or a is None for a in adjustments.values()]
+        ), msg
+
+        msg = f"An infectiousness adjustment for {compartment_name} \
+                already exists for strat {self.name}"
+        assert compartment_name not in self.infectiousness_adjustments, msg
+
+        # FIXME: This should work for computegraph Functions that are not time dependant,
+        # (and fail for those that are), but it's tricky to check...
+        # msg = "Cannot use time varying functions for infectiousness adjustments."
+        # assert not any([adj.param.is_time_varying() for adj in adjustments.values() if adj]), msg
+
+        self.infectiousness_adjustments[compartment_name] = adjustments
+
+    def set_mixing_matrix(self, mixing_matrix: MixingMatrix):
+        """
+        Sets the mixing matrix for the model.
+        Note that this must apply to all compartments, although this is checked at runtime rather
+        than here.
+        """
+        msg = "Strain stratifications cannot have a mixing matrix."
+        assert not self.is_strain(), msg
+
+        # msg = "Mixing matrix must be a NumPy array, or return a NumPy array."
+        # assert (
+        #    (isinstance(mixing_matrix, np.ndarray))
+        #    or isinstance(mixing_matrix, GraphObject)
+        #    or is_func(mixing_matrix)
+        # ), msg
+
+        # if isinstance(mixing_matrix, np.ndarray):
+        #    num_strata = len(self.strata)
+        #    msg = f"Mixing matrix must have both {num_strata} rows and {num_strata} columns."
+        #    assert mixing_matrix.shape == (num_strata, num_strata), msg
+
+        self.mixing_matrix = mixing_matrix
+
+    def _stratify_compartments(self, comps: List[Compartment]) -> List[Compartment]:
+        """
+        Stratify the model compartments into sub-compartments, based on the strata names,
+        Only compartments specified in the stratification's definition will be stratified.
+        Returns the new compartments.
+        """
+        new_comps = []
+        idx = 0
+        for old_comp in comps:
+            should_stratify = old_comp.has_name_in_list(self.compartments)
+            if should_stratify:
+                for stratum in self.strata:
+                    new_comp = old_comp.stratify(self.name, stratum)
+                    new_comp.idx = idx
+                    new_comps.append(new_comp)
+                    idx += 1
+            else:
+                old_comp.idx = idx
+                new_comps.append(old_comp)
+                idx += 1
+
+        return new_comps
+
+    def _stratify_compartment_values(
+        self, comps: List[Compartment], comp_values: np.ndarray, static_graph_values: dict = None
+    ) -> np.ndarray:
+        """
+        Stratify the model compartments into sub-compartments, based on the strata names provided.
+        Split the population according to the provided proportions.
+        Only compartments specified in the stratification's definition will be stratified.
+        Returns the new compartment values.
+        """
+        assert len(comps) == len(comp_values)
+        new_comp_values = []
+
+        if static_graph_values:
+            population_split = get_static_param_value(self.population_split, static_graph_values)
+        else:
+            population_split = self.population_split
+
+        for idx in range(len(comp_values)):
+            should_stratify = comps[idx].has_name_in_list(self.compartments)
+            if should_stratify:
+                for stratum in self.strata:
+                    new_value = comp_values[idx] * population_split[stratum]
+                    new_comp_values.append(new_value)
+            else:
+                new_comp_values.append(comp_values[idx])
 
-    def _get_rates(self, comp_vals: np.ndarray, time: float) -> Tuple[np.ndarray, np.ndarray]:
-        """Calculates inter-compartmental flow rates for a given state and time, as well
-        as the updated compartment values once these rate deltas have been applied
+        return np.array(new_comp_values)
 
-        Args:
-            comp_vals (np.ndarray): The current state of the model compartments
-                                    (ie. number of people)
-            time (float): Time in model.times coordinates
 
-        Returns:
-            Tuple[np.ndarray, np.ndarray]: (comp_rates, flow_rates) where
-                comp_rates is the rate of change of compartments, and
-                flow_rates is the contribution of each flow to compartment rate of change
-        """
-        self._prepare_time_step(time, comp_vals)
+class AgeStratification(Stratification):
+    """
+    A stratification that represents a set of age groups with ageing dynamics.
 
-        comp_rates = np.zeros(len(comp_vals))
-        flow_rates = self._get_flow_rates(comp_vals, time)
+    Args:
+        name: The name of the stratification.
+        strata: The new strata that will be created.
+        compartments: The compartments which will be stratified.
+
+
+    Strata must be a list of strings or integers that represent all ages. For example, the strata
+    [0, 10, 20, 30] will be interpreted as the age groups 0-9, 10-19, 20-29, 30+ respectively.
+
+    Using this stratification will automatically add a set of ageing flows to the model,
+    where the exit rate is proportional to the age group's time span. For example, in the 0-9
+    strata, there will be a flow created where 10% of occupants "age up" into the 10-19 strata
+    each year.
+    **Critically**, this feature assumes that each of the model's time steps represents a year.
 
-        if self._pos_flow_map.size > 0:
-            accumulate_positive_flow_contributions(flow_rates, comp_rates, self._pos_flow_map)
+    """
 
-        if self._neg_flow_map.size > 0:
-            accumulate_negative_flow_contributions(flow_rates, comp_rates, self._neg_flow_map)
+    _is_ageing = True
 
-        return comp_rates, flow_rates
+    def __init__(
+        self,
+        name: str,
+        strata: List[str],
+        compartments: List[str],
+    ):
+        try:
+            _strata = sorted(map(int, strata))
+        except Exception:
+            raise AssertionError("Strata must be in an int-compatible format")
 
-    def get_compartment_rates(self, compartment_values: np.ndarray, time: float):
-        """
-        Interface for the ODE solver: this function is passed to solve_ode func and defines the
-        dynamics of the model.
-        Returns the rate of change of the compartment values for a given state and time.
-        """
-        comp_vals = self._clean_compartment_values(compartment_values)
-        comp_rates, _ = self._get_rates(comp_vals, time)
-        return comp_rates
+        assert _strata[0] == 0, "First age strata must be 0"
 
-    def get_flow_rates(self, compartment_values: np.ndarray, time: float):
-        """
-        Returns the contribution of each flow to compartment rate of change for a given state and
-        time.
-        """
-        comp_vals = self._clean_compartment_values(compartment_values)
-        _, flow_rates = self._get_rates(comp_vals, time)
-        return flow_rates
+        _strata = map(str, _strata)
+        super().__init__(name, _strata, compartments)
 
 
-"""
-Additional functions - fast JIT specializations etc
-"""
+class StrainStratification(Stratification):
+    """
+    A stratification that represents a set of disease strains.
+
+    Args:
+        name: The name of the stratification.
+        strata: The new strata that will be created.
+        compartments: The compartments which will be stratified.
 
 
-@numba.jit
-def get_strain_infection_values(
-    compartment_values,
-    strain_compartment_infectiousness,
-    compartment_category_map,
-    num_cats,
-    mixing_matrix,
-    category_populations,
-):
-    infected_values = compartment_values * strain_compartment_infectiousness
-    infectious_populations = sparse_pairs_accum(compartment_category_map, infected_values, num_cats)
-    infection_density = mixing_matrix @ infectious_populations
-    category_prevalence = infectious_populations / category_populations
-    infection_frequency = mixing_matrix @ category_prevalence
+    Each requested stratum will be interpreted as a different strain of the disease being modelled.
+    This will mean that the force of infection calculations will consider each strain separately.
+
+    Strain stratifications cannot use a mixing matrix
+
+    """
 
-    return infection_density, infection_frequency
+    _is_strain = True
```

### Comparing `summerepi-4.1.0a0/summer/solver.py` & `summerepi-4.2.0a0/summer/solver.py`

 * *Files identical despite different names*

### Comparing `summerepi-4.1.0a0/summer/stochastic.py` & `summerepi-4.2.0a0/summer/stochastic.py`

 * *Files identical despite different names*

### Comparing `summerepi-4.1.0a0/setup.py` & `summerepi-4.2.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['summer',
+ 'summer.compute',
  'summer.experimental',
  'summer.parameters',
  'summer.runner',
  'summer.runner.jax']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['computegraph>=0.2.2',
+['computegraph>=0.3.0b',
  'networkx>=2.6.2',
  'numba>=0.54.0',
  'numpy>=1.20.3',
  'pandas>=1.3.2',
  'scipy>=1.7.1']
 
 extras_require = \
 {':sys_platform == "darwin"': ['jax[cpu]>=0.3.14,<0.4.0'],
  ':sys_platform == "linux"': ['jax[cpu]>=0.3.14,<0.4.0']}
 
 setup_kwargs = {
     'name': 'summerepi',
-    'version': '4.1.0a0',
+    'version': '4.2.0a0',
     'description': 'Summer is a compartmental disease modelling framework, written in Python. It provides a high-level API to build and run models.',
-    'long_description': '# Summer: compartmental disease modelling in Python\n\n[![Automated Tests](https://github.com/monash-emu/summer/actions/workflows/tests.yml/badge.svg)](https://github.com/monash-emu/summer/actions/workflows/tests.yml)\n\nSummer is a Python-based framework for the creation and execution of [compartmental](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology) (or "state-based") epidemiological models of infectious disease transmission.\n\nIt provides a range of structures for easily implementing compartmental models, including structure for some of the most common features added to basic compartmental frameworks, including:\n\n- A variety of inter-compartmental flows (infections, transitions, births, deaths, imports)\n- Force of infection multipliers (frequency, density)\n- Post-processing of compartment sizes into derived outputs\n- Stratification of compartments, including:\n  - Adjustments to flow rates based on strata\n  - Adjustments to infectiousness based on strata\n  - Heterogeneous mixing between strata\n  - Multiple disease strains\n\nSome helpful links to learn more:\n\n- [Rationale](http://summerepi.com/rationale.html) for why we are building Summer\n- **[Documentation](http://summerepi.com/)** with [code examples](http://summerepi.com/examples)\n- [Available on PyPi](https://pypi.org/project/summerepi/) as `summerepi`.\n- [Performance benchmarks](https://monash-emu.github.io/summer/)\n\n## Installation and Quickstart\n\nThis project requires at least Python 3.7 (and is actively targeted at 3.9)\nInstall the `summerepi` package from PyPI\n\n```bash\npip install summerepi\n```\n\nThen you can use the library to build and run models. See [here](http://summerepi.com/examples) for some code examples.\n\n## Development\n\n[Poetry](https://python-poetry.org/) is used for packaging and dependency management.\n\nInitial project setup is documented [here](./docs/dev-setup.md) and should work for Windows or Ubuntu, maybe for MacOS.\n\nSome common things to do as a developer working on this codebase:\n\n```bash\n# Activate summer conda environment prior to doing other stuff (see setup docs)\nconda activate summer\n\n# Install latest requirements\npoetry install\n\n# Publish to PyPI - use your PyPI credentials\npoetry publish --build\n\n# Add a new package\npoetry add\n\n# Run tests\npytest -vv\n\n# Format Python code\nblack .\nisort . --profile black\n```\n\n## Releases\n\nReleases are numbered using [Semantic Versioning](https://semver.org/)\n\n- 1.0.0/1:\n  - Initial release\n- 1.1.0:\n  - Add stochastic integrator\n- 2.0.2:\n  - Rename fractional flow to transition flow\n  - Remove sojourn flow\n  - Add vectorized backend and other performance improvements\n- 2.0.3:\n  - Set default IVP solver to use a maximum step size of 1 timestep\n- 2.0.4:\n  - Add runtime derived values\n- 2.0.5:\n  - Remove legacy Summer implementation\n- 2.1.0:\n  - Add AdjustmentSystems\n  - Improve vectorization of flows\n  - Add computed_values inputs to flow and adjustment parameters\n- 2.1.1:\n  - Fix for invalid/unused package imports (cachetools)\n- 2.2.0\n  - Add validation and compartment caching optimizations\n- 2.2.1\n  - Derived output index caching\n  - Optimized fast-tracks for infectious multipliers\n- 2.2.2\n  - JIT infectiousness calculations\n  - Various micro-optimizations\n- 2.2.3\n  - Bugfix release (clamp outputs to 0.0)\n- 2.2.4\n  - Datetime awareness, DataFrame outputs\n- 2.2.5\n  - Performance improvements (frozenset), no API changes\n- 2.2.6\n  - Verify strata in flow adjustments (prevent unexpected behaviour)\n- 2.2.7\n  - Rename add_flow_adjustments -> set_flow_adjustments\n- 2.2.8\n  - Split imports functionality (add_importation_flow now requires split_imports arg)\n- 2.2.9\n  - Post-stratification population restribution\n- 2.3.0\n  - First official version to support only Python 3.7\n- 2.5.0\n  - Support Python 3.9\n- 2.6.0\n  - Merge 3.9/master branches\n- 2.7.0\n  - Include Python 3.10 support and update requirements\n- 2.7.1\n  - Bugfix (source flows not counted correctly in _add_transition_flow)\n- 3.1.0\n  - Parameter aware summer using computegraph\n- 3.1.1\n  - Update computegraph and add additional param awareness\n- 3.1.2\n  - Initial population/stratification now param aware\n- 3.1.3\n  - More jax implementation (strain stratification)\n- 3.1.4\n  - Bugfix release (jax imported even though optional)\n- 3.1.5\n  - Bugfix and minor improvements search for parameters\n- 3.1.6\n  - Support lists of adjustments and flow params\n- 4.0.0a\n  - Full jax support with ModelBuilder wrapper\n- 4.1.0a\n  - Abstract and lazy parameters\n\n## Release process\n\nTo do a release:\n\n- Commit any code changes and push them to GitHub\n- Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)\n- Add a release note above\n- Edit the `version` key in `pyproject.toml` to reflect the release number\n- Publish the package to [PyPI](https://pypi.org/project/summerepi/) using Poetry, you will need a PyPI login and access to the project\n- Commit the release changes and push them to GitHub (Use a commit message like "Release 1.1.0")\n- Update `requirements.txt` in Autumn to use the new version of Summer\n\n```bash\npoetry build\npoetry publish\n```\n\n## Documentation\n\nSphinx is used to automatically build reference documentation for this library.\nThe documentation is automatically built and deployed to [summerepi.com](http://summerepi.com/) whenever code is pushed to `master`.\n\nTo run or edit the code examples in the documentation, start a jupyter notebook server as follows:\n\n```bash\njupyter notebook --config docs/jupyter_notebook_config.py\n# Go to http://localhost:8888/tree/docs/examples in your web browser.\n```\n\nYou can clean outputs from all the example notbooks with\n\n```bash\n./docs/scripts/clean.sh\n```\n\nTo build and deploy\n\n```bash\n./docs/scripts/build.sh\n./docs/scripts/deploy.sh\n```\n\nTo work on docs locally\n\n```bash\n./docs/scripts/watch.sh\n```\n',
+    'long_description': '# Summer: compartmental disease modelling in Python\n\n[![Automated Tests](https://github.com/monash-emu/summer/actions/workflows/tests.yml/badge.svg)](https://github.com/monash-emu/summer/actions/workflows/tests.yml)\n\nSummer is a Python-based framework for the creation and execution of [compartmental](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology) (or "state-based") epidemiological models of infectious disease transmission.\n\nIt provides a range of structures for easily implementing compartmental models, including structure for some of the most common features added to basic compartmental frameworks, including:\n\n- A variety of inter-compartmental flows (infections, transitions, births, deaths, imports)\n- Force of infection multipliers (frequency, density)\n- Post-processing of compartment sizes into derived outputs\n- Stratification of compartments, including:\n  - Adjustments to flow rates based on strata\n  - Adjustments to infectiousness based on strata\n  - Heterogeneous mixing between strata\n  - Multiple disease strains\n\nSome helpful links to learn more:\n\n- [Rationale](http://summerepi.com/rationale.html) for why we are building Summer\n- **[Documentation](http://summerepi.com/)** with [code examples](http://summerepi.com/examples)\n- [Available on PyPi](https://pypi.org/project/summerepi/) as `summerepi`.\n- [Performance benchmarks](https://monash-emu.github.io/summer/)\n\n## Installation and Quickstart\n\nThis project requires at least Python 3.7 (and is actively targeted at 3.9)\nInstall the `summerepi` package from PyPI\n\n```bash\npip install summerepi\n```\n\nThen you can use the library to build and run models. See [here](http://summerepi.com/examples) for some code examples.\n\n## Development\n\n[Poetry](https://python-poetry.org/) is used for packaging and dependency management.\n\nInitial project setup is documented [here](./docs/dev-setup.md) and should work for Windows or Ubuntu, maybe for MacOS.\n\nSome common things to do as a developer working on this codebase:\n\n```bash\n# Activate summer conda environment prior to doing other stuff (see setup docs)\nconda activate summer\n\n# Install latest requirements\npoetry install\n\n# Publish to PyPI - use your PyPI credentials\npoetry publish --build\n\n# Add a new package\npoetry add\n\n# Run tests\npytest -vv\n\n# Format Python code\nblack .\nisort . --profile black\n```\n\n## Releases\n\nReleases are numbered using [Semantic Versioning](https://semver.org/)\n\n- 1.0.0/1:\n  - Initial release\n- 1.1.0:\n  - Add stochastic integrator\n- 2.0.2:\n  - Rename fractional flow to transition flow\n  - Remove sojourn flow\n  - Add vectorized backend and other performance improvements\n- 2.0.3:\n  - Set default IVP solver to use a maximum step size of 1 timestep\n- 2.0.4:\n  - Add runtime derived values\n- 2.0.5:\n  - Remove legacy Summer implementation\n- 2.1.0:\n  - Add AdjustmentSystems\n  - Improve vectorization of flows\n  - Add computed_values inputs to flow and adjustment parameters\n- 2.1.1:\n  - Fix for invalid/unused package imports (cachetools)\n- 2.2.0\n  - Add validation and compartment caching optimizations\n- 2.2.1\n  - Derived output index caching\n  - Optimized fast-tracks for infectious multipliers\n- 2.2.2\n  - JIT infectiousness calculations\n  - Various micro-optimizations\n- 2.2.3\n  - Bugfix release (clamp outputs to 0.0)\n- 2.2.4\n  - Datetime awareness, DataFrame outputs\n- 2.2.5\n  - Performance improvements (frozenset), no API changes\n- 2.2.6\n  - Verify strata in flow adjustments (prevent unexpected behaviour)\n- 2.2.7\n  - Rename add_flow_adjustments -> set_flow_adjustments\n- 2.2.8\n  - Split imports functionality (add_importation_flow now requires split_imports arg)\n- 2.2.9\n  - Post-stratification population restribution\n- 2.3.0\n  - First official version to support only Python 3.7\n- 2.5.0\n  - Support Python 3.9\n- 2.6.0\n  - Merge 3.9/master branches\n- 2.7.0\n  - Include Python 3.10 support and update requirements\n- 2.7.1\n  - Bugfix (source flows not counted correctly in _add_transition_flow)\n- 3.1.0\n  - Parameter aware summer using computegraph\n- 3.1.1\n  - Update computegraph and add additional param awareness\n- 3.1.2\n  - Initial population/stratification now param aware\n- 3.1.3\n  - More jax implementation (strain stratification)\n- 3.1.4\n  - Bugfix release (jax imported even though optional)\n- 3.1.5\n  - Bugfix and minor improvements search for parameters\n- 3.1.6\n  - Support lists of adjustments and flow params\n- 4.0.0a\n  - Full jax support with ModelBuilder wrapper\n- 4.1.0a\n  - Abstract and lazy parameters\n- 4.2.0a\n  - Refactor parameters, combine runners\n\n## Release process\n\nTo do a release:\n\n- Commit any code changes and push them to GitHub\n- Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)\n- Add a release note above\n- Edit the `version` key in `pyproject.toml` to reflect the release number\n- Publish the package to [PyPI](https://pypi.org/project/summerepi/) using Poetry, you will need a PyPI login and access to the project\n- Commit the release changes and push them to GitHub (Use a commit message like "Release 1.1.0")\n- Update `requirements.txt` in Autumn to use the new version of Summer\n\n```bash\npoetry build\npoetry publish\n```\n\n## Documentation\n\nSphinx is used to automatically build reference documentation for this library.\nThe documentation is automatically built and deployed to [summerepi.com](http://summerepi.com/) whenever code is pushed to `master`.\n\nTo run or edit the code examples in the documentation, start a jupyter notebook server as follows:\n\n```bash\njupyter notebook --config docs/jupyter_notebook_config.py\n# Go to http://localhost:8888/tree/docs/examples in your web browser.\n```\n\nYou can clean outputs from all the example notbooks with\n\n```bash\n./docs/scripts/clean.sh\n```\n\nTo build and deploy\n\n```bash\n./docs/scripts/build.sh\n./docs/scripts/deploy.sh\n```\n\nTo work on docs locally\n\n```bash\n./docs/scripts/watch.sh\n```\n',
     'author': 'James Trauer',
     'author_email': 'james.trauer@monash.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'http://summerepi.com/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `summerepi-4.1.0a0/PKG-INFO` & `summerepi-4.2.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: summerepi
-Version: 4.1.0a0
+Version: 4.2.0a0
 Summary: Summer is a compartmental disease modelling framework, written in Python. It provides a high-level API to build and run models.
 Home-page: http://summerepi.com/
 License: BSD-2-Clause
 Keywords: epidemiology,disease,compartmental,infectious
 Author: James Trauer
 Author-email: james.trauer@monash.edu
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: computegraph (>=0.2.2)
+Requires-Dist: computegraph (>=0.3.0b)
 Requires-Dist: jax[cpu] (>=0.3.14,<0.4.0); sys_platform == "darwin"
 Requires-Dist: jax[cpu] (>=0.3.14,<0.4.0); sys_platform == "linux"
 Requires-Dist: networkx (>=2.6.2)
 Requires-Dist: numba (>=0.54.0)
 Requires-Dist: numpy (>=1.20.3)
 Requires-Dist: pandas (>=1.3.2)
 Requires-Dist: scipy (>=1.7.1)
@@ -159,14 +159,16 @@
   - Bugfix and minor improvements search for parameters
 - 3.1.6
   - Support lists of adjustments and flow params
 - 4.0.0a
   - Full jax support with ModelBuilder wrapper
 - 4.1.0a
   - Abstract and lazy parameters
+- 4.2.0a
+  - Refactor parameters, combine runners
 
 ## Release process
 
 To do a release:
 
 - Commit any code changes and push them to GitHub
 - Choose a new release number accoridng to [Semantic Versioning](https://semver.org/)
```

