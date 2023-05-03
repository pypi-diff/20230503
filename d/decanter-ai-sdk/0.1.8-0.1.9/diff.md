# Comparing `tmp/decanter-ai-sdk-0.1.8.tar.gz` & `tmp/decanter-ai-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decanter-ai-sdk-0.1.8.tar", max compression
+gzip compressed data, was "decanter-ai-sdk-0.1.9.tar", max compression
```

## Comparing `decanter-ai-sdk-0.1.8.tar` & `decanter-ai-sdk-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/LICENSE
--rw-r--r--   0        0        0     4508 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/README.md
--rw-r--r--   0        0        0       22 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/__init__.py
--rw-r--r--   0        0        0    22632 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/client.py
--rw-r--r--   0        0        0      696 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/algorithms.py
--rw-r--r--   0        0        0      132 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/data_types.py
--rw-r--r--   0        0        0     1018 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/evaluators.py
--rw-r--r--   0        0        0      372 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/missing_value_handling.py
--rw-r--r--   0        0        0      152 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/status.py
--rw-r--r--   0        0        0      118 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/time_units.py
--rw-r--r--   0        0        0     5382 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/experiment.py
--rw-r--r--   0        0        0      285 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/model.py
--rw-r--r--   0        0        0    24678 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/non_blocking_client.py
--rw-r--r--   0        0        0      669 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/prediction.py
--rw-r--r--   0        0        0     1189 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/api.py
--rw-r--r--   0        0        0    15145 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_exp.json
--rw-r--r--   0        0        0      897 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_predict.json
--rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_test_table.json
--rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_train_table.json
--rw-r--r--   0        0        0    80346 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/model_list.json
--rw-r--r--   0        0        0      365 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/table_info.json
--rw-r--r--   0        0        0     4128 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/table_list.json
--rw-r--r--   0        0        0    39974 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_exp.json
--rw-r--r--   0        0        0      897 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_predict.json
--rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_test_table.json
--rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_train_table.json
--rw-r--r--   0        0        0     7513 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/decanter_api.py
--rw-r--r--   0        0        0     2618 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/iid_testing_api.py
--rw-r--r--   0        0        0     2645 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/ts_testing_api.py
--rw-r--r--   0        0        0     1563 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5794 2023-04-14 02:25:48.049560 decanter-ai-sdk-0.1.8/setup.py
--rw-r--r--   0        0        0     5475 2023-04-14 02:25:48.050036 decanter-ai-sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-28 07:52:31.520841 decanter-ai-sdk-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4506 2023-04-28 07:52:31.520841 decanter-ai-sdk-0.1.9/README.md
+-rw-r--r--   0        0        0       22 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/__init__.py
+-rw-r--r--   0        0        0    24125 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/client.py
+-rw-r--r--   0        0        0      696 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/algorithms.py
+-rw-r--r--   0        0        0      132 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/data_types.py
+-rw-r--r--   0        0        0     1018 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/evaluators.py
+-rw-r--r--   0        0        0      372 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/missing_value_handling.py
+-rw-r--r--   0        0        0      152 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/status.py
+-rw-r--r--   0        0        0      118 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/time_units.py
+-rw-r--r--   0        0        0     5382 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/experiment.py
+-rw-r--r--   0        0        0      285 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/model.py
+-rw-r--r--   0        0        0    24744 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/non_blocking_client.py
+-rw-r--r--   0        0        0      669 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/prediction.py
+-rw-r--r--   0        0        0     1189 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/api.py
+-rw-r--r--   0        0        0    15145 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_exp.json
+-rw-r--r--   0        0        0      897 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_predict.json
+-rw-r--r--   0        0        0     1914 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_test_table.json
+-rw-r--r--   0        0        0     1914 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_train_table.json
+-rw-r--r--   0        0        0    80346 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/model_list.json
+-rw-r--r--   0        0        0      365 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/table_info.json
+-rw-r--r--   0        0        0     4128 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/table_list.json
+-rw-r--r--   0        0        0    39974 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_exp.json
+-rw-r--r--   0        0        0      897 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_predict.json
+-rw-r--r--   0        0        0     1914 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_test_table.json
+-rw-r--r--   0        0        0     1914 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_train_table.json
+-rw-r--r--   0        0        0     9117 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/decanter_api.py
+-rw-r--r--   0        0        0     2618 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/iid_testing_api.py
+-rw-r--r--   0        0        0     2645 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/ts_testing_api.py
+-rw-r--r--   0        0        0     1563 2023-04-28 07:52:31.524841 decanter-ai-sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5792 2023-04-28 07:52:44.319301 decanter-ai-sdk-0.1.9/setup.py
+-rw-r--r--   0        0        0     5473 2023-04-28 07:52:44.319757 decanter-ai-sdk-0.1.9/PKG-INFO
```

### Comparing `decanter-ai-sdk-0.1.8/LICENSE` & `decanter-ai-sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/README.md` & `decanter-ai-sdk-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 ```python
 # Training iid data
 experiment = client.train_iid(
     experiment_name=exp_name,
     experiment_table_id=train_id,
     target="Survived",
     evaluator=ClassificationMetric.AUC,
-    custom_feature_types={
+    custom_column_types={
         "Pclass": DataType.categorical,
         "Parch": DataType.categorical,
     },
 )
 ```
 
 ```python
@@ -74,15 +74,15 @@
     target="Passengers",
     datetime="Month",
     time_groups=[],
     timeunit=TimeUnit.month,
     groupby_method="sum",
     max_model=5,
     evaluator=RegressionMetric.MAPE,
-    custom_feature_types={"Pclass": DataType.numerical},
+    custom_column_types={"Pclass": DataType.numerical},
 )
 ```
 To get its attributes, you can either extract them by simply using dot or its functions.
 ```python
 # Experiment object usage
 best_model = experiment.get_best_model()
 model_list = experiment.get_model_list()
```

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/client.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return res["_id"]
 
     def train_iid(
         self,
         experiment_name: str,
         experiment_table_id: str,
         target: str,
-        custom_feature_types: Dict[str, DataType] = {},
+        custom_column_types: Dict[str, DataType] = {},
         drop_features: List[str] = [],
         evaluator: Optional[Union[RegressionMetric, ClassificationMetric]] = None,
         holdout_table_id: Optional[str] = None,
         algos: Union[List[IIDAlgorithms], List[str]] = [
             IIDAlgorithms.DRF,
             IIDAlgorithms.GBM,
             IIDAlgorithms.XGBoost,
@@ -127,15 +127,15 @@
         ----------
             experiment_name (str)
                 Name of the experiment.
             experiment_table_id (str)
                 Id for the table used in experiment.
             target (str)
                 Name of the target column.
-            custom_feature_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
+            custom_column_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
                 Set customized feature types by inputting {feature_name_1: feature_type_1, feature_name_2: feature_type_2}.
             missing_value_settings (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
                 Set missing value handling method by inputting {feature_name_1: feature_type_1, feature_name_2: feature_type_2}.
             drop_features (List[str])
                 Feature names that are not going to be used during experiment.
             evaluator (Union[`~decanter_ai_sdk.enums.evaluators.ClassificationMetric`, `~decanter_ai_sdk.enums.evaluators.RegressionMetric`])
                 Evaluator used as stopping metric.
@@ -194,15 +194,15 @@
                 Experiment results.
         """
 
         exp_id = self.non_blocking_client.train_iid(
             experiment_name=experiment_name,
             experiment_table_id=experiment_table_id,
             target=target,
-            custom_feature_types=custom_feature_types,
+            custom_column_types=custom_column_types,
             drop_features=drop_features,
             evaluator=evaluator,
             holdout_table_id=holdout_table_id,
             algos=algos,
             max_model=max_model,
             tolerance=tolerance,
             nfold=nfold,
@@ -256,15 +256,15 @@
         horizon_window: int = 1,
         validation_percentage: int = 10,
         nfold: int = 5,
         max_model: int = 20,
         tolerance: int = 3,
         seed: int = 1111,
         drop_features: List[str] = [],
-        custom_feature_types: Dict[str, DataType] = {},
+        custom_column_types: Dict[str, DataType] = {},
         holdout_percentage: int = 10,
         missing_value_settings: Dict[str, MissingValueHandling] = {},
     ) -> Experiment:
         """
         Train timeseries models.
 
         Parameters:
@@ -273,15 +273,15 @@
                 Name of the experiment.
             experiment_table_id (str)
                 Id for the table used in experiment.
             target (str)
                 Name of the target column.
             datetime (str)
                 Date-time column for Time Series Forecast training.
-            custom_feature_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
+            custom_column_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
                 Set customized feature types by inputting {feature_name_1: feature_type_1, feature_name_2: feature_type_2}.
             evaluator (`~decanter_ai_sdk.enums.evaluators.ClassificationMetric`, `~decanter_ai_sdk.enums.evaluators.RegressionMetric`)
                 Evaluator used as stopping metric.
             algos (List[`~decanter_ai_sdk.enums.algorithms.IIDAlgorithms`],  List[`~decanter_ai_sdk.enums.algorithms.TSAlgorithms`])
                 Algorithms used for experiment.
             max_model (int)
                 Limit for the number of models to train for this experiment.
@@ -334,15 +334,15 @@
             exogeneous_columns_list=exogeneous_columns_list,
             gap=gap,
             feature_derivation_window=feature_derivation_window,
             horizon_window=horizon_window,
             validation_percentage=validation_percentage,
             nfold=nfold,
             drop_features=drop_features,
-            custom_feature_types=custom_feature_types,
+            custom_column_types=custom_column_types,
             max_model=max_model,
             tolerance=tolerance,
             holdout_percentage=holdout_percentage,
             seed=seed,
         )
 
         experiment = Experiment.parse_obj(self.wait_for_response("experiment", exp_id))
@@ -461,14 +461,47 @@
             attributes=self.wait_for_response("prediction", pred_id)
         )
         prediction.predict_df = self.api.get_pred_data(
             prediction.attributes["_id"], download
         )
         return prediction
 
+    def batch_predict(
+        self,
+        pred_df: pd.DataFrame,
+        experiment_id: str,
+        model_id: str,
+        timestamp_format: str = "yyyy-MM-dd",
+    ) -> pd.Series:
+        """
+        Predict model with pd.DataFrame.
+
+        The output can't show on Decanter AI.
+
+        Parameters:
+        ----------
+            pred_df (pd.DataFrame)
+                Prediction data
+            model_id (str)
+                Id of model used to predict.
+            experiment_id (str)
+                Id of experiment used to predict.
+            timestamp_format (str)
+                Timestamp format, default: "yyyy-MM-dd"
+                (ref: https://en.wikipedia.org/wiki/ISO_8601)
+
+        Returns:
+        ----------
+            (pd.Series)
+                Prediction results.
+        """
+        return self.api.batch_predict(
+            pred_df, experiment_id, model_id, timestamp_format
+        )
+
     def stop_uploading(self, id: str) -> None:
         self.non_blocking_client.stop_uploading(id)
 
     def stop_training(self, id: str) -> None:
         self.non_blocking_client.stop_training(id)
 
     def wait_for_response(self, url, id):
@@ -509,14 +542,35 @@
         Returns:
         ----------
             (pandas.DataFrame)
                 Uploaded table dataframe.
         """
         return self.api.get_table(data_id=data_id)
 
+    def update_table(
+        self, table_id: str, updated_column: str, updated_type: str
+    ) -> None:
+        """
+        update columns type.
+
+        Params:
+        ----------
+            table_id (str)
+                table id which want to update type
+            updated_column (str)
+                column which want to update type
+            updated_type (str)
+                including: categorical, numerical, datetime, id
+
+        Returns:
+        ----------
+           None
+        """
+        return self.api.update_table(table_id, updated_column, updated_type)
+
     def get_table_list(self, page=1) -> List[str]:
         """
         Return list of table information.
 
         Args:
             page (int): page number.
```

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/algorithms.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/algorithms.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/evaluators.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/enums/evaluators.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/experiment.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/experiment.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/non_blocking_client.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/non_blocking_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,29 +86,29 @@
 
         if data is None:
             raise ValueError("[Upload] Uploaded None file.")  # pragma: no cover
 
         if isinstance(data, pd.DataFrame):
             text_stream = StringIO()
             data.to_csv(text_stream, index=False)
-            file = [("file", (name, text_stream.getvalue(), "text/csv"))]
+            file = (name, text_stream.getvalue(), "text/csv")
             text_stream.close()
 
         else:
-            file = [("file", (name, data, "text/csv"))]
+            file = (name, data, "text/csv")
         table_id = self.api.post_upload(file=file, name=name)
 
         return table_id
 
     def train_iid(
         self,
         experiment_name: str,
         experiment_table_id: str,
         target: str,
-        custom_feature_types: Dict[str, DataType] = {},
+        custom_column_types: Dict[str, DataType] = {},
         drop_features: List[str] = [],
         evaluator: Optional[Union[RegressionMetric, ClassificationMetric]] = None,
         holdout_table_id: Optional[str] = None,
         algos: Union[List[IIDAlgorithms], List[str]] = [
             IIDAlgorithms.DRF,
             IIDAlgorithms.GBM,
             IIDAlgorithms.XGBoost,
@@ -131,15 +131,15 @@
         ----------
             experiment_name (str)
                 Name of the experiment.
             experiment_table_id (str)
                 Id for the table used in experiment.
             target (str)
                 Name of the target column.
-            custom_feature_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
+            custom_column_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
                 Set customized feature types by inputting {feature_name_1: feature_type_1, feature_name_2: feature_type_2}.
             drop_features (List[str])
                 Feature names that are not going to be used during experiment.
             evaluator (Union[`~decanter_ai_sdk.enums.evaluators.ClassificationMetric`, `~decanter_ai_sdk.enums.evaluators.RegressionMetric`])
                 Evaluator used as stopping metric.
             holdout_table_id (str)
                 Id of the table used to perform holdout.
@@ -192,14 +192,16 @@
 
         Returns:
         ----------
             (`~decanter_ai_sdk.web_api.experiment.Experiment`)
                 Experiment id.
         """
         data_column_info = self.api.get_table_info(table_id=experiment_table_id)
+        # cast target column
+        data_column_info[target] = custom_column_types[target].value
 
         if validation_percentage < 5 or validation_percentage > 20:
             raise ValueError(
                 "validation_percentage should be inside a range between 5 to 20."
             )  # pragma: no cover
 
         algo_values = []
@@ -217,16 +219,16 @@
 
         feature_types = [
             {"id": k, "data_type": j}
             for k, j in {key: data_column_info[key] for key in features}.items()
         ]
 
         for feature in feature_types:
-            if feature["id"] in custom_feature_types.keys():
-                feature["data_type"] = custom_feature_types[feature["id"]].value
+            if feature["id"] in custom_column_types.keys():
+                feature["data_type"] = custom_column_types[feature["id"]].value
 
         column_list = []
         for column in missing_value_settings.keys():
             column_list.append(
                 {
                     "columnName": column,
                     "method": {"imputation": missing_value_settings[column].value},
@@ -303,15 +305,15 @@
         horizon_window: int = 1,
         validation_percentage: int = 10,
         nfold: int = 5,
         max_model: int = 20,
         tolerance: int = 3,
         seed: int = 1111,
         drop_features: List[str] = [],
-        custom_feature_types: Dict[str, DataType] = {},
+        custom_column_types: Dict[str, DataType] = {},
         holdout_percentage: int = 10,
         missing_value_settings: Dict[str, MissingValueHandling] = {},
     ) -> str:
         """
         Train timeseries models.
 
         Parameters:
@@ -320,15 +322,15 @@
                 Name of the experiment.
             experiment_table_id (str)
                 Id for the table used in experiment.
             target (str)
                 Name of the target column.
             datetime (str)
                 Date-time column for Time Series Forecast training.
-            custom_feature_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
+            custom_column_types (Dict[str: `~decanter_ai_sdk.enums.data_type.DataType`])
                 Set customized feature types by inputting {feature_name_1: feature_type_1, feature_name_2: feature_type_2}.
             evaluator (`~decanter_ai_sdk.enums.evaluators.ClassificationMetric`, `~decanter_ai_sdk.enums.evaluators.RegressionMetric`)
                 Evaluator used as stopping metric.
             algos (List[`~decanter_ai_sdk.enums.algorithms.IIDAlgorithms`],  List[`~decanter_ai_sdk.enums.algorithms.TSAlgorithms`])
                 Algorithms used for experiment.
             max_model (int)
                 Limit for the number of models to train for this experiment.
@@ -388,16 +390,16 @@
 
         feature_types = [
             {"id": k, "data_type": j}
             for k, j in {key: data_column_info[key] for key in features}.items()
         ]
 
         for feature in feature_types:
-            if feature["id"] in custom_feature_types.keys():
-                feature["data_type"] = custom_feature_types[feature["id"]].value
+            if feature["id"] in custom_column_types.keys():
+                feature["data_type"] = custom_column_types[feature["id"]].value
 
         column_list = []
         for column in missing_value_settings.keys():
             column_list.append(
                 {
                     "columnName": column,
                     "method": {"imputation": missing_value_settings[column]},
```

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/prediction.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/prediction.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/api.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_exp.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_exp.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_predict.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_predict.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_test_table.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_test_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_train_table.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/iid_train_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/model_list.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/model_list.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/table_list.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/table_list.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_exp.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_exp.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_predict.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_predict.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_test_table.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_test_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_train_table.json` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/data/ts_train_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/decanter_api.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/decanter_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 from io import StringIO
 import json
 import requests
 import pandas as pd
 import numpy as np
 
 from decanter_ai_sdk.web_api.api import ApiClient
+from requests_toolbelt import MultipartEncoder
 
 
 class DecanterApiClient(ApiClient):
     def __init__(self, host, headers, auth_headers, project_id):  # pragma: no cover
         self.url = host + "/v1/"
         self.headers = headers
         self.project_id = project_id
         self.auth_headers = auth_headers
 
-    def post_upload(self, file: Dict, name: str):  # pragma: no cover
+    def post_upload(self, file: tuple, name: str):  # pragma: no cover
+
+        m = MultipartEncoder(
+            fields={"project_id": self.project_id, "name": name, "file": file}
+        )
+        headers = self.auth_headers
+        headers["Content-Type"] = m.content_type
 
         res = requests.post(
             f"{self.url}table/upload",
-            files=file,
-            data={"name": name, "project_id": self.project_id},
-            headers=self.auth_headers,
+            data=m,
+            headers=headers,
             verify=False,
         )
 
         if not res.ok:
             raise RuntimeError(res.json()["message"])
         return res.json()["table"]["_id"]
 
@@ -63,28 +69,72 @@
             verify=False,
         )
         if not res.ok:
             raise RuntimeError(res.json()["message"])
 
         return res.json()["prediction"]["_id"]
 
+    def batch_predict(
+        self,
+        pred_df: pd.DataFrame,
+        experiment_id: str,
+        model_id: str,
+        timestamp_format: str,
+    ) -> pd.Series:
+
+        data = {
+            "project_id": self.project_id,
+            "featuresList": pred_df.to_dict(orient="records"),
+            "timestamp_format": timestamp_format,
+        }
+
+        res = requests.post(
+            f"{self.url}experiment/{experiment_id}/model/{model_id}/batch_predict",
+            headers=self.headers,
+            data=json.dumps(data),
+            verify=False,
+        )
+
+        if not res.ok:
+            raise RuntimeError(res.json()["message"])
+
+        return pd.DataFrame(res.json()["data"])["prediction"]
+
     def get_table_info(self, table_id):  # pragma: no cover
 
         table_response = requests.get(
             f"{self.url}table/{table_id}/columns", headers=self.headers, verify=False
         )
         table_info = {}
 
         if not table_response.ok:
             raise RuntimeError(table_response.json()["message"])
 
         for column in table_response.json()["columns"]:
             table_info[column["id"]] = column["data_type"]
         return table_info
 
+    def update_table(self, table_id, updated_column, updated_type) -> None:
+        data = {
+            "project_id": self.project_id,
+            "columns": [{"data_type": updated_type, "id": updated_column}],
+            "table_id": table_id,
+        }
+        data = json.dumps(data)
+        update_response = requests.put(
+            f"{self.url}table/update", headers=self.headers, data=data, verify=False
+        )
+        if update_response.status_code == 200:
+            print("Update Successfully!!")
+        else:
+            print(f"Update Fail - {update_response.status_code}")
+            print(
+                "typo? Only categorical, numerical, datetime, and id can be filled in"
+            )
+
     def check(self, task, id):  # pragma: no cover
         if task == "table":
 
             res = requests.get(
                 f"{self.url}table/{id}",
                 verify=False,
                 headers=self.headers,
```

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/iid_testing_api.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/iid_testing_api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/ts_testing_api.py` & `decanter-ai-sdk-0.1.9/decanter_ai_sdk/web_api/ts_testing_api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.8/pyproject.toml` & `decanter-ai-sdk-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decanter-ai-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "Decanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python."
 homepage = "https://github.com/MoBagel/decanter-ai-sdk"
 authors = ["senchao <senchao@mobagel.com>"]
 readme = "README.md"
 include = [
   "README.md"
 ]
```

### Comparing `decanter-ai-sdk-0.1.8/setup.py` & `decanter-ai-sdk-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'pydantic>=1.9.2,<2.0.0',
  'pytest>=7.1.2,<8.0.0',
  'requests-toolbelt>=0.9.1,<0.10.0',
  'tqdm>=4.64.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'decanter-ai-sdk',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Decanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.',
-    'long_description': '[![Coverage Status](https://coveralls.io/repos/github/MoBagel/decanter-ai-sdk/badge.svg?branch=coveralls)](https://coveralls.io/github/MoBagel/decanter-ai-sdk?branch=coveralls)\n[![tests](https://github.com/MoBagel/decanter-ai-sdk/workflows/main/badge.svg)](https://github.com/MoBagel/decanter-ai-sdk)\n[![PyPI version](https://badge.fury.io/py/decanter-ai-sdk.svg)](https://badge.fury.io/py/decanter-ai-sdk)\n# Mobagel decanter ai sdk\n\nDecanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.\n\nIt supports actions such as data uploading, model training, and prediction to run in a more efficient way and access results more easily.\n\nTo know more about Decanter AI and how you can be benefited with AutoML, visit [MoBagel website](https://mobagel.com/tw/) and contact us to try it out!\n\n## How it works\n\n- Upload train and test files in both csv and pandas dataframe.\n- Setup different standards and conduct customized experiments on uploaded data.\n- Use different models to run predictions\n- Get predict data in pandas dataframe form.\n\n## Requirements\n\n- [Python >= 3.8](https://www.python.org/downloads/release/python-380/)\n- [poetry](https://python-poetry.org/)\n\n## Usage\n\n### Installation\n\n`pip install decanter-ai-sdk`\n### Constructor\nTo use this sdk, you must first construct a client object.\n```python\nfrom decanter_ai_sdk.client import Client\n    client = Client(\n        auth_key="auth_API_key",\n        project_id="project_id",\n        host="host_url",\n    )\n```\n\n### Upload\nAfter the client is constructed, now you can use it to upload your training and testing files in both csv and pandas dataframe. This function will return uploaded data id in Decanter server.\n```python\nimport os\nsys.path.append("..")\n\ncurrent_path = os.path.dirname(os.path.abspath(__file__))\ntrain_file_path = os.path.join(current_path, "ts_train.csv")\ntrain_file = open(train_file_path, "rb")\ntrain_id = client.upload(train_file, "train_file")\n```\n\n### Experiment\nTo conduct an experiment, you need to first specify which type of data you are going to use , i.e., iid or ts, then you can input parameters by following our pyhint to customize your experiment.\nAfter the experiment, the function will return an object which you can get experiment attributes from it.\n```python\n# Training iid data\nexperiment = client.train_iid(\n    experiment_name=exp_name,\n    experiment_table_id=train_id,\n    target="Survived",\n    evaluator=ClassificationMetric.AUC,\n    custom_feature_types={\n        "Pclass": DataType.categorical,\n        "Parch": DataType.categorical,\n    },\n)\n```\n\n```python\n# Training ts data\nexperiment = client.train_ts(\n    experiment_name=exp_name,\n    experiment_table_id=train_id,\n    target="Passengers",\n    datetime="Month",\n    time_groups=[],\n    timeunit=TimeUnit.month,\n    groupby_method="sum",\n    max_model=5,\n    evaluator=RegressionMetric.MAPE,\n    custom_feature_types={"Pclass": DataType.numerical},\n)\n```\nTo get its attributes, you can either extract them by simply using dot or its functions.\n```python\n# Experiment object usage\nbest_model = experiment.get_best_model()\nmodel_list = experiment.get_model_list()\nbest_auc_model = experiment.get_best_model_by_metric(ClassificationMetric.AUC)\n```\n### Prediction\nNow you can use model data to run prediction.\n```python\n# Predicting iid data\npredict = client.predict_iid(\n    keep_columns=[], \n    non_negative=False, \n    test_table_id=test_id, \n    model=best_model\n)\n```\n\n```python\n# Predicting ts data\npredict = client.predict_ts(\n    keep_columns=[], \n    non_negative=False, \n    test_table_id=test_id, \n    model=best_model\n)\n```\nTo get prediction result, do\n```python\npredict_data = predict.get_predict_df()\n```\n## Development\n\n### Installing poetry\n\n1. `pip install poetry poethepoet`\n2. `poetry install` #Project setup.\n3. `poetry shell` #Start your project in poetry env.\n\nNow you can create your own branch to start developing new feature.\n\n### Testing\nTo run test, do:\n```\npoe test\n```\n\n### Lint and format\nTo lint, do:\n```\npoe lint\n```\n\nTo reformat, do:\n```\npoe format\n```\n\n## Releasing\n1. poetry version [new_version]\n2. git commit -m"Bump version"\n3. git push origin main\n4. create new release on github.\n5. Create release off main branch, auto generate notes, and review release note.\n6. Publish release\n\n## Enums\n#TODO\n\n## License\n#TODO\n\n## TODO\n#TODO\n\n\n\n',
+    'long_description': '[![Coverage Status](https://coveralls.io/repos/github/MoBagel/decanter-ai-sdk/badge.svg?branch=coveralls)](https://coveralls.io/github/MoBagel/decanter-ai-sdk?branch=coveralls)\n[![tests](https://github.com/MoBagel/decanter-ai-sdk/workflows/main/badge.svg)](https://github.com/MoBagel/decanter-ai-sdk)\n[![PyPI version](https://badge.fury.io/py/decanter-ai-sdk.svg)](https://badge.fury.io/py/decanter-ai-sdk)\n# Mobagel decanter ai sdk\n\nDecanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.\n\nIt supports actions such as data uploading, model training, and prediction to run in a more efficient way and access results more easily.\n\nTo know more about Decanter AI and how you can be benefited with AutoML, visit [MoBagel website](https://mobagel.com/tw/) and contact us to try it out!\n\n## How it works\n\n- Upload train and test files in both csv and pandas dataframe.\n- Setup different standards and conduct customized experiments on uploaded data.\n- Use different models to run predictions\n- Get predict data in pandas dataframe form.\n\n## Requirements\n\n- [Python >= 3.8](https://www.python.org/downloads/release/python-380/)\n- [poetry](https://python-poetry.org/)\n\n## Usage\n\n### Installation\n\n`pip install decanter-ai-sdk`\n### Constructor\nTo use this sdk, you must first construct a client object.\n```python\nfrom decanter_ai_sdk.client import Client\n    client = Client(\n        auth_key="auth_API_key",\n        project_id="project_id",\n        host="host_url",\n    )\n```\n\n### Upload\nAfter the client is constructed, now you can use it to upload your training and testing files in both csv and pandas dataframe. This function will return uploaded data id in Decanter server.\n```python\nimport os\nsys.path.append("..")\n\ncurrent_path = os.path.dirname(os.path.abspath(__file__))\ntrain_file_path = os.path.join(current_path, "ts_train.csv")\ntrain_file = open(train_file_path, "rb")\ntrain_id = client.upload(train_file, "train_file")\n```\n\n### Experiment\nTo conduct an experiment, you need to first specify which type of data you are going to use , i.e., iid or ts, then you can input parameters by following our pyhint to customize your experiment.\nAfter the experiment, the function will return an object which you can get experiment attributes from it.\n```python\n# Training iid data\nexperiment = client.train_iid(\n    experiment_name=exp_name,\n    experiment_table_id=train_id,\n    target="Survived",\n    evaluator=ClassificationMetric.AUC,\n    custom_column_types={\n        "Pclass": DataType.categorical,\n        "Parch": DataType.categorical,\n    },\n)\n```\n\n```python\n# Training ts data\nexperiment = client.train_ts(\n    experiment_name=exp_name,\n    experiment_table_id=train_id,\n    target="Passengers",\n    datetime="Month",\n    time_groups=[],\n    timeunit=TimeUnit.month,\n    groupby_method="sum",\n    max_model=5,\n    evaluator=RegressionMetric.MAPE,\n    custom_column_types={"Pclass": DataType.numerical},\n)\n```\nTo get its attributes, you can either extract them by simply using dot or its functions.\n```python\n# Experiment object usage\nbest_model = experiment.get_best_model()\nmodel_list = experiment.get_model_list()\nbest_auc_model = experiment.get_best_model_by_metric(ClassificationMetric.AUC)\n```\n### Prediction\nNow you can use model data to run prediction.\n```python\n# Predicting iid data\npredict = client.predict_iid(\n    keep_columns=[], \n    non_negative=False, \n    test_table_id=test_id, \n    model=best_model\n)\n```\n\n```python\n# Predicting ts data\npredict = client.predict_ts(\n    keep_columns=[], \n    non_negative=False, \n    test_table_id=test_id, \n    model=best_model\n)\n```\nTo get prediction result, do\n```python\npredict_data = predict.get_predict_df()\n```\n## Development\n\n### Installing poetry\n\n1. `pip install poetry poethepoet`\n2. `poetry install` #Project setup.\n3. `poetry shell` #Start your project in poetry env.\n\nNow you can create your own branch to start developing new feature.\n\n### Testing\nTo run test, do:\n```\npoe test\n```\n\n### Lint and format\nTo lint, do:\n```\npoe lint\n```\n\nTo reformat, do:\n```\npoe format\n```\n\n## Releasing\n1. poetry version [new_version]\n2. git commit -m"Bump version"\n3. git push origin main\n4. create new release on github.\n5. Create release off main branch, auto generate notes, and review release note.\n6. Publish release\n\n## Enums\n#TODO\n\n## License\n#TODO\n\n## TODO\n#TODO\n\n\n\n',
     'author': 'senchao',
     'author_email': 'senchao@mobagel.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/MoBagel/decanter-ai-sdk',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `decanter-ai-sdk-0.1.8/PKG-INFO` & `decanter-ai-sdk-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decanter-ai-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Decanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.
 Home-page: https://github.com/MoBagel/decanter-ai-sdk
 Author: senchao
 Author-email: senchao@mobagel.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -76,15 +76,15 @@
 ```python
 # Training iid data
 experiment = client.train_iid(
     experiment_name=exp_name,
     experiment_table_id=train_id,
     target="Survived",
     evaluator=ClassificationMetric.AUC,
-    custom_feature_types={
+    custom_column_types={
         "Pclass": DataType.categorical,
         "Parch": DataType.categorical,
     },
 )
 ```
 
 ```python
@@ -95,15 +95,15 @@
     target="Passengers",
     datetime="Month",
     time_groups=[],
     timeunit=TimeUnit.month,
     groupby_method="sum",
     max_model=5,
     evaluator=RegressionMetric.MAPE,
-    custom_feature_types={"Pclass": DataType.numerical},
+    custom_column_types={"Pclass": DataType.numerical},
 )
 ```
 To get its attributes, you can either extract them by simply using dot or its functions.
 ```python
 # Experiment object usage
 best_model = experiment.get_best_model()
 model_list = experiment.get_model_list()
```

