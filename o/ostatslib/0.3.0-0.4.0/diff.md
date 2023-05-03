# Comparing `tmp/ostatslib-0.3.0.tar.gz` & `tmp/ostatslib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ostatslib-0.3.0.tar", max compression
+gzip compressed data, was "ostatslib-0.4.0.tar", max compression
```

## Comparing `ostatslib-0.3.0.tar` & `ostatslib-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,56 @@
--rw-r--r--   0        0        0     1109 2022-11-24 19:40:02.919568 ostatslib-0.3.0/LICENSE
--rw-r--r--   0        0        0      606 2022-11-24 19:40:02.919568 ostatslib-0.3.0/README.md
--rw-r--r--   0        0        0        0 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/__init__.py
--rw-r--r--   0        0        0      398 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/__init__.py
--rw-r--r--   0        0        0     3922 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/actions_space.py
--rw-r--r--   0        0        0       89 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/classifiers/__init__.py
--rw-r--r--   0        0        0     1827 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/classifiers/logistic_regression.py
--rw-r--r--   0        0        0      393 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/exploratory_actions/__init__.py
--rw-r--r--   0        0        0     1270 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py
--rw-r--r--   0        0        0     2041 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py
--rw-r--r--   0        0        0     1500 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py
--rw-r--r--   0        0        0     1525 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py
--rw-r--r--   0        0        0     1239 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py
--rw-r--r--   0        0        0      135 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/regression_models/__init__.py
--rw-r--r--   0        0        0     3383 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/regression_models/linear_regression.py
--rw-r--r--   0        0        0     2358 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/regression_models/poisson_regression.py
--rw-r--r--   0        0        0      399 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/utils/__init__.py
--rw-r--r--   0        0        0      568 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/utils/action_result.py
--rw-r--r--   0        0        0      441 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/utils/as_binary_array.py
--rw-r--r--   0        0        0     1910 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/utils/explainability_rewards.py
--rw-r--r--   0        0        0      867 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/utils/reward_cap.py
--rw-r--r--   0        0        0      836 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py
--rw-r--r--   0        0        0       48 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/agents/__init__.py
--rw-r--r--   0        0        0     2806 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/agents/agent.py
--rw-r--r--   0        0        0       66 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/environments/__init__.py
--rw-r--r--   0        0        0     1676 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/environments/environment.py
--rw-r--r--   0        0        0      135 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/exploration_strategies/__init__.py
--rw-r--r--   0        0        0      866 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/exploration_strategies/epsilon_greedy.py
--rw-r--r--   0        0        0      693 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/exploration_strategies/exploration_strategy.py
--rw-r--r--   0        0        0      680 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/exploration_strategies/upper_confidence_bounds.py
--rw-r--r--   0        0        0      220 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/__init__.py
--rw-r--r--   0        0        0     7107 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/actor_critic.py
--rw-r--r--   0        0        0     1713 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/reinforcement_learning_method.py
--rw-r--r--   0        0        0     5435 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/support_vector_regression.py
--rw-r--r--   0        0        0      306 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/utils/__init__.py
--rw-r--r--   0        0        0      888 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/utils/build_actor_critic_neural_network.py
--rw-r--r--   0        0        0      487 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/utils/convert_state_to_tensor.py
--rw-r--r--   0        0        0      290 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/utils/model_not_fit_error.py
--rw-r--r--   0        0        0      600 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/reinforcement_learning_methods/utils/normalize_values_list.py
--rw-r--r--   0        0        0       72 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/replay_memories/__init__.py
--rw-r--r--   0        0        0     3060 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/replay_memories/replay_memory.py
--rw-r--r--   0        0        0       48 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/states/__init__.py
--rw-r--r--   0        0        0      396 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/states/analysis_features_set.py
--rw-r--r--   0        0        0      467 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/states/data_features_set.py
--rw-r--r--   0        0        0     3356 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/states/state.py
--rw-r--r--   0        0        0      566 2022-11-24 19:40:02.919568 ostatslib-0.3.0/ostatslib/states/state_iterator.py
--rw-r--r--   0        0        0      927 2022-11-24 19:40:02.923568 ostatslib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 ostatslib-0.3.0/setup.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 ostatslib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-03 20:29:52.561631 ostatslib-0.4.0/LICENSE
+-rw-r--r--   0        0        0      606 2023-05-03 20:29:52.561631 ostatslib-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/__init__.py
+-rw-r--r--   0        0        0      724 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/action.py
+-rw-r--r--   0        0        0     6398 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/actions_space.py
+-rw-r--r--   0        0        0      203 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/__init__.py
+-rw-r--r--   0        0        0     2417 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/decision_tree.py
+-rw-r--r--   0        0        0     2263 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/logistic_regression.py
+-rw-r--r--   0        0        0     2359 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/classifiers/support_vector_classification.py
+-rw-r--r--   0        0        0       91 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/clustering/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/clustering/dbscan.py
+-rw-r--r--   0        0        0     1702 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/clustering/k_means.py
+-rw-r--r--   0        0        0      527 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/__init__.py
+-rw-r--r--   0        0        0      455 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py
+-rw-r--r--   0        0        0     1563 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py
+-rw-r--r--   0        0        0     1764 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py
+-rw-r--r--   0        0        0     2283 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py
+-rw-r--r--   0        0        0     1722 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py
+-rw-r--r--   0        0        0     1763 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py
+-rw-r--r--   0        0        0     1478 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py
+-rw-r--r--   0        0        0     2872 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py
+-rw-r--r--   0        0        0      322 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/__init__.py
+-rw-r--r--   0        0        0     2256 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/decision_tree_regression.py
+-rw-r--r--   0        0        0     5741 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/linear_regression.py
+-rw-r--r--   0        0        0     3222 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/poisson_regression.py
+-rw-r--r--   0        0        0     2396 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/support_vector_regression.py
+-rw-r--r--   0        0        0     4669 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/regression_models/time_series_auto_arima.py
+-rw-r--r--   0        0        0      453 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/as_binary_array.py
+-rw-r--r--   0        0        0      424 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/calculate_score_reward.py
+-rw-r--r--   0        0        0     1837 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/explainability_rewards.py
+-rw-r--r--   0        0        0      815 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/reward_cap.py
+-rw-r--r--   0        0        0      841 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py
+-rw-r--r--   0        0        0      530 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/actions/utils/update_state_score.py
+-rw-r--r--   0        0        0      124 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/__init__.py
+-rw-r--r--   0        0        0     2175 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/agent.py
+-rw-r--r--   0        0        0     1664 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/analysis_result.py
+-rw-r--r--   0        0        0     1913 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/agents/ppo_agent.py
+-rw-r--r--   0        0        0       73 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/__init__.py
+-rw-r--r--   0        0        0     2630 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/gym_environment.py
+-rw-r--r--   0        0        0      101 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/__init__.py
+-rw-r--r--   0        0        0     1106 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/_generate_from_datacooker.py
+-rw-r--r--   0        0        0     3297 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/_generate_from_sklearn.py
+-rw-r--r--   0        0        0      500 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/environments/utils/generate_training_dataset.py
+-rw-r--r--   0        0        0       48 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/states/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/states/analysis_features_set.py
+-rw-r--r--   0        0        0     2096 2023-05-03 20:29:52.561631 ostatslib-0.4.0/ostatslib/states/data_features_set.py
+-rw-r--r--   0        0        0     1890 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/features_set.py
+-rw-r--r--   0        0        0     1289 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/models_features_set.py
+-rw-r--r--   0        0        0     5033 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/state.py
+-rw-r--r--   0        0        0      604 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/state_iterator.py
+-rw-r--r--   0        0        0       82 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/utils/__init__.py
+-rw-r--r--   0        0        0      937 2023-05-03 20:29:52.565631 ostatslib-0.4.0/ostatslib/states/utils/init_features_set.py
+-rw-r--r--   0        0        0     1002 2023-05-03 20:29:52.565631 ostatslib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 ostatslib-0.4.0/PKG-INFO
```

### Comparing `ostatslib-0.3.0/LICENSE` & `ostatslib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ostatslib-0.3.0/README.md` & `ostatslib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ostatslib-0.3.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py` & `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
 get_log_rows_count module
 """
 
 import numpy as np
 from pandas import DataFrame
-from ostatslib.actions.utils import ActionResult
+from ostatslib.actions import Action, ActionInfo, ActionResult
 from ostatslib.states import State
 
+_ACTION_NAME = "Get Log Rows Count"
+
+
 ROW_COUNT_UPPER_LIMIT = 150000
 LOG_COMPRESSION_CONSTANT = 12
 
 
-def get_log_rows_count(state: State,
-                       data: DataFrame) -> ActionResult[None]:
+def _get_log_rows_count(state: State,
+                        data: DataFrame) -> ActionResult[None]:
     """
     Gets log rows count: log(#rows)/c, where c is a compression constant
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
     log_rows_count = __calculate_log_rows_count(data)
     reward = __calculate_reward(state, log_rows_count)
     state = __update_state(state, log_rows_count)
-    return ActionResult(state, reward, "get_log_rows_count")
+    return state, reward, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_get_log_rows_count,
+                                     model=None,
+                                     raised_exception=False)
 
 
 def __calculate_log_rows_count(data: DataFrame) -> float:
     rows_count = len(data.index)
 
     if rows_count > ROW_COUNT_UPPER_LIMIT:
         return 1
@@ -38,13 +44,16 @@
     return np.log10(rows_count)/LOG_COMPRESSION_CONSTANT
 
 
 def __calculate_reward(state: State, log_rows_count: float) -> float:
     if state.get("log_rows_count") == log_rows_count:
         return -1
 
-    return 1
+    return 0.5
 
 
 def __update_state(state: State, log_rows_count: float) -> State:
     state.set("log_rows_count", log_rows_count)
     return state
+
+
+get_log_rows_count: Action[None] = _get_log_rows_count
```

### Comparing `ostatslib-0.3.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py` & `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 """
 is_response_dichotomous_check module
 """
 
-from copy import deepcopy
 from pandas import DataFrame, Series
 from pandas.api.types import infer_dtype
 import numpy as np
 
-from ostatslib.actions.utils import ActionResult
+from ostatslib.actions import Action, ActionInfo, ActionResult
 from ostatslib.states import State
+from ._get_exploratory_reward import get_exploratory_reward
 
+_ACTION_NAME = "Is Response Dichotomous Check"
 
-def is_response_dichotomous_check(state: State, data: DataFrame) -> ActionResult[str]:
+
+def _is_response_dichotomous_check(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is dichotomous
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
-        ActionResult[str]: action result
+        ActionResult[None]: action result
     """
-    state_copy: State = deepcopy(state)
+    state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
     response: Series = data[response_var_label]
+    state.set("is_response_dichotomous", __get_is_dichotomous_feature_value(response))
+    reward = get_exploratory_reward(state, state_copy)
+    return state, reward, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_is_response_dichotomous_check,
+                                     model=None,
+                                     raised_exception=False)
 
-    is_dichotomous: bool = __is_dichotomous_check(response)
-    if is_dichotomous:
-        state.set("is_response_dichotomous", 1)
-    else:
-        state.set("is_response_dichotomous", -1)
 
-    reward = __calculate_reward(state, state_copy)
-    return ActionResult(state, reward, "is_response_dichotomous_check")
+def __get_is_dichotomous_feature_value(values: Series) -> int:
+    return 1 if __is_dichotomous_check(values) else -1
 
 
 def __is_dichotomous_check(values: Series) -> bool:
     inferred_dtype: str = infer_dtype(values)
     if inferred_dtype == "boolean":
         return True
 
     unique_values = values.unique()
     if len(unique_values) > 2:
         return False
 
     match inferred_dtype:
-        case "categorical" | "string" | "object":
+        case "categorical" | "string" | "object" | "mixed-integer":
             return True
         case "integer":
-            return True if __is_within_possible_boolean_range_of_integers(unique_values) else False
+            return bool(__is_within_possible_boolean_range_of_integers(unique_values))
         case "floating" | "decimal" | "mixed-integer-float":
             first, second = unique_values
-            return True if first.is_integer() and second.is_integer() and \
-                __is_within_possible_boolean_range_of_integers(unique_values) else False
+            return bool(first.is_integer() and second.is_integer() and
+                bool(__is_within_possible_boolean_range_of_integers(unique_values)))
         case _:
             return False
 
 
 def __is_within_possible_boolean_range_of_integers(unique_values):
     return np.any((unique_values >= -1) | (unique_values <= 2))
 
 
-def __calculate_reward(state: State, state_copy: State) -> float:
-    if state == state_copy:
-        return -1
-
-    return 1
+is_response_dichotomous_check: Action[None] = _is_response_dichotomous_check
```

### Comparing `ostatslib-0.3.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py` & `ostatslib-0.4.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 """
 is_response_discrete_check module
 """
 
-from copy import deepcopy
 from pandas import DataFrame, Series
 import numpy as np
 
-from ostatslib.actions.utils import ActionResult
+from ostatslib.actions import Action, ActionInfo, ActionResult
 from ostatslib.states import State
+from ._get_exploratory_reward import get_exploratory_reward
 
+_ACTION_NAME = "Is Response Discrete Check"
 
-def is_response_discrete_check(state: State, data: DataFrame) -> ActionResult[str]:
+
+def _is_response_discrete_check(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is discrete
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
-        ActionResult[str]: action result
+        ActionResult[None]: action result
     """
-    state_copy: State = deepcopy(state)
+    state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
     response: Series = data[response_var_label]
 
     is_discrete: bool = __is_discrete_check(response)
     if is_discrete:
         state.set("is_response_discrete", 1)
     else:
         state.set("is_response_discrete", -1)
 
-    reward = __calculate_reward(state, state_copy)
-    return ActionResult(state, reward, "is_response_discrete_check")
+    reward = get_exploratory_reward(state, state_copy)
+    return state, reward, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_is_response_discrete_check,
+                                     model=None,
+                                     raised_exception=False)
 
 
 def __is_discrete_check(values: Series) -> bool:
     unique_values = values.unique()
 
     is_numeric = np.issubdtype(unique_values.dtype, np.number)
     if not is_numeric:
@@ -48,12 +53,8 @@
             is_whole = float(value).is_integer()
             if not is_whole:
                 return False
 
     return True
 
 
-def __calculate_reward(state: State, state_copy: State) -> float:
-    if state == state_copy:
-        return -1
-
-    return 1
+is_response_discrete_check: Action[None] = _is_response_discrete_check
```

### Comparing `ostatslib-0.3.0/ostatslib/actions/regression_models/poisson_regression.py` & `ostatslib-0.4.0/ostatslib/actions/regression_models/poisson_regression.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,84 @@
 """
 Poisson regression module
 """
 
-import math
 from pandas import DataFrame
 from statsmodels.api import GLM, families
 from statsmodels.genmod.generalized_linear_model import GLMResults
-
-from ostatslib.actions.utils import (ActionResult,
+from statsmodels.tools.sm_exceptions import PerfectSeparationError
+from ostatslib.actions import Action, ActionInfo, ActionResult
+from ostatslib.actions.utils import (calculate_score_reward,
                                      reward_cap,
                                      interpretable_model,
-                                     split_response_from_explanatory_variables)
+                                     split_response_from_explanatory_variables,
+                                     update_state_score)
 from ostatslib.states import State
 
+_ACTION_NAME = "Poisson Regression"
+
 
 @reward_cap
 @interpretable_model
-def poisson_regression(state: State,
-                       data: DataFrame) -> ActionResult[GLMResults]:
+def _poisson_regression(state: State, data: DataFrame) -> ActionResult[GLMResults]:
     """
     Fits data to a poisson regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[GLMResults]: action result
     """
     if not __is_valid_state(state):
-        return ActionResult(state, -1, "PoissonRegression")
+        return state, -1, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_poisson_regression,
+                                     model=None,
+                                     raised_exception=False)
 
     response_var, explanatory_vars = split_response_from_explanatory_variables(state,
                                                                                data)
     try:
         poisson_family = families.Poisson()
         regression: GLMResults = GLM(response_var,
                                      explanatory_vars,
                                      poisson_family).fit()
     except ValueError:
-        return ActionResult(state, -1, "PoissonRegression")
+        return state, -1, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_poisson_regression,
+                                     model=None,
+                                     raised_exception=True)
+    except PerfectSeparationError:
+        state.set('does_poisson_regression_raises_perfect_separation_error', 1)
+        state.set('score', -1)
+        return state, -1, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_poisson_regression,
+                                     model=None,
+                                     raised_exception=True)
 
+    state.set('does_poisson_regression_raises_perfect_separation_error', -1)
     reward = __calculate_reward(regression)
-    state = __apply_state_updates(state, regression)
-    return ActionResult(state, reward, regression)
+    state = update_state_score(state, regression.pseudo_rsquared())
+    return state, reward, ActionInfo(action_name=_ACTION_NAME,
+                                     action_fn=_poisson_regression,
+                                     model=regression,
+                                     raised_exception=False)
 
 
 def __is_valid_state(state: State) -> bool:
     if state.get("is_response_positive_values_only") <= 0:
         return False
 
     if state.get("is_response_discrete") <= 0:
         return False
 
     return True
 
 
 def __calculate_reward(regression: GLMResults) -> float:
     reward: float = 0
-    reward += __reward_for_model_r_squared(regression.pseudo_rsquared())
+    reward += calculate_score_reward(regression.pseudo_rsquared())
     return reward
 
 
-def __reward_for_model_r_squared(rsquared: float) -> float:
-    if math.isnan(rsquared):
-        return -1
-
-    if rsquared <= .6:
-        return - (1 - rsquared)
-
-    return rsquared
-
-
-def __apply_state_updates(state: State, regression: GLMResults) -> State:
-    rsquared = regression.pseudo_rsquared()
-    if math.isnan(rsquared):
-        return state
-
-    state.set('score', regression.pseudo_rsquared())
-    return state
+poisson_regression: Action[GLMResults] = _poisson_regression
```

### Comparing `ostatslib-0.3.0/ostatslib/actions/utils/explainability_rewards.py` & `ostatslib-0.4.0/ostatslib/actions/utils/explainability_rewards.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 """
 explainability rewards decorators module
 """
 
 from functools import wraps
 from typing import TypeVar
 
-from .action_result import ActionFunction, ActionResult
+from pandas import DataFrame
+
+from ostatslib.states import State
+from ostatslib.actions import Action, TModel
 
 T = TypeVar("T")
 
 OPAQUE_PENALTY = -.1
-INTERPETRABLE_REWARD = .1
-COMPREHENSIBLE_REWARD = .1
+INTERPRETABLE_REWARD = .1
+COMPREHENSIBLE_REWARD = .075
 
 
 def opaque_model(
-        action_function: ActionFunction[T]) -> ActionResult[T]:
+        action_function: Action[TModel]) -> Action[TModel]:
     """
     Penalty for actions resulting in an opaque model
 
     Args:
-        action_function (Callable[[State, DataFrame], ActionResult[T]]): action function
+        action_function (Action[TModel]): action
 
     Returns:
-        ActionResult[T]: action results
+        Action[TModel]: action
     """
     wraps(action_function)
 
-    def function_wrapper(*args, **kargs):
-        action_result = action_function(*args, **kargs)
-        action_result.reward += OPAQUE_PENALTY
-        return action_result
+    def function_wrapper(state: State, data: DataFrame):
+        state, reward, info = action_function(state, data)
+        reward += OPAQUE_PENALTY
+        return state, reward, info
 
     return function_wrapper
 
 
 def interpretable_model(
-        action_function: ActionFunction[T]) -> ActionResult[T]:
+        action_function: Action[TModel]) -> Action[TModel]:
     """
-    Reward for actions resulting in an interpetrable model
+    Reward for actions resulting in an interpretable model
 
     Args:
-        action_function (Callable[[State, DataFrame], ActionResult[T]]): action function
+        action_function (Action[TModel]): action
 
     Returns:
-        ActionResult[T]: action results
+        Action[TModel]: action
     """
     wraps(action_function)
 
-    def function_wrapper(*args, **kargs):
-        action_result = action_function(*args, **kargs)
-        action_result.reward += INTERPETRABLE_REWARD
-        return action_result
+    def function_wrapper(state: State, data: DataFrame):
+        state, reward, info = action_function(state, data)
+        reward += INTERPRETABLE_REWARD
+        return state, reward, info
 
     return function_wrapper
 
 
 def comprehensible_model(
-        action_function: ActionFunction[T]) -> ActionResult[T]:
+        action_function: Action[TModel]) -> Action[TModel]:
     """
     Reward for actions resulting in an comprehensible model
 
     Args:
-        action_function (Callable[[State, DataFrame], ActionResult[T]]): action function
+        action_function (Action[TModel]): action
 
     Returns:
-        ActionResult[T]: action results
+        Action[TModel]: action
     """
     wraps(action_function)
 
-    def function_wrapper(*args, **kargs):
-        action_result = action_function(*args, **kargs)
-        action_result.reward += COMPREHENSIBLE_REWARD
-        return action_result
+    def function_wrapper(state: State, data: DataFrame):
+        state, reward, info = action_function(state, data)
+        reward += COMPREHENSIBLE_REWARD
+        return state, reward, info
 
     return function_wrapper
```

### Comparing `ostatslib-0.3.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py` & `ostatslib-0.4.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from pandas import DataFrame, Series
 from ostatslib.states import State
 
 
 def split_response_from_explanatory_variables(state: State,
                                               data: DataFrame) -> tuple[Series, DataFrame]:
-    """Split Dataframe in a response variable values Serie and other potential explanatory variables values in another dataframe without response column
+    """Split Dataframe in a response variable values Serie and 
+    other potential explanatory variables values in another dataframe without response column
 
     Args:
         state (State): state
         data (DataFrame): dataframe
 
     Returns:
         tuple[Series, DataFrame]: response values serie and explanatory variables dataframe
```

### Comparing `ostatslib-0.3.0/ostatslib/states/state_iterator.py` & `ostatslib-0.4.0/ostatslib/states/state_iterator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+#pylint: disable=too-few-public-methods
 """
 State iterator module
 """
 
 
 class StateIterator:
     """
     Iterator for State classes
     """
 
     def __init__(self, state) -> None:
         self.__state = state
-        self.__features_keys_list = state.keys()
+        self.__features_keys_list = state.keys
         self.__index = 0
 
     def __next__(self) -> tuple[str, int | float | bool]:
         if self.__index < len(self.__features_keys_list):
             next_feature_key = self.__features_keys_list[self.__index]
             self.__index += 1
             return (next_feature_key, self.__state.get(next_feature_key))
```

### Comparing `ostatslib-0.3.0/pyproject.toml` & `ostatslib-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [tool.poetry]
 name = "ostatslib"
-version = "0.3.0"
+version = "0.4.0"
 description = "Open Statistical Analysis Agent Library"
 authors = ["Guilherme <g.lisboa.oliveira@outlook.com>"]
 repository = "https://github.com/OStatsAA/ostatslib"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.12"
 numpy = "^1.23.4"
 pandas = "^1.5.0"
 statsmodels = "^0.13.2"
 scipy = "^1.9.3"
 scikit-learn = "^1.1.2"
-tensorflow = "^2.10.1"
+pmdarima = "^2.0.2"
+tabulate = "^0.9.0"
+datacooker = "0.4.0"
+tensorboard = "^2.12.0"
+stable-baselines3 = "2.0.0a5"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.4"
-autopep8 = "^1.7.0"
+autopep8 = ">=1.7,<3.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 scipy = "^1.9.2"
-datacooker = "0.3.0"
 
 
 [tool.poetry.group.docs.dependencies]
-jupyter-book = "^0.13.1"
-sphinxcontrib-mermaid = "^0.7.1"
+jupyter-book = "^0.15.0"
+sphinxcontrib-mermaid = "^0.8.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 relative_files = true
```

### Comparing `ostatslib-0.3.0/PKG-INFO` & `ostatslib-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: ostatslib
-Version: 0.3.0
+Version: 0.4.0
 Summary: Open Statistical Analysis Agent Library
 Home-page: https://github.com/OStatsAA/ostatslib
 License: MIT
 Author: Guilherme
 Author-email: g.lisboa.oliveira@outlook.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: datacooker (==0.4.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pmdarima (>=2.0.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: stable-baselines3 (==2.0.0a5)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
-Requires-Dist: tensorflow (>=2.10.1,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tensorboard (>=2.12.0,<3.0.0)
 Project-URL: Repository, https://github.com/OStatsAA/ostatslib
 Description-Content-Type: text/markdown
 
 # ostatslib
 Open Statistics Library
 
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=OStatsAA_ostatslib&metric=coverage)](https://sonarcloud.io/summary/new_code?id=OStatsAA_ostatslib)
```

