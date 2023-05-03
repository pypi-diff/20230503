# Comparing `tmp/compose_chart_export-0.0.14-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.15-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 12706 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 07:58 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 23-May-03 07:58 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    12399 b- defN 23-May-03 07:58 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-03 07:58 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-03 07:58 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     8781 b- defN 23-May-03 07:58 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-03 07:58 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-03 07:58 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      583 b- defN 23-May-03 07:58 compose_chart_export-0.0.14.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 07:58 compose_chart_export-0.0.14.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 07:58 compose_chart_export-0.0.14.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-03 07:58 compose_chart_export-0.0.14.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-May-03 07:58 compose_chart_export-0.0.14.dist-info/RECORD
-13 files, 35262 bytes uncompressed, 10650 bytes compressed:  69.8%
+Zip file size: 12708 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 12:56 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 23-May-03 12:56 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    12399 b- defN 23-May-03 12:56 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-May-03 12:56 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-03 12:56 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     8779 b- defN 23-May-03 12:56 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-May-03 12:56 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-03 12:56 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      583 b- defN 23-May-03 12:56 compose_chart_export-0.0.15.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 12:56 compose_chart_export-0.0.15.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-03 12:56 compose_chart_export-0.0.15.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-03 12:56 compose_chart_export-0.0.15.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-May-03 12:56 compose_chart_export-0.0.15.dist-info/RECORD
+13 files, 35260 bytes uncompressed, 10652 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.14.dist-info/METADATA
+Filename: compose_chart_export-0.0.15.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.14.dist-info/WHEEL
+Filename: compose_chart_export-0.0.15.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.14.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.15.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.14.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.15.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.14.dist-info/RECORD
+Filename: compose_chart_export-0.0.15.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/compose_export.py

```diff
@@ -134,15 +134,15 @@
     chart_version = ensure_chart_version_valid(chart_version)
     compose_path = Path(compose_path)
     service_name, extra_containers = parse_service_name_extra_containers(compose_path)
     info = read_compose_info(compose_path, service_name)
     env = info.default_env
     compose_labels = info.labels
     prefix_ports = parse_container_ports(compose_labels, info.host_container_ports)
-    container_name = service_name.replace("_", "-")
+    container_name = chart_name.replace("_", "-")
     with TemporaryDirectory() as path:
         chart_path = Path(path) / chart_name
         if existing_chart := parse_existing_chart(compose_labels):
             existing_chart = (compose_path.parent / existing_chart).resolve()
             assert (
                 existing_chart.exists()
             ), f"existing chart not found @ {existing_chart}"
```

## Comparing `compose_chart_export-0.0.14.dist-info/METADATA` & `compose_chart_export-0.0.15.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.14
+Version: 0.0.15
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.14)
-Requires-Dist: model-lib (==0.0.14)
+Requires-Dist: docker-compose-parser (==0.0.15)
+Requires-Dist: model-lib (==0.0.15)
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: semver (==2.13.0)
-Requires-Dist: zero-3rdparty (==0.0.14)
+Requires-Dist: zero-3rdparty (==0.0.15)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

