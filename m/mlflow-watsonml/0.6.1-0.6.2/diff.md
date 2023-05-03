# Comparing `tmp/mlflow-watsonml-0.6.1.tar.gz` & `tmp/mlflow-watsonml-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-watsonml-0.6.1.tar", last modified: Tue May  2 19:31:19 2023, max compression
+gzip compressed data, was "mlflow-watsonml-0.6.2.tar", last modified: Wed May  3 12:17:38 2023, max compression
```

## Comparing `mlflow-watsonml-0.6.1.tar` & `mlflow-watsonml-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/mlflow_watsonml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/mlflow_watsonml/wml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 19:31:19.000000 mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:31:19.355198 mlflow-watsonml-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 19:31:08.000000 mlflow-watsonml-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/mlflow_watsonml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/mlflow_watsonml/wml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 12:17:38.000000 mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:17:38.684838 mlflow-watsonml-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 12:17:25.000000 mlflow-watsonml-0.6.2/setup.py
```

### Comparing `mlflow-watsonml-0.6.1/PKG-INFO` & `mlflow-watsonml-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.1
+Version: 0.6.2
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.6.1/README.md` & `mlflow-watsonml-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.1/mlflow_watsonml/config.py` & `mlflow-watsonml-0.6.2/mlflow_watsonml/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.1/mlflow_watsonml/deploy.py` & `mlflow-watsonml-0.6.2/mlflow_watsonml/deploy.py`

 * *Files identical despite different names*

### Comparing `mlflow-watsonml-0.6.1/mlflow_watsonml/utils.py` & `mlflow-watsonml-0.6.2/mlflow_watsonml/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -273,7 +273,12 @@
         )
 
 
 def software_spec_exists(client: APIClient, sw_spec: str) -> bool:
     sw_specs = list_software_specs(client=client)
 
     return any(item for item in sw_specs if item["metadata"]["name"] == sw_spec)
+
+
+def delete_sw_spec(client, name):
+    sw_spec_id = client.software_specifications.get_id_by_name(name)
+    client.software_specifications.delete(sw_spec_id)
```

### Comparing `mlflow-watsonml-0.6.1/mlflow_watsonml/wml.py` & `mlflow-watsonml-0.6.2/mlflow_watsonml/wml.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,47 +180,60 @@
 
 
 def create_custom_software_spec(
     client: APIClient,
     name: str,
     base_sofware_spec: str,
     custom_packages: List[Dict[str, str]],
+    rewrite: bool = False,
 ):
     if software_spec_exists(client=client, sw_spec=name):
-        raise MlflowException(
-            f"""Software spec {name} already exists. 
-            Please delete the software spec or create one with another name."""
+        if rewrite:
+            delete_sw_spec(client=client, name=name)
+        else:
+            raise MlflowException(
+                f"""Software spec {name} already exists. 
+                Please delete the software spec or create one with another name."""
+            )
+
+    try:
+        base_software_spec_id = client.software_specifications.get_id_by_name(
+            base_sofware_spec
         )
 
-    base_software_spec_id = client.software_specifications.get_id_by_name(
-        base_sofware_spec
-    )
-
-    meta_prop_sw_spec = {
-        client.software_specifications.ConfigurationMetaNames.NAME: name,
-        client.software_specifications.ConfigurationMetaNames.BASE_SOFTWARE_SPECIFICATION: {
-            "guid": base_software_spec_id
-        },
-    }
-
-    sw_spec_details = client.software_specifications.store(meta_props=meta_prop_sw_spec)
-    software_spec_id = client.software_specifications.get_uid(sw_spec_details)
-
-    for custom_package in custom_packages:
-        meta_prop_pkg_extn = {
-            client.package_extensions.ConfigurationMetaNames.NAME: custom_package[
-                "name"
-            ],
-            client.package_extensions.ConfigurationMetaNames.TYPE: "pip_zip",
+        meta_prop_sw_spec = {
+            client.software_specifications.ConfigurationMetaNames.NAME: name,
+            client.software_specifications.ConfigurationMetaNames.BASE_SOFTWARE_SPECIFICATION: {
+                "guid": base_software_spec_id
+            },
         }
 
-        pkg_extn_details = client.package_extensions.store(
-            meta_props=meta_prop_pkg_extn, file_path=custom_package["file"]
+        sw_spec_details = client.software_specifications.store(
+            meta_props=meta_prop_sw_spec
         )
+        software_spec_id = client.software_specifications.get_uid(sw_spec_details)
 
-        pkg_extn_id = client.package_extensions.get_id(pkg_extn_details)
+        for custom_package in custom_packages:
+            meta_prop_pkg_extn = {
+                client.package_extensions.ConfigurationMetaNames.NAME: custom_package[
+                    "name"
+                ],
+                client.package_extensions.ConfigurationMetaNames.TYPE: "pip_zip",
+            }
+
+            pkg_extn_details = client.package_extensions.store(
+                meta_props=meta_prop_pkg_extn, file_path=custom_package["file"]
+            )
+
+            pkg_extn_id = client.package_extensions.get_id(pkg_extn_details)
+
+            client.software_specifications.add_package_extension(
+                software_spec_id, pkg_extn_id
+            )
+
+    except Exception as e:
+        if software_spec_exists(client=client, sw_spec=name):
+            delete_sw_spec(client, name)
 
-        client.software_specifications.add_package_extension(
-            software_spec_id, pkg_extn_id
-        )
+        raise MlflowException(e)
 
     return software_spec_id
```

### Comparing `mlflow-watsonml-0.6.1/mlflow_watsonml.egg-info/PKG-INFO` & `mlflow-watsonml-0.6.2/mlflow_watsonml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-watsonml
-Version: 0.6.1
+Version: 0.6.2
 Summary: WatsonML MLflow deployment plugin
 Home-page: https://github.com/IBM/mlflow-watsonml
 Author: IBM AI Model Factory team
 Author-email: dhruv.shah@ibm.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mlflow-watsonml-0.6.1/setup.py` & `mlflow-watsonml-0.6.2/setup.py`

 * *Files identical despite different names*

