# Comparing `tmp/openstef_dbc-3.6.3a0.tar.gz` & `tmp/openstef_dbc-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.3a0.tar", last modified: Wed Apr 19 13:44:50 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.4.tar", last modified: Wed May  3 11:44:29 2023, max compression
```

## Comparing `openstef_dbc-3.6.3a0.tar` & `openstef_dbc-3.6.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.286216 openstef_dbc-3.6.3a0/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.286216 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 13:44:50.000000 openstef_dbc-3.6.3a0/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 13:44:50.290216 openstef_dbc-3.6.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-19 13:44:38.000000 openstef_dbc-3.6.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:29.789217 openstef_dbc-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-03 11:44:29.789217 openstef_dbc-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:29.785216 openstef_dbc-3.6.4/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:29.785216 openstef_dbc-3.6.4/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:29.785216 openstef_dbc-3.6.4/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:29.785216 openstef_dbc-3.6.4/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:44:29.785216 openstef_dbc-3.6.4/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-03 11:44:29.000000 openstef_dbc-3.6.4/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-03 11:44:29.000000 openstef_dbc-3.6.4/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:44:29.000000 openstef_dbc-3.6.4/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-03 11:44:29.000000 openstef_dbc-3.6.4/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 11:44:29.000000 openstef_dbc-3.6.4/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 11:44:29.789217 openstef_dbc-3.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-03 11:44:15.000000 openstef_dbc-3.6.4/setup.py
```

### Comparing `openstef_dbc-3.6.3a0/LICENSE` & `openstef_dbc-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/PKG-INFO` & `openstef_dbc-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.3a0
+Version: 3.6.4
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.3a0/README.md` & `openstef_dbc-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/__init__.py` & `openstef_dbc-3.6.4/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.4/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/database.py` & `openstef_dbc-3.6.4/openstef_dbc/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,30 +33,32 @@
     _splitting = Splitting()
     _predictions = Predictions()
     _model_input = ModelInput()
     _systems = Systems()
 
     # write methods
     write_weather_data = _write.write_weather_data
-    write_realised_power_measurements = _write.write_realised_power_measurements
+    write_realised = _write.write_realised
     write_realised_pvdata = _write.write_realised_pvdata
     write_kpi = _write.write_kpi
     write_forecast = _write.write_forecast
     write_apx_market_data = _write.write_apx_market_data
     write_sjv_load_profiles = _write.write_sjv_load_profiles
     write_windturbine_powercurves = _write.write_windturbine_powercurves
     write_energy_splitting_coefficients = _write.write_energy_splitting_coefficients
 
     # prediction job methods
     get_prediction_jobs_solar = _prediction_job.get_prediction_jobs_solar
     get_prediction_jobs_wind = _prediction_job.get_prediction_jobs_wind
     get_prediction_jobs = _prediction_job.get_prediction_jobs
     get_prediction_job = _prediction_job.get_prediction_job
     get_pids_for_api_key = _prediction_job.get_pids_for_api_key
+    get_pids_for_api_keys = _prediction_job.get_pids_for_api_keys
     get_ean_for_pid = _prediction_job.get_ean_for_pid
+    get_eans_for_pids = _prediction_job.get_eans_for_pids
 
     # weather methods
     get_weather_forecast_locations = _weather.get_weather_forecast_locations
     get_weather_data = _weather.get_weather_data
     get_datetime_last_stored_knmi_weatherdata = (
         _weather.get_datetime_last_stored_knmi_weatherdata
     )
@@ -88,14 +90,15 @@
     get_systems_near_location = _systems.get_systems_near_location
     get_systems_by_pid = _systems.get_systems_by_pid
     get_pv_systems_with_incorrect_location = (
         _systems.get_pv_systems_with_incorrect_location
     )
     get_random_pv_systems = _systems.get_random_pv_systems
     get_api_key_for_system = _systems.get_api_key_for_system
+    get_api_keys_for_systems = _systems.get_api_keys_for_systems
 
     def __init__(self, config):
         """Construct the DataBase singleton.
 
         Initialize the datainterface and api. WARNING: this is a singleton class when
         calling multiple times with a config argument no new configuration will be
         applied.
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.4/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.4/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.4/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.4/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.4/openstef_dbc/services/ems.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,18 +116,19 @@
                     |> pivot(rowKey:["_time"], columnKey: ["system"], valueColumn: "_value")
             """
 
         # Query load
         result_raw = _DataInterface.get_instance().exec_influx_query(query, bind_params)
 
         if isinstance(result_raw, pd.DataFrame) and result_raw.empty:
-            raise RuntimeError(
+            self.logger.warning(
                 f"Probably no load data avalailable for the following system(s): \n {sid} \n"
                 f"The following query yields an empty dataframe: {query}"
             )
+            return pd.DataFrame()
 
         if aggregated:
             result = pd.concat(
                 [
                     result_raw[0][["_time", "_value"]].rename(
                         columns={"_value": "load"}
                     ),
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.4/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.4/openstef_dbc/services/prediction_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,16 +216,44 @@
         """
         result = _DataInterface.get_instance().exec_sql_query(query, bind_params)
         if isinstance(result, pd.DataFrame) and result.empty:
             return []
         else:
             return result["id"].to_list()
 
-    def get_ean_for_pid(self, pid: int) -> str:
-        """Get EAN that is connectec to a prediction
+    def get_pids_for_api_keys(self, api_keys: list[str]) -> list[int]:
+        """Get all pids that belong to a given list of API keys.
+
+        Args:
+            api_key (str): The list with API keys
+
+        Returns:
+            list[int]: List of pids
+        """
+        pids = []
+        for api_key in api_keys:
+            pids.append(self.get_pids_for_api_key(api_key))
+        return list(set(pids))
+
+    def get_eans_for_pids(self, pids: list[int]) -> dict[int : list[str]]:
+        """Get EANs that are connected to a prediction.
+
+        Args:
+            pid (int): The prediction ID
+
+        Returns:
+            dict{int:list[str]}: The pid to eans mapping
+        """
+        eans = {}
+        for pid in pids:
+            eans.update({pid: eans.append(self.get_ean_for_pid(pid))})
+        return eans
+
+    def get_ean_for_pid(self, pid: int) -> list[str]:
+        """Get EAN that is connected to a prediction
 
         Args:
             pid (int): The prediction ID
 
         Returns:
             str: The corresponding EAN code
         """
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.4/openstef_dbc/services/predictions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 
 import pandas as pd
 import re
 
 from openstef_dbc.data_interface import _DataInterface
 from openstef_dbc.utils import parse_influx_result
 
+FIELDS_OF_INTEREST = [
+    "forecast",
+    "stdev",
+    "forecast_other",
+    "forecast_solar",
+    "forecast_wind_on_shore",
+]
+
 
 class Predictions:
     def get_predicted_load(
         self,
         pj: dict,
         start_time: datetime = None,
         end_time: datetime = None,
@@ -69,15 +77,15 @@
             # Shifting is needed to output the same as with the old influx client
             return parse_influx_result(result).shift(-15, freq="T")
         else:
             return pd.Series()
 
     def get_forecast_quality(
         self, pj: dict, start_time: datetime = None, end_time: datetime = None
-    ):
+    ) -> pd.Series:
         """Get forecast quality for historic load predictions for given pid.
 
         Args:
             pj (dict): Prediction job
             start_time (datetime): Start time to retrieve the historic load prediction.
             end_time (datetime): End time to retrieve the historic load prediction.
 
@@ -129,15 +137,15 @@
     ):
         """Get historic load predictions for given pid including component forecasts.
 
         Args:
             pj (dict): Prediction job
             start_time (datetime): Start time  to retrieve the historic load prediction.
             end_time (datetime): End timeto retrieve the historic load prediction.
-            quantiles: (boo): Indicates wheter quantiles should be retrieved as well.
+            quantiles: (bool): Indicates wheter quantiles should be retrieved as well.
 
         Returns:
             pandas.DataFrame: Dataframe with the total forecast,
             the components forecasts and the quantiles if they are requested.
 
         """
         # Apply default parameters if none are provided
@@ -154,35 +162,38 @@
         quantile_section = (
             """or r._field == "quantile_P"""
             + """" or r._field == "quantile_P""".join(
                 [f"{quantile * 100:02.0f}" for quantile in pj["quantiles"]]
             )
             + '"'
         )
+        fields_of_interest_section = (
+            'r._field == "' + '" or r._field == "'.join(FIELDS_OF_INTEREST) + '"'
+        )
 
         if quantiles:
             query = f"""
             from(bucket: "forecast_latest/autogen")
                 |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
                 |> filter(fn: (r) => 
                     r._measurement == "prediction")
                 |> filter(fn: (r) => 
-                   r._field == "forecast" or r._field == "stdev" or r._field == "forecast_other" or r._field == "forecast_solar" or r._field == "forecast_wind_on_shore"{quantile_section})                 
+                   {fields_of_interest_section} {quantile_section})                 
                 |> filter(fn: (r) => r.pid == "{bind_params["pid"]}")
                 |> aggregateWindow(every: {pj["resolution_minutes"]}m, fn: mean)
         """
 
         else:
             query = f"""
                 from(bucket: "forecast_latest/autogen")
                     |> range(start: {bind_params["_start"].strftime('%Y-%m-%dT%H:%M:%SZ')}, stop: {bind_params["_stop"].strftime('%Y-%m-%dT%H:%M:%SZ')}) 
                     |> filter(fn: (r) => 
                         r._measurement == "prediction")
                     |> filter(fn: (r) => 
-                        r._field == "quality" or r._field == "forecast" or r._field == "stdev" or r._field == "forecast_other" or r._field == "forecast_solar" or r._field == "forecast_wind_on_shore")                 
+                        {fields_of_interest_section})                 
                     |> filter(fn: (r) => r.pid == "{bind_params["pid"]}")
                     |> aggregateWindow(every: {pj["resolution_minutes"]}m, fn: mean)
             """
 
         # Query the database
         result = _DataInterface.get_instance().exec_influx_query(query, bind_params)
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.4/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.4/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.4/openstef_dbc/services/systems.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,7 +142,21 @@
         """
 
         result = _DataInterface.get_instance().exec_sql_query(query, bind_params)
         if isinstance(result, pd.DataFrame) and result.empty:
             return ""
         else:
             return result["apiKey"][0]
+
+    def get_api_keys_for_systems(self, sids: list[str]) -> list[str]:
+        """Get (sysetm) API keys that are connected to a given list of systems.
+
+        Args:
+            sid (str): The list with system IDs
+
+        Returns:
+            list(str): The API keys that are connected to the given systems in the list.
+        """
+        api_keys = []
+        for sid in sids:
+            api_keys.append(self.get_api_key_for_system(sid))
+        return list(set(api_keys))
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.4/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/services/write.py` & `openstef_dbc-3.6.4/openstef_dbc/services/write.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from typing import Tuple, List
 from datetime import datetime
 import time
 
 import numpy as np
 import pandas as pd
-from influxdb_client.rest import ApiException
 
 from openstef_dbc.data_interface import _DataInterface
 from openstef_dbc.log import logging
 
 
 class Write:
     def __init__(self):
@@ -111,15 +110,15 @@
                 field_columns=field_columns,
             )
             message += f"Written {num_rows} rows to {dbname}.{influxtable}"
 
         # If desired, write tAhead series to influx - tAhead table
         if t_ahead_series:
             if len(forecast) == 0:
-                self.logger.info("Len forecasts=0, not going to write them to tAheads")
+                message += "Len forecasts=0, not going to write them to tAheads"
                 return message
             message += self._write_t_ahead_series(forecast=forecast, dbname=dbname)
 
         return message
 
     def _write_t_ahead_series(
         self, forecast: pd.DataFrame, dbname: str = "forecast_latest"
@@ -161,47 +160,31 @@
             [x for x in allowed_columns if x in t_adf.columns],
         ]
         tag_columns = ["pid", "customer", "type", "tAhead"]
         field_columns = [x for x in t_adf.columns if x not in tag_columns]
 
         # Force a hard typecast so floats are definetly stored as floats!
         float_columns = ["tAhead", "forecast", "stdev"] + quantile_forecasts
-        t_adf[float_columns] = t_adf[float_columns].apply(
+        float_columns_in_dataframe = [
+            df_column for df_column in t_adf.columns if df_column in float_columns
+        ]
+        t_adf[float_columns_in_dataframe] = t_adf[float_columns_in_dataframe].apply(
             pd.to_numeric, downcast="float", errors="coerce"
         )
 
-        try:
-            result = _DataInterface.get_instance().exec_influx_write(
-                t_adf.copy(),
-                database=dbname,
-                measurement=influxtable,
-                tag_columns=tag_columns,
-                field_columns=field_columns,
-                time_precision="s",
-            )
-            if not result:
-                return ""
-
-        # Temporary workaround for invalid dtypes in tAheads (FK@20230331; expected to be required until 20230407, since then shard rolls over)
-        except ApiException:
-            self.logger.exception(
-                "Invalid dtypes for fiels, writing to *field*_temp instead"
-            )
-            # rename field_columns to '_temp' so they are still stored
-            rename_dict = {colname: f"{colname}_temp" for colname in float_columns}
-            result = _DataInterface.get_instance().exec_influx_write(
-                t_adf.copy().rename(columns=rename_dict),
-                database=dbname,
-                measurement=influxtable,
-                tag_columns=tag_columns,
-                field_columns=list(rename_dict.values()),
-                time_precision="s",
-            )
-            if not result:
-                return ""
+        result = _DataInterface.get_instance().exec_influx_write(
+            t_adf.copy(),
+            database=dbname,
+            measurement=influxtable,
+            tag_columns=tag_columns,
+            field_columns=field_columns,
+            time_precision="s",
+        )
+        if not result:
+            return ""
 
         num_rows = str(len(t_adf))
         self.logger.info(
             "Succesfully written t ahead series to database",
             num_rows=num_rows,
             database=dbname,
             measurement=influxtable,
@@ -272,15 +255,15 @@
             )
             self.logger.info(
                 "Successfully written tags to database", tag_columns=tag_columns
             )
 
         return message
 
-    def write_realised_power_measurements(self, df: pd.DataFrame, sid: str):
+    def write_realised(self, df: pd.DataFrame, sid: str):
         """Method that writes measurement data to the influx database.
 
         Args:
             df: pd.DataFrame(index = "datetime", columns = ['output'])
             sid: (str) String with system id of the measurement
 
         Returns:
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc/utils.py` & `openstef_dbc-3.6.4/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.4/openstef_dbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.3a0
+Version: 3.6.4
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.3a0/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.4/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.3a0/setup.py` & `openstef_dbc-3.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.3a",
+    version="3.6.4",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

