# Comparing `tmp/woe_scoring-0.8.0.tar.gz` & `tmp/woe_scoring-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woe_scoring-0.8.0.tar", max compression
+gzip compressed data, was "woe_scoring-0.9.0.tar", max compression
```

## Comparing `woe_scoring-0.8.0.tar` & `woe_scoring-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1073 2022-10-19 05:26:04.023549 woe_scoring-0.8.0/LICENSE
--rw-r--r--   0        0        0      533 2023-04-19 09:06:21.886073 woe_scoring-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-19 09:06:21.886220 woe_scoring-0.8.0/woe_scoring/__init__.py
--rw-r--r--   0        0        0       62 2022-10-19 05:26:04.024413 woe_scoring-0.8.0/woe_scoring/core/__init__.py
--rw-r--r--   0        0        0       94 2022-10-19 05:26:04.024664 woe_scoring-0.8.0/woe_scoring/core/binning/__init__.py
--rw-r--r--   0        0        0    21992 2023-04-19 09:06:21.886869 woe_scoring-0.8.0/woe_scoring/core/binning/functions.py
--rw-r--r--   0        0        0    10932 2022-10-19 09:46:50.410755 woe_scoring-0.8.0/woe_scoring/core/main.py
--rw-r--r--   0        0        0      150 2022-10-19 05:26:04.025257 woe_scoring-0.8.0/woe_scoring/core/model/__init__.py
--rw-r--r--   0        0        0    27095 2023-04-19 09:06:21.887225 woe_scoring-0.8.0/woe_scoring/core/model/functions.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 woe_scoring-0.8.0/setup.py
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 woe_scoring-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-10-19 05:26:04.023549 woe_scoring-0.9.0/LICENSE
+-rw-r--r--   0        0        0      533 2023-04-20 12:19:54.559341 woe_scoring-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-20 12:19:54.560248 woe_scoring-0.9.0/woe_scoring/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-20 12:19:54.560363 woe_scoring-0.9.0/woe_scoring/core/__init__.py
+-rw-r--r--   0        0        0      120 2023-04-20 12:19:54.560485 woe_scoring-0.9.0/woe_scoring/core/binning/__init__.py
+-rw-r--r--   0        0        0    21834 2023-04-20 12:19:54.560694 woe_scoring-0.9.0/woe_scoring/core/binning/functions.py
+-rw-r--r--   0        0        0    11596 2023-04-20 12:19:54.561251 woe_scoring-0.9.0/woe_scoring/core/main.py
+-rw-r--r--   0        0        0      162 2023-04-20 12:19:54.561370 woe_scoring-0.9.0/woe_scoring/core/model/__init__.py
+-rw-r--r--   0        0        0    21392 2023-04-20 12:19:54.561550 woe_scoring-0.9.0/woe_scoring/core/model/functions.py
+-rw-r--r--   0        0        0     4929 2023-04-20 12:19:54.561659 woe_scoring-0.9.0/woe_scoring/core/model/selector.py
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 woe_scoring-0.9.0/setup.py
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 woe_scoring-0.9.0/PKG-INFO
```

### Comparing `woe_scoring-0.8.0/LICENSE` & `woe_scoring-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woe_scoring-0.8.0/pyproject.toml` & `woe_scoring-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woe_scoring"
-version = "0.8.0"
+version = "0.9.0"
 description = "Weight Of Evidence Transformer and LogisticRegression model with scikit-learn API"
 authors = ["Stroganov Kirill <kiraplenkin@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = ">=1.19.5"
```

### Comparing `woe_scoring-0.8.0/woe_scoring/core/binning/functions.py` & `woe_scoring-0.9.0/woe_scoring/core/binning/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 import copy
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from scipy.stats import chisquare
 
 
 def _chi2(bad_rates: List[Dict], overall_rate: float) -> float:
     """Calculate the chi-squared statistic for the given bad rates and overall rate.
     Args:
         bad_rates (List[Dict]): List of bad rates.
         overall_rate (float): Overall rate.
     Returns:
         float: Chi-squared statistic."""
 
-    f_obs = [_bin["bad"] for _bin in bad_rates]
-    f_exp = [_bin["total"] * overall_rate for _bin in bad_rates]
-    return chisquare(f_obs=f_obs, f_exp=f_exp)[0]
+    f_obs = np.array([b["bad"] for b in bad_rates])
+    f_exp = np.array([b["total"] * overall_rate for b in bad_rates])
+    return np.sum((f_obs - f_exp) ** 2 / f_exp)
 
 
 def _check_diff_woe(bad_rates: List[Dict], diff_woe_threshold: float) -> Union[None, int]:
     """Check if the difference in woe is greater than the threshold.
     Args:
         bad_rates (List[Dict]): List of bad rates.
         diff_woe_threshold (float): Difference in woe threshold.
     Returns:
         Union[None, int]: Index of the bad rate with the smallest difference in woe."""
-        
-    woe_delta: np.ndarray = np.abs(np.diff([bad_rate["woe"] for bad_rate in bad_rates]))
-    min_diff_woe = min(sorted(list(set(woe_delta))))
-    if min_diff_woe < diff_woe_threshold:
-        return list(woe_delta).index(min_diff_woe)
+
+    woe_values = [bad_rate["woe"] for bad_rate in bad_rates]
+    woe_delta = np.abs(np.diff(woe_values))
+    min_diff_woe_index = np.argmin(woe_delta)
+    if woe_delta[min_diff_woe_index] < diff_woe_threshold:
+        return min_diff_woe_index
     else:
         return None
 
 
 def _mono_flags(bad_rates: List[Dict]) -> bool:
     """Check if the difference in bad rate is monotonic.
     Args:
         bad_rates (List[Dict]): List of bad rates.
     Returns:
         bool: True if the difference in bad rate is monotonic."""
-
-    bad_rate_diffs = np.diff([bad_rate["bad_rate"] for bad_rate in bad_rates])
-    positive_mono_diff = np.all(bad_rate_diffs > 0)
-    negative_mono_diff = np.all(bad_rate_diffs < 0)
-    return True in [positive_mono_diff, negative_mono_diff]
+    prev_bad_rate = bad_rates[0]["bad_rate"]
+    
+    increasing, decreasing = False, False
+    for i in range(1, len(bad_rates)):
+        curr_bad_rate = bad_rates[i]["bad_rate"]
+        if curr_bad_rate < prev_bad_rate:
+            increasing = False
+        elif curr_bad_rate > prev_bad_rate:
+            decreasing = False
+        prev_bad_rate = curr_bad_rate
+        if not (increasing or decreasing):
+            return False
+    return True
 
 
 def _find_index_of_diff_flag(bad_rates: List[Dict]) -> int:
     """Find the index of the bad rate with the smallest difference in woe.
     Args:
         bad_rates (List[Dict]): List of bad rates.
     Returns:
         int: Index of the bad rate with the smallest difference in woe."""
 
     bad_rate_diffs = np.diff([bad_rate["bad_rate"] for bad_rate in bad_rates])
-    return list(bad_rate_diffs > 0).index(
-        pd.Series(bad_rate_diffs > 0).value_counts().sort_values().index.tolist()[0]
-    )
+    return np.argmin(bad_rate_diffs)
 
 
 def _merge_bins_chi(x, y: np.ndarray, bad_rates: List[Dict], bins: List) -> List[Dict]:
     """Merge the bins with the chi-squared statistic.
     Args:
         x (pd.DataFrame): Input data.
         y (np.ndarray): Output data.
@@ -73,39 +79,38 @@
 
     idx = _find_index_of_diff_flag(bad_rates)
     if idx == 0:
         del bins[1]
     elif idx == len(bad_rates) - 2:
         del bins[len(bins) - 2]
     else:
-        _extracted_from__merge_bins_chi_8(bins, idx, x, y)
-    bad_rates, _ = _bin_bad_rate(x, y, bins)
+        _extract_bin_by_chi2(bins, idx, x, y)
+    bad_rates, _ = _bin_bad_rates(x, y, bins)
     return bad_rates, bins
 
 
-# TODO Rename this here and in `_merge_bins_chi`
-def _extracted_from__merge_bins_chi_8(bins, idx, x, y) -> None:
+def _extract_bin_by_chi2(bins, idx, x, y) -> None:
     """Extract the bins with the chi-squared statistic.
     Args:
         bins (List[Dict]): List of bins.
         idx (int): Index of the bad rate with the smallest difference in woe.
         x (pd.DataFrame): Input data.
         y (np.ndarray): Output data.
     Returns:
         None."""
 
     temp_bins = copy.deepcopy(bins)
     del temp_bins[idx + 1]
-    temp_bad_rates, temp_overall_rate = _bin_bad_rate(x, y, temp_bins)
+    temp_bad_rates, temp_overall_rate = _bin_bad_rates(x, y, temp_bins)
     chi_1 = _chi2(temp_bad_rates, temp_overall_rate)
     del temp_bins
 
     temp_bins = copy.deepcopy(bins)
     del temp_bins[idx + 2]
-    temp_bad_rates, temp_overall_rate = _bin_bad_rate(x, y, temp_bins)
+    temp_bad_rates, temp_overall_rate = _bin_bad_rates(x, y, temp_bins)
     chi_2 = _chi2(temp_bad_rates, temp_overall_rate)
     if chi_1 < chi_2:
         del bins[idx + 1]
     else:
         del bins[idx + 2]
 
 
@@ -121,85 +126,77 @@
 
     idx = _find_index_of_diff_flag(bad_rates)
     if idx == 0:
         del bins[1]
     elif idx == len(bad_rates) - 2:
         del bins[len(bins) - 2]
     else:
-        _extracted_from__merge_bins_iv_8(bins, idx, x, y)
-    bad_rates, _ = _bin_bad_rate(x, y, bins)
+        _extract_bin_by_iv(bins, idx, x, y)
+    bad_rates, _ = _bin_bad_rates(x, y, bins)
     return bad_rates, bins
 
 
-# TODO Rename this here and in `_merge_bins_iv`
-def _extracted_from__merge_bins_iv_8(bins, idx, x, y) -> None:
+def _extract_bin_by_iv(bins, idx, x, y) -> None:
     """Extract the bins with the IV statistic.
     Args:
         bins (List[Dict]): List of bins.
         idx (int): Index of the bad rate with the smallest difference in woe.
         x (pd.DataFrame): Input data.
         y (np.ndarray): Output data.
     Returns:
         None."""
 
     temp_bins = copy.deepcopy(bins)
     del temp_bins[idx + 1]
-    temp_bad_rates, _ = _bin_bad_rate(x, y, temp_bins)
+    temp_bad_rates, _ = _bin_bad_rates(x, y, temp_bins)
     iv_1 = sum(_bin["iv"] for _bin in temp_bad_rates)
     del temp_bins
 
     temp_bins = copy.deepcopy(bins)
     del temp_bins[idx + 2]
-    temp_bad_rates, _ = _bin_bad_rate(x, y, temp_bins)
+    temp_bad_rates, _ = _bin_bad_rates(x, y, temp_bins)
     iv_2 = sum(_bin["iv"] for _bin in temp_bad_rates)
     if iv_1 > iv_2:
         del bins[idx + 1]
     else:
         del bins[idx + 2]
 
 
 def _merge_bins_min_pct(
-        x, y: np.ndarray, bad_rates: List[Dict], bins: List, cat: bool = False
-) -> List[Dict]:
+    x, y: np.ndarray, bad_rates: Tuple[Dict], bins: List, cat: bool = False
+) -> Tuple[List[Dict], List]:
     """Merge the bins with the minimum percentage.
     Args:
         x (pd.DataFrame): Input data.
         y (np.ndarray): Output data.
-        bad_rates (List[Dict]): List of bad rates.
+        bad_rates (Tuple[Dict]): Tuple of bad rates.
         bins (List): List of bins.
         cat (bool, optional): If True, the bins are merged into a categorical bin. Defaults to False.
     Returns:
-        List[Dict]: List of bad rates."""
+        Tuple[List[Dict], List]: Tuple of bad rates and bins.
+    """
 
-    idx = [bad_rates[i]["pct"] for i in range(len(bad_rates))].index(
-        min(bad_rate["pct"] for bad_rate in bad_rates)
-    )
+    idx = [br["pct"] for br in bad_rates].index(min(br["pct"] for br in bad_rates))
 
     if cat:
         if idx == 0:
             bins[idx + 1] += bins[idx]
-        elif idx == len(bad_rates) - 1:
-            bins[idx - 1] += bins[idx]
-        elif bad_rates[idx - 1]["pct"] < bad_rates[idx + 1]["pct"]:
+        elif idx == len(bad_rates) - 1 or bad_rates[idx - 1]["pct"] < bad_rates[idx + 1]["pct"]:
             bins[idx - 1] += bins[idx]
         else:
             bins[idx + 1] += bins[idx]
-        del bins[idx]
+        bins = bins[:idx] + bins[idx+1:]
     elif idx == 0:
-        del bins[1]
+        bins = bins[1:]
     elif idx == len(bad_rates) - 1:
-        del bins[len(bins) - 2]
-    elif bad_rates[idx - 1]["pct"] < bad_rates[idx + 1]["pct"]:
-        del bins[idx]
+        bins = bins[:-1]
     else:
-        del bins[idx + 1]
+        bins = bins[:idx] + bins[idx+1:]
 
-    bad_rates, _ = _bin_bad_rate(x, y, bins, cat=cat)
-    if cat:
-        bins = [bad_rate["bin"] for bad_rate in bad_rates]
+    bad_rates, _ = _bin_bad_rates(x, y, bins, cat=cat)
     return bad_rates, bins
 
 
 def _calc_stats(
         x, y: np.ndarray, idx, all_bad, all_good: int, bins: List, cat: bool = False, refit_fl: bool = False
 ) -> Dict:
     """Calculate the statistics.
@@ -218,19 +215,17 @@
     if refit_fl:
         value = bins[idx]
     else:
         value = bins[idx] if cat else [bins[idx], bins[idx + 1]]
     x_not_na = x[~pd.isna(x)]
     y_not_na = y[~pd.isna(x)]
     if cat:
-        x_in = x_not_na[pd.Series(x_not_na).isin(value)]
+        x_in = x_not_na[np.isin(x_not_na, value)]
     else:
-        x_in = x_not_na[
-            np.where((x_not_na >= np.min(value)) & (x_not_na < np.max(value)))
-        ]
+        x_in = x_not_na[[i for i in range(len(x_not_na)) if x_not_na[i] >= np.min(value) and x_not_na[i] < np.max(value)]]
     total = len(x_in)
     bad = y_not_na[np.isin(x_not_na, x_in)].sum()
     pct = np.sum(np.isin(x_not_na, x_in)) / len(x)
     bad_rate = bad / total if total != 0 else 0
     good = total - bad
     woe = np.log((good / all_good) / (bad / all_bad)) if good != 0 and bad != 0 else np.log(
         ((good + 0.5) / all_good) / ((bad + 0.5) / all_bad)
@@ -243,15 +238,16 @@
         "pct": pct,
         "bad_rate": bad_rate,
         "woe": woe,
         "iv": iv,
     }
 
 
-def _bin_bad_rate(
+# @jit(nopython=True)
+def _bin_bad_rates(
         x: np.ndarray, y: np.ndarray, bins: List, cat: bool = False, refit_fl: bool = False
 ) -> Tuple[List[Dict], np.ndarray]:
     """Bin the bad rates.
     Args:
         x (pd.DataFrame): Input data.
         y (np.ndarray): Output data.
         bins (List): List of bins.
@@ -271,57 +267,63 @@
         bad = sum(bad_rate["bad"] for bad_rate in bad_rates)
         total = sum(bad_rate["total"] for bad_rate in bad_rates)
         overall_rate = bad / total
     return bad_rates, overall_rate
 
 
 def _calc_max_bins(bins, max_bins: float) -> int:
-    """Calculate the maximum number of bins.
+    """
+    Calculate the maximum number of bins.
+
     Args:
         bins (List): List of bins.
         max_bins (float): Maximum number of bins.
+
     Returns:
-        int: Maximum number of bins."""
+        int: Maximum number of bins.
+    """
+    return max(2, min(int(len(bins) * max_bins), int(max_bins)))
 
-    return max(int(len(bins) * max_bins), 2)
 
+def prepare_data(data: pd.DataFrame, special_cols: List[str] = None) -> Tuple[pd.DataFrame, List[str]]:
+    """
+    Prepare the data.
 
-def prepare_data(x: Union[pd.DataFrame, np.ndarray], special_cols: List[str] = None) -> Tuple[pd.DataFrame, List[str]]:
-    """Prepare the data.
     Args:
-        x (Union[pd.DataFrame, np.ndarray]): Input data.
+        data (pd.DataFrame): Input data.
         special_cols (List[str], optional): List of special columns. Defaults to None.
+
     Returns:
-        Tuple[pd.DataFrame, List[str]]: Prepared data."""
+        Tuple[pd.DataFrame, List[str]]: Prepared data.
+    """
 
-    if not isinstance(x, pd.DataFrame):
+    if not isinstance(data, pd.DataFrame):
         raise TypeError("data should be pandas data frame")
     if special_cols:
-        x = x.drop(special_cols, axis=1)
-    feature_names = x.columns
-    return x, feature_names
+        data = data.drop(special_cols, axis=1)
+    feature_names = data.columns
+    return data, feature_names
 
 
 def find_cat_features(x: pd.DataFrame, feature_names: List[str], cat_features_threshold: int) -> List[str]:
     """Find the categorical features.
     Args:
         x (pd.DataFrame): Input data.
         feature_names (List[str]): List of feature names.
         cat_features_threshold (int): Threshold of categorical features.
     Returns:
         List[str]: List of categorical features."""
 
-    return [
-        feature_names[i] for i in range(len(feature_names)) if (
-                type(x[0, i]) == np.dtype("object")
-                or type(x[0, i]) == np.dtype("str")
-                or len(np.unique(x[:, i])) < cat_features_threshold
-        )
+    is_categorical = np.array([
+        np.issubdtype(x.dtypes[i], np.object_) or np.issubdtype(x.dtypes[i], np.floating)
+        or len(np.unique(x.iloc[:, i].values.astype(str))) < cat_features_threshold
+        for i in range(len(feature_names))
+    ])
 
-    ]
+    return list(np.array(feature_names)[is_categorical])
 
 
 def _cat_binning(
         x, y: np.ndarray,
         min_pct_group: float,
         max_bins: Union[int, float],
         diff_woe_threshold: float,
@@ -382,29 +384,29 @@
                         new_bins[i] += [list(bad_rates_dict.keys())[n]]
                         start += 1
                     except IndexError:
                         new_bins.append([])
                         new_bins[i] += [list(bad_rates_dict.keys())[n]]
                         start += 1
 
-        bad_rates, _ = _bin_bad_rate(x, y, new_bins, cat=True)
+        bad_rates, _ = _bin_bad_rates(x, y, new_bins, cat=True)
         bins = [bad_rate["bin"] for bad_rate in bad_rates]
     else:
-        bad_rates, _ = _bin_bad_rate(x, y, bins, cat=True)
+        bad_rates, _ = _bin_bad_rates(x, y, bins, cat=True)
 
     if len(y[pd.isna(x)]) > 0:
         if len(bins) < 2:
             bins.append([])
             if data_type == "object":
                 bins[1] += ["Missing"]
                 x[pd.isna(x)] = "Missing"
             else:
                 bins[1] += [-1]
                 x[pd.isna(x)] = -1
-            bad_rates, _ = _bin_bad_rate(x, y, bins, cat=True)
+            bad_rates, _ = _bin_bad_rates(x, y, bins, cat=True)
             missing_bin = "first" if bad_rates[0]["bin"][0] in ["Missing", -1] else "last"
         else:
             na_bad_rate = y[pd.isna(x)].sum() / len(y[pd.isna(x)])
             if abs(na_bad_rate - bad_rates[0]["bad_rate"]) < abs(
                     na_bad_rate - bad_rates[len(bad_rates) - 1]["bad_rate"]
             ):
                 missing_bin = "first"
@@ -418,27 +420,27 @@
                 missing_bin = "last"
                 if data_type == "object":
                     bad_rates[-1]["bin"] += ["Missing"]
                     x[pd.isna(x)] = "Missing"
                 else:
                     bad_rates[-1]["bin"] += [-1]
                     x[pd.isna(x)] = -1
-            bad_rates, _ = _bin_bad_rate(x, y, bins, cat=True)
+            bad_rates, _ = _bin_bad_rates(x, y, bins, cat=True)
             bins = [bad_rate["bin"] for bad_rate in bad_rates]
 
     if len(bins) <= 2:
         return bad_rates, missing_bin
 
     while (_check_diff_woe(bad_rates, diff_woe_threshold) is not None) and (
             len(bad_rates) > 2
     ):
         idx = _check_diff_woe(bad_rates, diff_woe_threshold)
         bins[idx + 1] += bins[idx]
         del bins[idx]
-        bad_rates, _ = _bin_bad_rate(x, y, bins, cat=True)
+        bad_rates, _ = _bin_bad_rates(x, y, bins, cat=True)
         bins = [bad_rate["bin"] for bad_rate in bad_rates]
 
     if len(bins) <= 2:
         return bad_rates, missing_bin
 
     while (
             min(bad_rate["pct"] for bad_rate in bad_rates) <= min_pct_group
@@ -517,19 +519,19 @@
         bins = list(np.unique(bins))
         if len(bins) == 2:
             bins.append(np.unique(x[~pd.isna(x)])[1])
     else:
         bins.extend(iter(sorted(np.unique(x[~pd.isna(x)]))))
     bins.append(np.inf)
 
-    bad_rates, _ = _bin_bad_rate(x, y, bins)
+    bad_rates, _ = _bin_bad_rates(x, y, bins)
 
     if (pd.isna(bad_rates[0]["bad_rate"])) and (len(bad_rates) > 2):
         del bins[1]
-        bad_rates, _ = _bin_bad_rate(x, y, bins)
+        bad_rates, _ = _bin_bad_rates(x, y, bins)
 
     if len(y[pd.isna(x)]) > 0:
         na_bad_rate = y[pd.isna(x)].sum() / len(y[pd.isna(x)])
         if len(bad_rates) == 2:
             if na_bad_rate < bad_rates[1]["bad_rate"]:
                 x = np.nan_to_num(x, nan=np.amin(x[~pd.isna(x)]) - 1)
                 bins = [np.NINF, np.amin(x[~pd.isna(x)])] + bins[1:]
@@ -550,15 +552,15 @@
             )
         ):
             x = np.nan_to_num(x, nan=np.amin(x[~pd.isna(x)]))
             missing_bin = "first"
         else:
             x = np.nan_to_num(x, nan=np.amax(x[~pd.isna(x)]))
             missing_bin = "last"
-        bad_rates, _ = _bin_bad_rate(x, y, bins)
+        bad_rates, _ = _bin_bad_rates(x, y, bins)
 
     if len(bad_rates) <= 2:
         return bad_rates, missing_bin
 
     while (_mono_flags(bad_rates) is False) and (len(bad_rates) > 2):
         if merge_type == 'chi2':
             bad_rates, bins = _merge_bins_chi(x, y, bad_rates, bins)
@@ -580,15 +582,15 @@
         return bad_rates, missing_bin
 
     while (_check_diff_woe(bad_rates, diff_woe_threshold) is not None) and (
             len(bad_rates) > 2
     ):
         idx = _check_diff_woe(bad_rates, diff_woe_threshold) + 1
         del bins[idx]
-        bad_rates, _ = _bin_bad_rate(x, y, bins)
+        bad_rates, _ = _bin_bad_rates(x, y, bins)
 
     return bad_rates, missing_bin
 
 
 def num_processing(
         x: pd.Series,
         y: Union[np.ndarray, pd.Series],
@@ -628,44 +630,44 @@
         x: feature
         y: target
         bins: bins
         type_feature: type of feature
         missing_bin: missing bin
     Returns:
         Dict: binning result"""
-        
+
     cat = type_feature == "cat"
     if cat:
-        try:
-            x = x.astype(float)
-            x[pd.isna(x)] = -1
-        except ValueError:
-            x = x.astype(str)
-            x[pd.isna(x)] = "Missing"
+        na_value = -1.0 if np.issubdtype(x.dtype, np.floating) else "Missing"
+        x[np.isnan(x)] = na_value
     elif missing_bin == "first":
-        x = np.nan_to_num(x, nan=np.amin(x[~pd.isna(x)]) - 1)
+        na_value = np.nanmin(x[~np.isnan(x)]) - 1
+        x[np.isnan(x)] = na_value
     elif missing_bin == "last":
-        x = np.nan_to_num(x, nan=np.amax(x[~pd.isna(x)]) + 1)
-    bad_rates, _ = _bin_bad_rate(x, y, bins, cat=cat, refit_fl=True)
+        na_value = np.nanmax(x[~np.isnan(x)]) + 1
+        x[np.isnan(x)] = na_value
+    bad_rates, _ = _bin_bad_rates(x, y, bins, cat=cat, refit_fl=True)
     return bad_rates
 
 
 def refit(
         x, y: np.ndarray,
         bins: List,
         type_feature: str,
         missing_bin: str
 ) -> Dict:
     """Refit woe dict.
+
     Args:
         x: feature
         y: target
         bins: bins
         type_feature: type of feature
         missing_bin: missing bin
+
     Returns:
         Dict: binning result"""
         
     res_dict = _refit_woe_dict(
         x.values, y, bins, type_feature, missing_bin
     )
     return {
```

### Comparing `woe_scoring-0.8.0/woe_scoring/core/main.py` & `woe_scoring-0.9.0/woe_scoring/core/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,48 +3,66 @@
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.multiclass import unique_labels
 
-from .binning.functions import cat_processing, find_cat_features, num_processing, prepare_data, refit
-from .model.functions import create_model, generate_sql, iv_feature_select, predict_proba, save_reports, \
-    save_scorecard_fn, \
-    sequential_feature_select
+from .binning.functions import (cat_processing, find_cat_features,
+                                num_processing, prepare_data, refit)
+from .model.functions import (_check_correlation_threshold, create_model,
+                              generate_sql, predict_proba, save_reports,
+                              save_scorecard_fn)
+from .model.selector import FeatureSelector
 
 
 class NpEncoder(json.JSONEncoder):
+    """Convert NumPy objects to JSON serializable ones."""
+
     def default(self, obj):
+        """Convert a non-serializable object to a serializable one.
+
+        If `obj` is an instance of `np.integer`, this function returns it as a
+        Python integer. If `obj` is an instance of `np.floating`, this function
+        returns it as a Python float. If `obj` is an instance of `np.ndarray`,
+        this function returns its contents as a nested list. Otherwise, this
+        function delegates the conversion to the parent class.
+
+        Args:
+            obj: An object to be converted to a serializable one.
+
+        Returns:
+            A serializable version of `obj`.
+        """
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
             return float(obj)
         elif isinstance(obj, np.ndarray):
             return obj.tolist()
         else:
-            return super(NpEncoder, self).default(obj)
+            return super().default(obj)
 
 
 class WOETransformer(BaseEstimator, TransformerMixin):
     def __init__(
             self,
             max_bins: Union[int, float] = 10,
             min_pct_group: float = 0.05,
             n_jobs: int = 1,
             prefix: str = "WOE_",
             merge_type: str = "chi2",
-            cat_features: List = None,
-            special_cols: List = None,
+            cat_features: List[str] = None,
+            special_cols: List[str] = None,
             cat_features_threshold: int = 0,
             diff_woe_threshold: float = 0.05,
             safe_original_data: bool = False,
     ):
         """
-        Performs the Weight Of Evidence transformation over the input x features using information from y vector.
+        Initializes the class with the given hyperparameters.
         """
         self.classes_ = None
         self.max_bins = max_bins
         self.min_pct_group = min_pct_group
         self.cat_features = cat_features or []
         self.special_cols = special_cols or []
         self.cat_features_threshold = cat_features_threshold
@@ -54,148 +72,162 @@
         self.safe_original_data = safe_original_data
         self.merge_type = merge_type
 
         self.woe_iv_dict = []
         self.feature_names = []
         self.num_features = []
 
-    def fit(self, x: pd.DataFrame, y: Union[pd.Series, np.ndarray]):
+    def fit(self, data: pd.DataFrame, target: Union[pd.Series, np.ndarray]) -> None:
         """
         Fits the input data
-        :param x: data matrix
-        :param y: target vector
+        :param data: data matrix
+        :param target: target vector
+        :return: None
         """
-        x, self.feature_names = prepare_data(x=x, special_cols=self.special_cols)
-        self.classes_ = unique_labels(y)
+        data, self.feature_names = prepare_data(data=data, special_cols=self.special_cols)
+        self.classes_ = unique_labels(target)
 
         if len(self.cat_features) == 0 and self.cat_features_threshold > 0:
             self.cat_features = find_cat_features(
-                x=x,
+                data=data,
                 feature_names=self.feature_names,
                 cat_features_threshold=self.cat_features_threshold
             )
+
         if len(self.cat_features) > 0:
             self.num_features = [
                 feature
                 for feature in self.feature_names
                 if feature not in self.cat_features
             ]
             self.woe_iv_dict = Parallel(n_jobs=self.n_jobs)(
                 delayed(cat_processing)(
-                    x[col],
-                    y,
+                    data[col],
+                    target,
                     self.min_pct_group,
                     self.max_bins,
                     self.diff_woe_threshold
                 ) for col in self.cat_features
             )
         else:
             self.num_features = self.feature_names
 
         num_features_res = Parallel(n_jobs=self.n_jobs)(
             delayed(num_processing)(
-                x[col],
-                y,
+                data[col],
+                target,
                 self.min_pct_group,
                 self.max_bins,
                 self.diff_woe_threshold,
                 self.merge_type
             ) for col in self.num_features
         )
 
         self.woe_iv_dict += num_features_res
 
-    def transform(self, x: pd.DataFrame):
+
+    def transform(self, data: pd.DataFrame) -> pd.DataFrame:
         """
-        Transforms input arrays
-        :param x: x data array
+        Transforms input data
+        :param data: input data frame
         :return: transformed data
         """
-        x = x.copy()
-        for i, _ in enumerate(self.woe_iv_dict):
-            feature = list(self.woe_iv_dict[i])[0]
+        data = data.copy()
+        for i, woe_iv in enumerate(self.woe_iv_dict):
+            feature = list(woe_iv)[0]
+            woe_iv_feature = woe_iv[feature]
             new_feature = self.prefix + feature
-            for bin_values in self.woe_iv_dict[i][feature]:
+            for bin_values in woe_iv_feature:
                 if feature in self.cat_features:
-                    x.loc[
-                        np.isin(x[feature], bin_values["bin"]), new_feature
+                    data.loc[
+                        np.isin(data[feature], bin_values["bin"]), new_feature
                     ] = bin_values["woe"]
                 else:
-                    x.loc[
+                    data.loc[
                         np.logical_and(
-                            x[feature] >= np.min(bin_values["bin"]),
-                            x[feature] < np.max(bin_values["bin"]),
+                            data[feature] >= np.min(bin_values["bin"]),
+                            data[feature] < np.max(bin_values["bin"]),
                         ),
                         new_feature,
                     ] = bin_values["woe"]
-            if self.woe_iv_dict[i]["missing_bin"] == "first":
-                x[new_feature].fillna(
-                    self.woe_iv_dict[i][feature][0]["woe"], inplace=True
-                )
-            elif self.woe_iv_dict[i]["missing_bin"] == "last":
-                x[new_feature].fillna(
-                    self.woe_iv_dict[i][feature][-1]["woe"], inplace=True
-                )
-            elif (
-                    self.woe_iv_dict[i][feature][0]["woe"]
-                    < self.woe_iv_dict[i][feature][-1]["woe"]
-            ):
-                x[new_feature].fillna(
-                    self.woe_iv_dict[i][feature][0]["woe"], inplace=True
-                )
+            missing_bin = woe_iv["missing_bin"]
+            if missing_bin == "first":
+                data[new_feature].fillna(woe_iv_feature[0]["woe"], inplace=True)
+            elif missing_bin == "last":
+                data[new_feature].fillna(woe_iv_feature[-1]["woe"], inplace=True)
+            elif woe_iv_feature[0]["woe"] < woe_iv_feature[-1]["woe"]:
+                data[new_feature].fillna(woe_iv_feature[0]["woe"], inplace=True)
             else:
-                x[new_feature].fillna(
-                    self.woe_iv_dict[i][feature][-1]["woe"], inplace=True
-                )
+                data[new_feature].fillna(woe_iv_feature[-1]["woe"], inplace=True)
             if not self.safe_original_data:
-                del x[feature]
+                del data[feature]
+        return data
+
+
+
+    def save_to_file(self, file_path: str) -> None:
+        """
+        Save the woe_iv_dict to a JSON file at the specified file path.
+
+        Args:
+            file_path (str): The path where the file should be saved.
+
+        Returns:
+            None
+        """
+        with open(file_path, "w") as f:
+            json.dump(self.woe_iv_dict, f, indent=4, cls=NpEncoder)
 
-        return x
 
-    def save(self, path: str) -> None:
-        with open(path, "w") as file:
-            json.dump(self.woe_iv_dict, file, indent=4, cls=NpEncoder)
+    def load_woe_iv_dict(self, file_path: str) -> None:
+        """
+        Load a dictionary of WoE and IV values from a JSON file.
+
+        Args:
+            file_path (str): The path to the JSON file.
+
+        Returns:
+            None
+        """
+        with open(file_path, "r") as json_file:
+            self.woe_iv_dict = json.load(json_file)
 
-    def load(self, path: str) -> None:
-        with open(path, "r") as file:
-            self.woe_iv_dict = json.load(file)
 
     def refit(self, x: pd.DataFrame, y: Union[pd.Series, np.ndarray]) -> None:
         x, self.feature_names = prepare_data(x=x, special_cols=self.special_cols)
-        self.woe_iv_dict = Parallel(n_jobs=self.n_jobs)(
+        self.woe_iv_dict = Parallel(n_jobs=self.n_jobs, backend='multiprocessing')(
             delayed(refit)(
                 x[list(self.woe_iv_dict[i].keys())[0]],
                 y.values,
                 [_bin["bin"] for _bin in self.woe_iv_dict[i][list(self.woe_iv_dict[i].keys())[0]]],
                 self.woe_iv_dict[i]["type_feature"],
                 self.woe_iv_dict[i]["missing_bin"]
             ) for i in range(len(self.woe_iv_dict))
         )
 
 
 class CreateModel(BaseEstimator, TransformerMixin):
     def __init__(
-            self,
-            selection_method: str = 'iv',
-            max_vars: Union[int, float, None] = None,
-            special_cols: List = None,
-            unused_cols: List = None,
-            n_jobs: int = 1,
-            gini_threshold: float = 5.0,
-            iv_threshold: float = 0.05,
-            corr_threshold: float = 0.5,
-            min_pct_group: float = 0.05,
-            random_state: int = None,
-            class_weight: str = None,
-            direction: str = "forward",
-            cv: int = 3,
-            C: float = None,
-            scoring: str = "roc_auc",
+        self,
+        selection_method: str = 'rfe', # 'rfe' or 'sfe'
+        max_vars: Union[int, float, None] = None,
+        special_cols: List[str] = None,
+        unused_cols: List[str] = None,
+        n_jobs: int = 1,
+        gini_threshold: float = 5.0,
+        iv_threshold: float = 0.05,
+        corr_threshold: float = 0.5,
+        min_pct_group: float = 0.05,
+        random_state: int = None,
+        class_weight: str = None,
+        direction: str = "forward",
+        cv: int = 3,
+        C: float = None,
+        scoring: str = "roc_auc",
     ):
-
         self.model_results = None
         self.selection_method = selection_method
         self.max_vars = max_vars
         self.special_cols = special_cols or []
         self.unused_cols = unused_cols or []
         self.n_jobs = n_jobs
         self.gini_threshold = gini_threshold
@@ -206,64 +238,59 @@
         self.class_weight = class_weight
         self.direction = direction
         self.cv = cv
         self.C = C
         self.scoring = scoring
 
         self.feature_names_: List[str] = []
-        self.coef_: List[float] = []
-        self.intercept_: float = 0.0
+        self.coef: List[float] = []
+        self.intercept: float = 0.0
         self.model = None
 
     def fit(self, x: pd.DataFrame, y: Union[pd.Series, np.ndarray]):
-        x, self.feature_names_ = prepare_data(x, special_cols=self.special_cols)
+        x, self.feature_names_ = prepare_data(data=x, special_cols=self.special_cols)
 
         if self.unused_cols:
             self.feature_names_ = [feature for feature in self.feature_names_ if feature not in self.unused_cols]
-
+        
         if self.C is None:
             self.C = 1.0e4 / x.shape[0]
 
         if self.max_vars is not None and self.max_vars < 1:
             self.max_vars = int(len(self.feature_names_) * self.max_vars)
 
-        if self.selection_method == 'iv':
-            self.feature_names_ = iv_feature_select(
-                x, y,
-                feature_names=self.feature_names_,
-                iv_threshold=self.iv_threshold,
-                max_vars=self.max_vars,
-                n_jobs=self.n_jobs,
-                random_state=self.random_state,
-                cv=self.cv,
-                scoring=self.scoring,
-                c=self.C,
-                class_weight=self.class_weight,
-                corr_threshold=self.corr_threshold,
-                min_pct_group=self.min_pct_group,
-            )
-        elif self.selection_method == 'sequential':
-            self.feature_names_ = sequential_feature_select(
-                x, y,
-                feature_names=self.feature_names_,
-                gini_threshold=self.gini_threshold,
-                corr_threshold=self.corr_threshold,
-                min_pct_group=self.min_pct_group,
-                random_state=self.random_state,
-                class_weight=self.class_weight,
-                max_vars=self.max_vars,
-                direction=self.direction,
-                cv=self.cv,
-                c=self.C,
-                scoring=self.scoring,
-                n_jobs=self.n_jobs,
-            )
-        else:
-            raise NameError("selection_method should be 'iv' or 'sequential'")
-
+        selector = FeatureSelector(
+            selection_type=self.selection_method,
+            max_vars=self.max_vars,
+            n_jobs=self.n_jobs,
+            random_state=self.random_state,
+            class_weight=self.class_weight,
+            direction=self.direction,
+            cv=self.cv,
+            C=self.C,
+            scoring=self.scoring,
+            gini_threshold=self.gini_threshold,
+            min_pct_group=self.min_pct_group,
+        )
+        self.feature_names_ = selector.select(x, y, self.feature_names_)
+        
+        if len(self.feature_names_) == 0:
+            raise ValueError("No features selected")
+        
+        self.feature_names_ = _check_correlation_threshold(
+            x, y,
+            self.feature_names_,
+            self.corr_threshold,
+            self.random_state,
+            self.class_weight,
+            self.cv,
+            self.C,
+            self.scoring,
+            self.n_jobs
+        )
         self.model = create_model(
             x, y,
             feature_names=self.feature_names_
         )
 
         self.model_results = pd.read_html(self.model.summary().tables[1].as_html(), header=0, index_col=0)[
             0].reset_index()
```

### Comparing `woe_scoring-0.8.0/woe_scoring/core/model/functions.py` & `woe_scoring-0.9.0/woe_scoring/core/model/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
-from itertools import product
-from operator import itemgetter
-from typing import Dict, List, Union
+from typing import List, Union
 
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 from joblib import Parallel, delayed
-from sklearn.feature_selection import SequentialFeatureSelector
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import cross_val_score
 
 
 def _calc_score(
         x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
@@ -36,14 +33,17 @@
         n_jobs: Number of jobs.
     Returns:
         Score of the feature."""
 
     model = LogisticRegression(
         random_state=random_state,
         class_weight=class_weight,
+        solver='saga',
+        max_iter=1000,
+        warm_start=True,
         n_jobs=n_jobs,
         C=c,
     )
     scores = cross_val_score(
         model,
         x[var].values.reshape(-1, 1),
         y,
@@ -109,306 +109,101 @@
         class_weight: str,
         cv: int,
         c: float,
         scoring: str,
         n_jobs: int
 ) -> List[str]:
     """Check if a feature has a correlation score below a threshold.
+
     Args:
         x: DataFrame or numpy array.
         y: Series or numpy array.
         feature_names: List of features.
         corr_threshold: Correlation threshold.
         random_state: Random state.
         class_weight: Class weight.
         cv: Number of folds.
         c: Regularization parameter.
         scoring: Scoring method.
         n_jobs: Number of jobs.
+
     Returns:
-        List of features with a correlation score below a threshold."""
+        List of features with a correlation score below a threshold.
+    """
+
+    if isinstance(x, np.ndarray):
+        x = pd.DataFrame(x, columns=feature_names)
 
-    iterator = product(feature_names, feature_names)
     correlation = x[feature_names].corr()
-    for var_a, var_b in iterator:
-        if (var_a != var_b) and (var_a in feature_names) and (var_b in feature_names) and abs(
-                correlation[var_a][var_b]
-        ) >= corr_threshold:
-            if _calc_score(
-                    x,
-                    y,
-                    var_a,
-                    random_state,
-                    class_weight,
-                    cv,
-                    c,
-                    scoring,
-                    n_jobs,
-            ) > _calc_score(
-                x,
-                y,
-                var_b,
-                random_state,
-                class_weight,
-                cv,
-                c,
-                scoring,
-                n_jobs,
-            ):
-                feature_names.remove(var_b)
+    mask = np.tril(np.ones_like(correlation, dtype=bool), k=-1)
+    correlation = correlation.where(mask)
+    correlation = correlation.stack().reset_index()
+    correlation.columns = ['feature_a', 'feature_b', 'correlation']
+    correlation = correlation.query(f"correlation.abs() >= {corr_threshold}")
+    features_to_remove = []
+
+    for feature in feature_names:
+        if feature in features_to_remove:
+            continue
+        correlated_features = correlation.query(f"feature_a == '{feature}' or feature_b == '{feature}'")
+        if len(correlated_features) == 0:
+            continue
+        scores = []
+        for _, row in correlated_features.iterrows():
+            if row['feature_a'] == feature:
+                other_feature = row['feature_b']
             else:
-                feature_names.remove(var_a)
-    return feature_names
+                other_feature = row['feature_a']
+            score = _calc_score(x, y, other_feature, random_state, class_weight, cv, c, scoring, n_jobs)
+            scores.append(score)
+        if all(score <= scores[0] for score in scores):
+            features_to_remove.append(feature)
+
+    return [f for f in feature_names if f not in features_to_remove]
 
 
 def _check_min_pct_group(
-        x: Union[pd.DataFrame, np.ndarray],
-        feature_names: List[str],
-        min_pct_group: float,
+    x: Union[pd.DataFrame, np.ndarray],
+    feature_names: List[str],
+    min_pct_group: float,
 ) -> List[str]:
     """Check if a feature has a minimum percentage of values below a threshold.
     Args:
         x: DataFrame or numpy array.
         feature_names: List of features.
         min_pct_group: Minimum percentage of values below a threshold.
     Returns:
         List of features with a minimum percentage of values below a threshold."""
-
+    
     to_drop = [
         feature_name for feature_name in feature_names if
         x[feature_name].value_counts(normalize=True).min() < min_pct_group
     ]
     return [var for var in feature_names if var not in to_drop]
 
 
-def _feature_selector(
-        x: Union[pd.DataFrame, np.ndarray],
-        y: Union[pd.Series, np.ndarray],
-        feature_names: List[str],
-        random_state: int,
-        class_weight: str,
-        cv: int,
-        c: float,
-        n_jobs: int,
-        max_vars: Union[int, float],
-        direction: str,
-        scoring: str,
-) -> List[str]:
-    """Feature selector.
-    Args:
-        x: DataFrame or numpy array.
-        y: Series or numpy array.
-        feature_names: List of features.
-        random_state: Random state.
-        class_weight: Class weight.
-        cv: Number of folds.
-        c: Regularization parameter.
-        n_jobs: Number of jobs.
-        max_vars: Maximum number of features.
-        direction: Direction of selection.
-        scoring: Scoring method.
-    Returns:
-        List of features."""
-
-    sfs = SequentialFeatureSelector(
-        LogisticRegression(
-            random_state=random_state,
-            class_weight=class_weight,
-            n_jobs=n_jobs,
-            C=c,
-        ),
-        n_features_to_select=max_vars,
-        direction=direction,
-        cv=cv,
-        n_jobs=n_jobs,
-        scoring=scoring,
-    )
-    sfs.fit(x[feature_names], y)
-    return list(np.array(feature_names)[list(sfs.get_support())])
-
-
-def sequential_feature_select(
-        x: pd.DataFrame,
-        y: Union[pd.Series, np.ndarray],
-        feature_names: List[str],
-        gini_threshold: float,
-        corr_threshold: float,
-        min_pct_group: float,
-        random_state: int,
-        class_weight: str,
-        max_vars: Union[int, float],
-        direction: str,
-        cv: int,
-        c: float,
-        scoring: str,
-        n_jobs: int,
-) -> List[str]:
-    """Sequential feature selector.
-    Args:
-        x: DataFrame or numpy array.
-        y: Series or numpy array.
-        feature_names: List of features.
-        gini_threshold: Gini threshold.
-        corr_threshold: Correlation threshold.
-        min_pct_group: Minimum percentage of values below a threshold.
-        random_state: Random state.
-        class_weight: Class weight.
-        cv: Number of folds.
-        c: Regularization parameter.
-        scoring: Scoring method.
-        n_jobs: Number of jobs.
-    Returns:
-        List of features."""
-
-    feature_names = _check_min_pct_group(
-        x,
-        feature_names=feature_names,
-        min_pct_group=min_pct_group,
-    )
-
-    feature_names = _check_features_gini_threshold(
-        x, y,
-        feature_names=feature_names,
-        gini_threshold=gini_threshold,
-        random_state=random_state,
-        class_weight=class_weight,
-        cv=cv,
-        c=c,
-        scoring=scoring,
-        n_jobs=n_jobs
-    )
-
-    feature_names = _feature_selector(
-        x, y,
-        feature_names=feature_names,
-        random_state=random_state,
-        class_weight=class_weight,
-        cv=cv,
-        c=c,
-        n_jobs=n_jobs,
-        max_vars=max_vars,
-        direction=direction,
-        scoring=scoring,
-    )
-
-    feature_names = _check_correlation_threshold(
-        x, y,
-        feature_names=feature_names,
-        corr_threshold=corr_threshold,
-        random_state=random_state,
-        class_weight=class_weight,
-        cv=cv,
-        c=c,
-        scoring=scoring,
-        n_jobs=n_jobs
-    )
-    return feature_names
-
-
-def _calc_iv_dict(x: pd.DataFrame, y: np.ndarray, feature: str) -> Dict:
-    """Calculate IV for a feature.
-    Args:
-        x: DataFrame or numpy array.
-        y: Series or numpy array.
-        feature: Feature name.
-    Returns:
-        Dictionary with feature name as key and IV as value."""
-
-    _iv = 0
-    for value in x[feature].sort_values().unique():
-        bad = y[x[feature] == value].sum()
-        good = len(y[x[feature] == value]) - bad
-        all_bad = y.sum()
-        all_good = len(y) - all_bad
-        _iv += ((good / all_good) - (bad / all_bad)) * value
-    return {feature: _iv}
-
-
-def iv_feature_select(
-        x: pd.DataFrame,
-        y: Union[pd.Series, np.ndarray],
-        feature_names: List[str],
-        iv_threshold: float,
-        max_vars: int,
-        n_jobs: int,
-        corr_threshold: float,
-        min_pct_group: float,
-        random_state: int,
-        class_weight: str,
-        cv: int,
-        c: float,
-        scoring: str,
-) -> List[str]:
-    """Information value feature selector.
-    Args:
-        x: DataFrame or numpy array.
-        y: Series or numpy array.
-        feature_names: List of features.
-        iv_threshold: Information value threshold.
-        max_vars: Maximum number of features.
-        n_jobs: Number of jobs.
-        corr_threshold: Correlation threshold.
-        min_pct_group: Minimum percentage of values below a threshold.
-        random_state: Random state.
-        class_weight: Class weight.
-        cv: Number of folds.
-        c: Regularization parameter.
-        scoring: Scoring method.
-    Returns:
-        List of features."""
-
-    temp_res_dict = Parallel(n_jobs=n_jobs)(
-        delayed(_calc_iv_dict)(x, y, feature) for feature in feature_names
-    )
-    res_dict = {}
-    for d in temp_res_dict:
-        res_dict |= d
-
-    feature_names = [feature for feature in dict(sorted(res_dict.items(), key=itemgetter(1), reverse=True)) if
-                     res_dict[feature] >= iv_threshold][:max_vars]
-
-    feature_names = _check_min_pct_group(
-        x,
-        feature_names=feature_names,
-        min_pct_group=min_pct_group,
-    )
-
-    feature_names = _check_correlation_threshold(
-        x, y,
-        feature_names=feature_names,
-        corr_threshold=corr_threshold,
-        random_state=random_state,
-        class_weight=class_weight,
-        cv=cv,
-        c=c,
-        scoring=scoring,
-        n_jobs=n_jobs
-    )
-    return feature_names
-
-
-def _check_pvalue_and_sign(model: sm.Logit) -> List[int]:
-    """Check p-value.
-    Args:
-        model: Model.
-    Returns:
-        List of variables with p-values > 0.05 or positive sign."""
-
-    # return [
-    #     model.wald_test_terms().table.index[i]
-    #     for i, pvalue in enumerate(model.wald_test_terms().table["pvalue"])
-    #     if pvalue > 0.05
-    # ]
-
-    return [
-        model.summary().tables[1].data[i][0]
-        for i in range(2, len(model.summary().tables[1].data))
-        if float(model.summary().tables[1].data[i][1]) > 0
-        or float(model.summary().tables[1].data[i][4]) > 0.05
-    ]
+def _get_high_pval_positive_vars(X: pd.DataFrame, y: Union[pd.Series, np.ndarray], feature_names: List[str]) -> List[str]:
+        """
+        Returns variables with high p-values and positive sign.
+
+        Args:
+            X: DataFrame.
+            y: Series or numpy array.
+            feature_names: List of features.
+
+        Returns:
+            List of variables with high p-values and positive sign.
+        """
+        model = sm.Logit(y, sm.add_constant(X[feature_names])).fit()
+        summary_table = model.summary().tables[1].data
+        return [
+            row[0]
+            for row in summary_table[2:]
+            if float(row[1]) > 0 or float(row[4]) > 0.05
+        ]
 
 
 def create_model(
         x: Union[pd.DataFrame, np.ndarray],
         y: Union[pd.Series, np.ndarray],
         feature_names: List[str],
 ) -> sm.Logit:
@@ -416,23 +211,15 @@
     Args:
         x: DataFrame or numpy array.
         y: Series or numpy array.
         feature_names: List of features.
     Returns:
         Model."""
 
-    model = sm.Logit(y, sm.add_constant(x[feature_names])).fit()
-
-    to_drop = _check_pvalue_and_sign(model)
-    while len(to_drop) > 0:
-        feature_names = [feature for feature in feature_names if feature not in to_drop]
-        model = sm.Logit(y, sm.add_constant(x[feature_names])).fit()
-        to_drop = _check_pvalue_and_sign(model)
-
-    return model
+    return sm.Logit(y, sm.add_constant(x[feature_names])).fit()
 
 
 def save_reports(
         model: sm.Logit,
         path: str = os.getcwd()
 ) -> None:
     """Save model reports.
@@ -551,83 +338,88 @@
     Returns:
         Score points."""
 
     return -(woe * coef + intercept / n_features) * factor + offset / n_features
 
 
 def _calc_stats_for_feature(
-        idx,
-        feature,
-        feature_names: List[str],
-        encoder,
-        model_results,
-        factor: float,
-        offset: float,
+    idx,
+    feature,
+    feature_names: List[str],
+    encoder,
+    model_results,
+    factor: float,
+    offset: float,
 ) -> pd.DataFrame:
     """Calculate stats for feature.
     Args:
         idx: Index.
         feature: Feature.
         feature_names: Feature names.
         encoder: Encoder.
         model_results: Model results.
         factor: Factor.
         offset: Offset.
     Returns:
-        Stats for feature."""
-
+        Stats for feature.
+    """
     result_dict = {
         "feature": [],
         "coef": [],
         "pvalue": [],
         "bin": [],
         "WOE": [],
         "IV": [],
         "percent_of_population": [],
         "total": [],
         "event_cnt": [],
         "non_event_cnt": [],
         "event_rate": [],
         "score_ball": [],
     }
+
+    woe_iv_dict = encoder.woe_iv_dict
+    intercept = model_results.iloc[0, 1]
+    n_features = len(feature_names)
+
     if idx < 1:
-        _update_result_dict(
-            result_dict, feature, model_results, idx
-        )
+        _update_result_dict(result_dict, feature, model_results, idx)
         for key, value in result_dict.items():
             if key not in ["feature", "coef", "pvalue"]:
                 value.append("-")
     else:
-        for i, _ in enumerate(encoder.woe_iv_dict):
-            if list(encoder.woe_iv_dict[i])[0] == feature.replace("WOE_", ""):
-                for _bin in encoder.woe_iv_dict[i][feature.replace("WOE_", "")]:
-                    _update_result_dict(
-                        result_dict, feature, model_results, idx
-                    )
-                    result_dict["bin"].append(
-                        [val if val != -1 else str(val).replace("-1", "missing") for val in _bin["bin"]]
-                    )
-                    result_dict["WOE"].append(_bin["woe"])
-                    result_dict["IV"].append(_bin["iv"])
-                    result_dict["percent_of_population"].append(_bin["pct"])
-                    result_dict["total"].append(_bin["total"])
-                    result_dict["event_cnt"].append(_bin["bad"])
-                    result_dict["non_event_cnt"].append(result_dict["total"][-1] - result_dict["event_cnt"][-1])
-                    result_dict["event_rate"].append(_bin["bad_rate"])
+        for woe_iv in woe_iv_dict:
+            if list(woe_iv.keys())[0] == feature.replace("WOE_", ""):
+                feature_woe_iv = woe_iv[feature.replace("WOE_", "")]
+                for bin_info in feature_woe_iv:
+                    _update_result_dict(result_dict, feature, model_results, idx)
+                    bin_values = bin_info["bin"]
+                    bin_values_str = [
+                        str(val).replace("-1", "missing") if val == -1 else val
+                        for val in bin_values
+                    ]
+                    result_dict["bin"].append(bin_values_str)
+                    result_dict["WOE"].append(bin_info["woe"])
+                    result_dict["IV"].append(bin_info["iv"])
+                    result_dict["percent_of_population"].append(bin_info["pct"])
+                    result_dict["total"].append(bin_info["total"])
+                    result_dict["event_cnt"].append(bin_info["bad"])
+                    result_dict["non_event_cnt"].append(bin_info["good"])
+                    result_dict["event_rate"].append(bin_info["bad_rate"])
                     result_dict["score_ball"].append(
                         _calc_score_points(
                             woe=result_dict["WOE"][-1],
                             coef=result_dict["coef"][-1],
-                            intercept=model_results.iloc[0, 1],
+                            intercept=intercept,
                             factor=factor,
                             offset=offset,
-                            n_features=len(feature_names),
-
+                            n_features=n_features,
                         )
                     )
+
     return pd.DataFrame.from_dict(result_dict)
 
 
 def _update_result_dict(result_dict, feature, model_results, idx) -> None:
     """Update result dict.
     Args:
         result_dict: Result dict.
@@ -655,28 +447,20 @@
         encoder: Encoder.
         model_results: Model results.
         factor: Factor.
         offset: Offset.
     Returns:
         Stats."""
 
-    feature_stats = []
-    for idx, feature in enumerate(model_results.iloc[:, 0]):
-        res_df = _calc_stats_for_feature(
-            idx,
-            feature,
-            feature_names,
-            encoder,
-            model_results,
-            factor,
-            offset
-        )
-        res_df.name = feature.replace("WOE_", "")
-        feature_stats.append(res_df)
-    return feature_stats
+    return Parallel(n_jobs=-1, backend="multiprocessing")(
+        delayed(_calc_stats_for_feature)(
+            idx, feature, feature_names, encoder, model_results, factor, offset
+        ).rename(feature.replace("WOE_", ""))
+        for idx, feature in enumerate(model_results.iloc[:, 0])
+    )
 
 
 def _build_excel_sheet_with_charts(
         feature_stats: list[pd.DataFrame],
         writer: pd.ExcelWriter,
         width: int = 640,
         height: int = 480,
```

### Comparing `woe_scoring-0.8.0/setup.py` & `woe_scoring-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pandas>=1.2.2',
  'scikit-learn>=0.24.1',
  'scipy>=1.6.1',
  'statsmodels>=0.12.2']
 
 setup_kwargs = {
     'name': 'woe-scoring',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Weight Of Evidence Transformer and LogisticRegression model with scikit-learn API',
     'long_description': 'None',
     'author': 'Stroganov Kirill',
     'author_email': 'kiraplenkin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `woe_scoring-0.8.0/PKG-INFO` & `woe_scoring-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woe-scoring
-Version: 0.8.0
+Version: 0.9.0
 Summary: Weight Of Evidence Transformer and LogisticRegression model with scikit-learn API
 License: MIT
 Author: Stroganov Kirill
 Author-email: kiraplenkin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

