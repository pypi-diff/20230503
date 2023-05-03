# Comparing `tmp/pants_py_deploy-0.0.15-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.15rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10661 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 12:58 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4618 b- defN 23-May-03 12:58 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7083 b- defN 23-May-03 12:58 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx      606 b- defN 23-May-03 12:58 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     3534 b- defN 23-May-03 12:58 pants_py_deploy/models.py
--rw-r--r--  2.0 unx     9097 b- defN 23-May-03 12:58 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx      482 b- defN 23-May-03 12:58 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2250 b- defN 23-May-03 12:58 pants_py_deploy-0.0.15.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 12:58 pants_py_deploy-0.0.15.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-03 12:58 pants_py_deploy-0.0.15.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-03 12:58 pants_py_deploy-0.0.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1026 b- defN 23-May-03 12:58 pants_py_deploy-0.0.15.dist-info/RECORD
-12 files, 28805 bytes uncompressed, 8911 bytes compressed:  69.1%
+Zip file size: 10724 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 14:00 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4618 b- defN 23-May-03 14:00 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-May-03 14:00 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx      606 b- defN 23-May-03 14:00 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     3534 b- defN 23-May-03 14:00 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx     9230 b- defN 23-May-03 14:00 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      482 b- defN 23-May-03 14:00 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2253 b- defN 23-May-03 14:00 pants_py_deploy-0.0.15rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 14:00 pants_py_deploy-0.0.15rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-03 14:00 pants_py_deploy-0.0.15rc1.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-03 14:00 pants_py_deploy-0.0.15rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1041 b- defN 23-May-03 14:00 pants_py_deploy-0.0.15rc1.dist-info/RECORD
+12 files, 28956 bytes uncompressed, 8944 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.15.dist-info/METADATA
+Filename: pants_py_deploy-0.0.15rc1.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.15.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.15rc1.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.15.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.15rc1.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.15.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.15rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.15.dist-info/RECORD
+Filename: pants_py_deploy-0.0.15rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pants_py_deploy/plugin.py

```diff
@@ -141,15 +141,14 @@
 async def helm_chart_partition(
     request: HelmChartFileFixer.PartitionRequest,
     new_exported_charts: HelmChartsExported,
 ) -> Partitions:
     managed_chart_files = list(
         file.path for file in chain.from_iterable(new_exported_charts.charts.values())
     )
-
     return Partitions.single_partition(managed_chart_files)
 
 
 @rule
 async def find_env_vars(targets: AllTargets) -> FileEnvVars:
     # don't understand why targets: Targets doesn't work
     sources = await Get(
@@ -253,15 +252,17 @@
     )
 
 
 @rule
 async def fix_helm_charts(
     request: HelmChartFileFixer.Batch, charts: HelmChartsExported
 ) -> FixResult:
-    new_contents = await Get(Snapshot, CreateDigest(charts.full_digest))
+    batch_files = set(request.files)
+    out_files = [file_content for file_content in charts.full_digest if file_content.path in batch_files]
+    new_contents = await Get(Snapshot, CreateDigest(out_files))
     return FixResult(
         input=request.snapshot,
         output=new_contents,
         stderr="",
         stdout="",
         tool_name=HelmChartFileFixer.tool_name,
     )
```

## Comparing `pants_py_deploy-0.0.15.dist-info/METADATA` & `pants_py_deploy-0.0.15rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.15
+Version: 0.0.15rc1
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
```

## Comparing `pants_py_deploy-0.0.15.dist-info/RECORD` & `pants_py_deploy-0.0.15rc1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pants_py_deploy/compose_file.py,sha256=kl6m34S_tdU1SxirGM5FEasPeqqjb_jUndwA2AQBO4c,4618
 pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
 pants_py_deploy/fields.py,sha256=entMoIWLwKiEwOBBr54Mi9CDX6HdqLDdo8RZ-aDIJP4,606
 pants_py_deploy/models.py,sha256=96cqQqW1w3z-tZhthlOyGozL4YwR93H_FVEkipH0qsA,3534
-pants_py_deploy/plugin.py,sha256=zYn7jBYzvBcR2aUKBhdiYa1WbOH5filJ0jvPOKS7Ydg,9097
+pants_py_deploy/plugin.py,sha256=dXZBStXuTYLcYRF7o3jOlCO_Bioh0OuyTo9fUGboFWE,9230
 pants_py_deploy/register.py,sha256=DdsyxfuCEzkruWOItCsoYMpTN75iBkQ1df25Si46KZk,482
-pants_py_deploy-0.0.15.dist-info/METADATA,sha256=qRFdfBCGuZMktL39Hio6oLr0VC32s_v-j_LVzAI83v8,2250
-pants_py_deploy-0.0.15.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.15.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.15.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.15.dist-info/RECORD,,
+pants_py_deploy-0.0.15rc1.dist-info/METADATA,sha256=Jq8CYC3vKIcsLorIh1fsTA73H45qRAE6exIXcD6dKwM,2253
+pants_py_deploy-0.0.15rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.15rc1.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.15rc1.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.15rc1.dist-info/RECORD,,
```

