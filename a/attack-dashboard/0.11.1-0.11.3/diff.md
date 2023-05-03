# Comparing `tmp/attack_dashboard-0.11.1.tar.gz` & `tmp/attack_dashboard-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attack_dashboard-0.11.1.tar", max compression
+gzip compressed data, was "attack_dashboard-0.11.3.tar", max compression
```

## Comparing `attack_dashboard-0.11.1.tar` & `attack_dashboard-0.11.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2766 2023-04-28 18:53:57.860694 attack_dashboard-0.11.1/README.md
--rw-r--r--   0        0        0        0 2023-04-28 16:34:44.467427 attack_dashboard-0.11.1/attack_dashboard/__init__.py
--rw-r--r--   0        0        0      115 2023-04-28 17:57:26.509249 attack_dashboard-0.11.1/attack_dashboard/__main__.py
--rwxr-xr-x   0        0        0     3177 2023-04-30 15:56:22.607112 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/mitre_dashboards.sh
--rw-r--r--   0        0        0     3309 2023-04-30 15:15:19.803918 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson
--rw-r--r--   0        0        0     2837 2023-04-30 15:15:19.803918 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson
--rw-r--r--   0        0        0    16915 2023-04-30 15:15:19.823918 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson
--rw-r--r--   0        0        0      701 2023-04-30 15:15:19.823918 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson
--rw-r--r--   0        0        0      702 2023-04-30 15:15:19.823918 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson
--rw-r--r--   0        0        0      775 2023-04-30 15:15:19.833918 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson
--rw-r--r--   0        0        0     1403 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson
--rw-r--r--   0        0        0     1397 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson
--rw-r--r--   0        0        0     1572 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson
--rw-r--r--   0        0        0     1505 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson
--rw-r--r--   0        0        0     1253 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson
--rw-r--r--   0        0        0     1365 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson
--rw-r--r--   0        0        0     1378 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson
--rw-r--r--   0        0        0     2116 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson
--rw-r--r--   0        0        0     1335 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson
--rw-r--r--   0        0        0     1355 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson
--rw-r--r--   0        0        0     1210 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson
--rw-r--r--   0        0        0     2101 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson
--rw-r--r--   0        0        0     1379 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson
--rw-r--r--   0        0        0     1397 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson
--rw-r--r--   0        0        0     1282 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson
--rw-r--r--   0        0        0     1378 2023-04-30 15:15:19.863917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson
--rw-r--r--   0        0        0     1522 2023-04-30 15:15:19.873917 attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson
--rw-r--r--   0        0        0        0 2023-04-28 16:35:03.959977 attack_dashboard-0.11.1/attack_dashboard/join/__init__.py
--rw-r--r--   0        0        0     6275 2023-04-30 19:37:28.497375 attack_dashboard-0.11.1/attack_dashboard/join/join.py
--rw-r--r--   0        0        0     8694 2023-04-30 19:33:39.793782 attack_dashboard-0.11.1/attack_dashboard/join/join_helpers.py
--rw-r--r--   0        0        0     1567 2023-04-30 19:23:22.624204 attack_dashboard-0.11.1/attack_dashboard/up_dash.py
--rw-r--r--   0        0        0      591 2023-04-30 19:40:08.003480 attack_dashboard-0.11.1/pyproject.toml
--rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 attack_dashboard-0.11.1/PKG-INFO
+-rw-r--r--   0        0        0     2766 2023-04-28 18:53:57.860694 attack_dashboard-0.11.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 16:34:44.467427 attack_dashboard-0.11.3/attack_dashboard/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-28 17:57:26.509249 attack_dashboard-0.11.3/attack_dashboard/__main__.py
+-rwxr-xr-x   0        0        0     3175 2023-05-01 19:48:01.009624 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/mitre_dashboards.sh
+-rw-r--r--   0        0        0     3309 2023-04-30 15:15:19.803918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson
+-rw-r--r--   0        0        0     2837 2023-04-30 15:15:19.803918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson
+-rw-r--r--   0        0        0    16915 2023-04-30 15:15:19.823918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson
+-rw-r--r--   0        0        0      701 2023-04-30 15:15:19.823918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson
+-rw-r--r--   0        0        0      702 2023-04-30 15:15:19.823918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson
+-rw-r--r--   0        0        0      775 2023-04-30 15:15:19.833918 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson
+-rw-r--r--   0        0        0     1403 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson
+-rw-r--r--   0        0        0     1397 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson
+-rw-r--r--   0        0        0     1572 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson
+-rw-r--r--   0        0        0     1505 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson
+-rw-r--r--   0        0        0     1253 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson
+-rw-r--r--   0        0        0     1365 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson
+-rw-r--r--   0        0        0     1378 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson
+-rw-r--r--   0        0        0     2116 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson
+-rw-r--r--   0        0        0     1335 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson
+-rw-r--r--   0        0        0     1355 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson
+-rw-r--r--   0        0        0     1210 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson
+-rw-r--r--   0        0        0     2101 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson
+-rw-r--r--   0        0        0     1379 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson
+-rw-r--r--   0        0        0     1397 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson
+-rw-r--r--   0        0        0     1282 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson
+-rw-r--r--   0        0        0     1378 2023-04-30 15:15:19.863917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson
+-rw-r--r--   0        0        0     1522 2023-04-30 15:15:19.873917 attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson
+-rw-r--r--   0        0        0        0 2023-04-28 16:35:03.959977 attack_dashboard-0.11.3/attack_dashboard/join/__init__.py
+-rw-r--r--   0        0        0     8199 2023-05-03 11:06:59.008344 attack_dashboard-0.11.3/attack_dashboard/join/join.py
+-rw-r--r--   0        0        0     9538 2023-05-03 10:28:50.424295 attack_dashboard-0.11.3/attack_dashboard/join/join_helpers.py
+-rw-r--r--   0        0        0     1567 2023-04-30 19:23:22.624204 attack_dashboard-0.11.3/attack_dashboard/up_dash.py
+-rw-r--r--   0        0        0      725 2023-05-03 11:08:40.841752 attack_dashboard-0.11.3/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 attack_dashboard-0.11.3/PKG-INFO
```

### Comparing `attack_dashboard-0.11.1/README.md` & `attack_dashboard-0.11.3/README.md`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/mitre_dashboards.sh` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/mitre_dashboards.sh`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 echo "$HELK_INFO_TAG Creating Kibana index patterns.."
 for index_pattern in "${index_patterns[@]}"; do
   while true; do
     echo "$HELK_INFO_TAG Creating index pattern ${index_pattern}.."
     ES_STATUS_CODE="$(
-      curl -X POST -s -o /dev/null -w "%{http_code}" -u "${ELASTICSEARCH_CREDS}" "$KIBANA_HOST/api/saved_objects/index-pattern/${index_pattern}?overwrite=true" \
+      curl -X POST -s -r -o /dev/null -w "%{http_code}" -u "${ELASTICSEARCH_CREDS}" "$KIBANA_HOST/api/saved_objects/index-pattern/${index_pattern}?overwrite=true" \
         -H 'Content-Type: application/json' \
         -H 'kbn-xsrf: true' \
         -d"{\"attributes\":{\"title\":\"${index_pattern}\",\"timeFieldName\":\"$TIME_FIELD\"}}"
     )"
     if [ "$ES_STATUS_CODE" -eq 200 ]; then
       break
     else
@@ -63,30 +63,30 @@
 
   response=$(
     curl -sk -XPOST -u "${ELASTICSEARCH_CREDS}" \
       "${KIBANA_HOST}/api/saved_objects/_import?overwrite=true" \
       -H "kbn-xsrf: true" \
       --form file=@"${file}"
   )
-  result=$(echo "${response}" | grep -w "success" | cut -d ',' -f 1 | cut -d ':' -f 2 | sed -E 's/[^-[:alnum:]]//g')
+  result=$(echo "${response}" | grep -w "success" | cut -d ',' -f 2 | cut -d ':' -f 2 | sed -E 's/[^-[:alnum:]]//g')
   if [[ "${result}" == "true" ]]; then
     created=$((created + 1))
     echo "Successfuly imported ${item} named ${file}"
   else
     if [[ $retry -ne 1 ]]; then
       fail="${DIR}/${item}/${file}"
       ARRAY+=($fail)
     else
       failed=$((failed + 1))
     fi
     echo -e "Failed to import ${item} named ${file}: \n ${response}\n"
   fi
 }
 
-echo "Please be patient as we import 100+ custom dashboards, visualizations, and searches..."
+echo "Please be patient as we import custom dashboards, visualizations, and searches..."
 #Go to the right directory to find objects
 cd $DIR
 
 for item in config map canvas-workpad canvas-element lens query index-pattern search visualization dashboard url; do
   cd ${item} 2>/dev/null || continue
 
   for file in *.ndjson; do
```

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/ALL_MITRE_ATTACK__HELK.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/dashboard/MITRE_ATTACK_GROUPS__HELK.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/index-pattern/mitre_attack.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/Global_Discover.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/IOC_Discover.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/search/mitre_attack_discover.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_data_sources_techniques.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_relationship.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_group_select.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_matrices.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_software_cloud.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_tactics.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_groups_techniques_bar.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_mitigation_technique.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_permissions_required.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_select.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_software_groups.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_tactic_techniques.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_technique_data_sources_cloud.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_groups.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson` & `attack_dashboard-0.11.3/attack_dashboard/dashboard_data/objects/visualization/mitre_attack_techniques_matrices.ndjson`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/attack_dashboard/join/join_helpers.py` & `attack_dashboard-0.11.3/attack_dashboard/join/join_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,66 @@
 # import modin.pandas as pd
 # import pandas as pd
 # Check if cuDF is available
 try:
     import cudf as pd
+    import pandas
+
+    is_cuda = True
 except ImportError:
     import pandas as pd
 
+    is_cuda = False
+
 import mitreattack.attackToExcel.attackToExcel as attackToExcel
 from typing import Dict, List
 
 import pickle
 import os
 import argparse
 import logging
 
 
+def cuda_apply(series: pd.Series, func: callable, *args, **kwargs) -> pd.Series:
+    """Apply a function to a series using cuDF if available.
+
+    Args:
+        series (pd.Series): The series to apply the function to.
+        func (callable): The callable function.
+        *args: Variable length argument list.
+        **kwargs: Arbitrary keyword arguments.
+
+    Returns:
+        pd.Series: The series with the function applied.
+    """
+    if is_cuda:
+        # cuDF doesn't support apply yet -> copy the series to a pandas series
+        pd_series = pandas.Series(series)
+        pd_series = pd_series.apply(func, *args, **kwargs)
+        return pd_series
+    else:
+        return series.apply(func, *args, **kwargs)
+
+
 def split_literals_cols(df: pd.DataFrame, cols: List, sep: str = ",") -> pd.DataFrame:
     """Split the given columns from strings into an array of
     strings on the given separator.
 
     Args:
         df (pd.DataFrame): the host dataframe
         cols (List): the columns with strings to split
         sep (str, optional): the separator to split on. Defaults to ",".
 
     Returns:
         pd.DataFrame: the dataframe with the split columns
     """
-    # for col in cols:
-    #     if col in df.columns:
-    #         df[col] = df[col].apply(lambda x: x.split(sep) if isinstance(x, str) else x)
+    lit_splitter = lambda x: x.split(sep) if isinstance(x, str) else x
+    for col in cols:
+        if col in df.columns:
+            df[col] = cuda_apply(df[col], lit_splitter)
     return df
 
 
 def get_args(op_name: str) -> argparse.Namespace:
     """Parse the arguments for the given operation.
 
     Args:
@@ -164,15 +191,15 @@
         )
     len_before = len(df_main)
     df_ret = df_main.merge(
         df_temp,
         on=source_id,
         how="left",
     )
-    logging.info("Rows:\n Before:\t{}\n  After:\t{}\n".format(len_before, len(df_ret)))
+    logging.debug("Rows:\n Before:\t{}\n  After:\t{}\n".format(len_before, len(df_ret)))
     return df_ret
 
 
 def get_join_key(key_text) -> str:
     """
     Returns the standardized column name for the given column name.
     Accounts for inconsistencies in the MITRE data.
@@ -250,15 +277,15 @@
     """
     cols = df.columns
     cols_x = [col for col in cols if col.endswith("_x")]
     cols_y = [col for col in cols if col.endswith("_y")]
     cols_to_merge = list(zip(cols_x, cols_y))
     for col_x, col_y in cols_to_merge:
         col = col_x[:-2]
-        logging.info(
+        logging.debug(
             "Merging x/y column: {}\nNaNs on x:\t\t{}\nNaNs on y:\t\t{}\nOverlapping:\t{}\n".format(
                 col,
                 df[col_x].isna().sum(),
                 df[col_y].isna().sum(),
                 df[df[col_x].isna() & df[col_y].isna()].shape[0],
             )
         )
@@ -271,15 +298,15 @@
         else:
             df[col] = df[col_x].fillna(df[col_y])
             del df[col_x]
             del df[col_y]
     # remove duplicate rows
     len_before = len(df)
     df = df.drop_duplicates()
-    logging.info(
+    logging.debug(
         "Dropped {} duplicate rows".format(len_before - len(df)),
     )
     return df
 
 
 def drop_sub_techniques(
     df: pd.DataFrame, include_sub_techniques: bool = False
@@ -293,10 +320,11 @@
         include_sub_techniques (bool, optional): Whether to actually drop the sub-techniques. Defaults to False.
 
     Returns:
         pd.DataFrame: Filtered dataframe
     """
     if include_sub_techniques:
         return df
-    is_sub = lambda x: str(x).startswith("T") and "." in str(x)
-    df = df[~df["technique_id"].apply(is_sub)]
+    # drop rows which have the field subtechnique_of
+    if "subtechnique_of" in df.columns:
+        df = df[df["subtechnique_of"].isna()]
     return df
```

### Comparing `attack_dashboard-0.11.1/attack_dashboard/up_dash.py` & `attack_dashboard-0.11.3/attack_dashboard/up_dash.py`

 * *Files identical despite different names*

### Comparing `attack_dashboard-0.11.1/PKG-INFO` & `attack_dashboard-0.11.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: attack-dashboard
-Version: 0.11.1
-Summary: 
+Version: 0.11.3
+Summary: Update ATT&CK data for the HELK kibana dashboard.
+Home-page: https://github.com/3lLobo/mitre-dash
+License: MIT
 Author: 3lLobo
 Author-email: flocwolf@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: mitreattack-python (>=2.0.6,<3.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: stix2 (>=3.0.1,<4.0.0)
 Requires-Dist: taxii2-client (>=2.3.0,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Project-URL: Repository, https://github.com/3lLobo/mitre-dash
 Description-Content-Type: text/markdown
 
 # Update Mitre Dashboard
 
 > Goal: Update the Mitre Dashboard from the [HELK](https://github.com/Cyb3rWard0g/HELK) with the latest data.
 
 ### Challenge
```

