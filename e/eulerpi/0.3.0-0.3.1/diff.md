# Comparing `tmp/eulerpi-0.3.0.tar.gz` & `tmp/eulerpi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.3.0.tar", max compression
+gzip compressed data, was "eulerpi-0.3.1.tar", max compression
```

## Comparing `eulerpi-0.3.0.tar` & `eulerpi-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1117 2023-05-01 17:45:45.703946 eulerpi-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     4704 2023-05-01 17:45:45.707946 eulerpi-0.3.0/README.md
--rw-r--r--   0        0        0      564 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/__init__.py
--rw-r--r--   0        0        0      191 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/__init__.py
--rw-r--r--   0        0        0     7531 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/data_transformation.py
--rw-r--r--   0        0        0      362 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/data_transformation_types.py
--rw-r--r--   0        0        0    11433 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0      355 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/dense_grid_types.py
--rw-r--r--   0        0        0     6790 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/inference.py
--rw-r--r--   0        0        0      514 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/inference_types.py
--rw-r--r--   0        0        0     3684 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/kde.py
--rw-r--r--   0        0        0    15896 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/model.py
--rw-r--r--   0        0        0    17922 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    15769 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    21145 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0     7006 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/core/transformations.py
--rw-r--r--   0        0        0    14800 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0     1811 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0     1133 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1859 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2023-05-01 17:45:45.711946 eulerpi-0.3.0/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0   189602 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/ETF.csv
--rw-r--r--   0        0        0      268 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/ETF50.csv
--rw-r--r--   0        0        0       88 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/__init__.py
--rw-r--r--   0        0        0     5556 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/stock/stock.py
--rw-r--r--   0        0        0     5877 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     2136 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2023-05-01 17:45:45.715946 eulerpi-0.3.0/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2340 2023-05-01 17:45:45.715946 eulerpi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6173 1970-01-01 00:00:00.000000 eulerpi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-03 13:37:52.817343 eulerpi-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     4704 2023-05-03 13:37:52.817343 eulerpi-0.3.1/README.md
+-rw-r--r--   0        0        0      564 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0     7531 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/data_transformation.py
+-rw-r--r--   0        0        0      362 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/data_transformation_types.py
+-rw-r--r--   0        0        0    11433 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      355 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0     6790 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      514 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     3684 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    15896 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/model.py
+-rw-r--r--   0        0        0    18493 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    15655 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    21145 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0     7006 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0    14800 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1295 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0     1811 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0     1133 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1859 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0   189602 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/stock/ETF.csv
+-rw-r--r--   0        0        0      268 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/stock/ETF50.csv
+-rw-r--r--   0        0        0       88 2023-05-03 13:37:52.825343 eulerpi-0.3.1/eulerpi/examples/stock/__init__.py
+-rw-r--r--   0        0        0     5556 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/stock/stock.py
+-rw-r--r--   0        0        0     5877 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     2136 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2023-05-03 13:37:52.829343 eulerpi-0.3.1/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2340 2023-05-03 13:37:52.829343 eulerpi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6173 1970-01-01 00:00:00.000000 eulerpi-0.3.1/PKG-INFO
```

### Comparing `eulerpi-0.3.0/LICENSE.md` & `eulerpi-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/README.md` & `eulerpi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/__init__.py` & `eulerpi-0.3.1/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/data_transformation.py` & `eulerpi-0.3.1/eulerpi/core/data_transformation.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/dense_grid.py` & `eulerpi-0.3.1/eulerpi/core/dense_grid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/inference.py` & `eulerpi-0.3.1/eulerpi/core/inference.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/inference_types.py` & `eulerpi-0.3.1/eulerpi/core/inference_types.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/kde.py` & `eulerpi-0.3.1/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/model.py` & `eulerpi-0.3.1/eulerpi/core/model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/result_manager.py` & `eulerpi-0.3.1/eulerpi/core/result_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,17 +216,15 @@
             sampler_results[:, -1],
             delimiter=",",
         )
 
         # Save the simulation results
         np.savetxt(
             results_path + "/SimResults/sim_results_" + str(run) + ".csv",
-            sampler_results[
-                :, sampling_dim : model.param_dim + model.data_dim
-            ],
+            sampler_results[:, sampling_dim : sampling_dim + model.data_dim],
             delimiter=",",
         )
 
         # Save the final walker positions
         np.savetxt(
             results_path + "/final_walker_positions_" + str(run) + ".csv",
             final_walker_positions,
@@ -407,14 +405,17 @@
         # use default values saved in inference_information if not specified
         if num_burn_in_samples is None:
             num_burn_in_samples = inference_information["num_burn_in_samples"]
 
         if thinning_factor is None:
             thinning_factor = inference_information["thinning_factor"]
 
+        num_steps = inference_information["num_steps"]
+        num_walkers = inference_information["num_walkers"]
+
         # load samples from raw chains
         for i in range(inference_information["num_runs"]):
             density_evals = np.loadtxt(
                 results_path + f"/DensityEvals/density_evals_{i}.csv",
                 delimiter=",",
             )
             sim_results = np.loadtxt(
@@ -424,41 +425,50 @@
             )
             params = np.loadtxt(
                 results_path + f"/Params/params_{i}.csv",
                 delimiter=",",
                 ndmin=2,
             )
             if i == 0:
-                overall_density_evals = density_evals
-                overall_sim_results = sim_results
-                overall_params = params
+                param_dim = params.shape[1]
+                data_dim = sim_results.shape[1]
+                overall_density_evals = density_evals.reshape(
+                    num_steps, num_walkers, 1
+                )
+                overall_sim_results = sim_results.reshape(
+                    num_steps, num_walkers, data_dim
+                )
+                overall_params = params.reshape(
+                    num_steps, num_walkers, param_dim
+                )
             else:
                 overall_density_evals = np.concatenate(
-                    (overall_density_evals, density_evals)
+                    (
+                        overall_density_evals,
+                        density_evals.reshape(num_steps, num_walkers, 1),
+                    )
                 )
                 overall_sim_results = np.concatenate(
-                    (overall_sim_results, sim_results)
+                    (
+                        overall_sim_results,
+                        sim_results.reshape(num_steps, num_walkers, data_dim),
+                    )
+                )
+                overall_params = np.concatenate(
+                    (
+                        overall_params,
+                        params.reshape(num_steps, num_walkers, param_dim),
+                    )
                 )
-                overall_params = np.concatenate((overall_params, params))
-
-        num_walkers = inference_information["num_walkers"]
 
         # thin and burn in
         return (
-            overall_params[
-                num_burn_in_samples
-                * num_walkers :: thinning_factor
-                * num_walkers,
-                :,
-            ],
+            overall_params[num_burn_in_samples::thinning_factor, :, :].reshape(
+                -1, param_dim
+            ),
             overall_sim_results[
-                num_burn_in_samples
-                * num_walkers :: thinning_factor
-                * num_walkers,
-                :,
-            ],
+                num_burn_in_samples::thinning_factor, :, :
+            ].reshape(-1, data_dim),
             overall_density_evals[
-                num_burn_in_samples
-                * num_walkers :: thinning_factor
-                * num_walkers
-            ],
+                num_burn_in_samples::thinning_factor, :, :
+            ].reshape(-1, 1),
         )
```

### Comparing `eulerpi-0.3.0/eulerpi/core/sampling.py` & `eulerpi-0.3.1/eulerpi/core/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,14 @@
     # TODO: Keep as 3d array?
     # Should have shape (num_steps, num_walkers, param_dim+data_dim+1)
     sampler_results = sampler.get_blobs()
     data_dim = model.data_dim
     sampler_results = sampler_results.reshape(
         num_steps * num_walkers, sampling_dim + data_dim + 1
     )
-    sampler_results = sampler_results.reshape(
-        num_walkers * num_steps, sampling_dim + data_dim + 1
-    )
 
     logger.info(
         f"The acceptance fractions of the emcee sampler per walker are: {np.round(sampler.acceptance_fraction, 2)}"
     )
     try:
         corrTimes = sampler.get_autocorr_time()
         logger.info(f"autocorrelation time: {corrTimes[0]}")
```

### Comparing `eulerpi-0.3.0/eulerpi/core/sparsegrid.py` & `eulerpi-0.3.1/eulerpi/core/sparsegrid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/core/transformations.py` & `eulerpi-0.3.1/eulerpi/core/transformations.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.3.1/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/corona/corona.py` & `eulerpi-0.3.1/eulerpi/examples/corona/corona.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.3.1/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.3.1/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.3.1/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.3.1/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.3.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.3.1/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.py` & `eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.3.1/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/simple_models.py` & `eulerpi-0.3.1/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/stock/ETF.csv` & `eulerpi-0.3.1/eulerpi/examples/stock/ETF.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/stock/stock.py` & `eulerpi-0.3.1/eulerpi/examples/stock/stock.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.3.1/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.3.1/eulerpi/examples/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/eulerpi/jax_extension.py` & `eulerpi-0.3.1/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.3.0/pyproject.toml` & `eulerpi-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.3.0"
+version = "0.3.1"
 description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `eulerpi-0.3.0/PKG-INFO` & `eulerpi-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.3.0
+Version: 0.3.1
 Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

