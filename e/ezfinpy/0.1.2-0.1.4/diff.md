# Comparing `tmp/ezfinpy-0.1.2.tar.gz` & `tmp/ezfinpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezfinpy-0.1.2.tar", max compression
+gzip compressed data, was "ezfinpy-0.1.4.tar", max compression
```

## Comparing `ezfinpy-0.1.2.tar` & `ezfinpy-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       29 2023-04-26 22:08:04.122488 ezfinpy-0.1.2/ezfinpy/__init__.py
--rw-r--r--   0        0        0     3431 2023-05-01 00:00:11.815291 ezfinpy-0.1.2/ezfinpy/pandas_patcher.py
--rw-r--r--   0        0        0     5919 2023-05-01 00:01:35.584345 ezfinpy-0.1.2/ezfinpy/simulator.py
--rw-r--r--   0        0        0      668 2023-05-01 00:01:27.977646 ezfinpy-0.1.2/ezfinpy/utils.py
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 ezfinpy-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      567 2023-05-01 00:02:12.027231 ezfinpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 00:20:52.359673 ezfinpy-0.1.2/README.md
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 ezfinpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-05-02 23:42:09.064184 ezfinpy-0.1.4/ezfinpy/__init__.py
+-rw-r--r--   0        0        0     4761 2023-05-02 23:44:13.671012 ezfinpy-0.1.4/ezfinpy/pandas_patcher.py
+-rw-r--r--   0        0        0     4106 2023-05-02 23:45:24.757480 ezfinpy-0.1.4/ezfinpy/simulator.py
+-rw-r--r--   0        0        0      668 2023-05-01 00:01:27.977646 ezfinpy-0.1.4/ezfinpy/utils.py
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 ezfinpy-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      486 2023-05-03 00:08:13.190950 ezfinpy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 00:20:52.359673 ezfinpy-0.1.4/README.md
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 ezfinpy-0.1.4/PKG-INFO
```

### Comparing `ezfinpy-0.1.2/ezfinpy/simulator.py` & `ezfinpy-0.1.4/ezfinpy/simulator.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     if isinstance(weights, str) and weights not in ["ew"]:
         raise ValueError(
             f"""Not a valid string value for weights parameter: {weights}.
                          If it isn't a dict, it has to be 'ew' (equal weight)"""
         )
 
 
-def simulate_without_rebalance(prices, starting_weights: dict | str = "ew") -> SimResult:
+def simulate_without_rebalance(prices: Series | DataFrame, starting_weights: dict | str = "ew") -> SimResult:
     validate_weights(starting_weights)
 
     if starting_weights == "ew":
         values = prices.pct_change().fillna(0).add(1).cumprod()
         sim_result = values.sum(axis=1).pct_change().fillna(0).add(1).cumprod()
 
     if isinstance(starting_weights, dict):
@@ -66,65 +66,15 @@
         result = sim_result,
         all_dates = sim_result.index.to_list(),
         rebal_dates = [],
     )
 
 
 def simulate_with_rebalance(
-    prices: DataFrame,
-    rebal_weights: dict | str = 'ew',
-    rebal_freq: str = "1M",
-) -> SimResult:
-    validate_weights(rebal_weights)
-
-    tickers = prices.columns.to_list()
-    n_tickers = len(prices.columns)
-
-    if rebal_weights == "ew":
-        weights = pd.Series(index=tickers, dtype=np.float64).fillna(1 / n_tickers).to_dict()
-    if isinstance(rebal_weights, dict):
-        weights = rebal_weights.copy()
-
-    returns_array = prices.pct_change().fillna(0).values
-
-    all_dates_array = prices.index.values
-
-    rebal_dates = get_sim_rebal_dates(prices, rebal_freq)
-    rebal_dates_array = np.insert(rebal_dates.values, 0, all_dates_array[0]) # first day
-
-    values = np.zeros((len(all_dates_array), len(tickers)))
-    total_value = []
-    for i, date in enumerate(all_dates_array):
-        for j, ticker in enumerate(tickers):
-            if i == 0:
-                values[i, j] = 1 * weights.get(ticker)
-            else:
-                if all_dates_array[i-1] in rebal_dates_array:
-                    values[i, j] = (total_value[i-1] * weights.get(ticker)) * (1 + returns_array[i, j])
-                else:
-                    values[i, j] = values[i-1, j] * (1 + returns_array[i, j])
-        total_value.append(values[i,:].sum())
-
-    exposure = values / np.array(total_value)[:, np.newaxis]
-
-    values = pd.DataFrame(values, index=all_dates_array, columns=tickers)
-    exposure = pd.DataFrame(exposure, index=all_dates_array, columns=tickers)
-    sim_result = pd.DataFrame(total_value, index=all_dates_array, columns=['sim'])
-
-    return SimResult(
-        prices = prices,
-        values = values,
-        exposure = exposure,
-        result = sim_result,
-        all_dates = prices.index,
-        rebal_dates = rebal_dates,
-    )
-
-def cython_simulate_with_rebalance(
-    prices: DataFrame,
+    prices: Series | DataFrame,
     rebal_weights: dict | str = 'ew',
     rebal_freq: str = "1M",
 ) -> SimResult:
     validate_weights(rebal_weights)
 
     tickers = prices.columns.to_list()
     n_tickers = len(prices.columns)
```

### Comparing `ezfinpy-0.1.2/ezfinpy/utils.py` & `ezfinpy-0.1.4/ezfinpy/utils.py`

 * *Files identical despite different names*

### Comparing `ezfinpy-0.1.2/LICENSE.txt` & `ezfinpy-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

