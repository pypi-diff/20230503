# Comparing `tmp/eo_grow-1.5.0.tar.gz` & `tmp/eo_grow-1.5.1.tar.gz`

## Comparing `eo_grow-1.5.0.tar` & `eo_grow-1.5.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/__init__.py
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/py.typed
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/types.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/base.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/config.py
--rw-r--r--   0        0        0    16771 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/logging.py
--rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/pipeline.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/schemas.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/storage.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/__init__.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/base.py
--rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/batch.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/custom_grid.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/core/area/utm.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/__init__.py
--rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/batch_to_eopatch.py
--rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/byoc.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/download.py
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/download_batch.py
--rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/export_maps.py
--rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/features.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/import_tiff.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/import_vector.py
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/merge_samples.py
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/prediction.py
--rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/rasterize.py
--rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/sampling.py
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/split_grid.py
--rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/testing.py
--rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/training.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/pipelines/zipmap.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/__init__.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/batch_to_eopatch.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/common.py
--rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/features.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/prediction.py
--rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/spatial.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/tasks/testing.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/batch.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/eopatch_list.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/filter.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/fs.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/general.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/grid.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/logging.py
--rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/map.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/meta.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/ray.py
--rw-r--r--   0        0        0    16448 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/testing.py
--rw-r--r--   0        0        0    10294 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/validators.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/vector.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 eo_grow-1.5.0/eogrow/utils/zipmap.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eo_grow-1.5.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 eo_grow-1.5.0/LICENSE
--rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 eo_grow-1.5.0/README.md
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 eo_grow-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    10156 2020-02-02 00:00:00.000000 eo_grow-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/__init__.py
+-rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/py.typed
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/types.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/__init__.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/base.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/config.py
+-rw-r--r--   0        0        0    16786 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/logging.py
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/pipeline.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/schemas.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/storage.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/area/__init__.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/area/base.py
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/area/batch.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/area/custom_grid.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/core/area/utm.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/__init__.py
+-rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/batch_to_eopatch.py
+-rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/byoc.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/download.py
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/download_batch.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/export_maps.py
+-rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/features.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/import_tiff.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/import_vector.py
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/merge_samples.py
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/prediction.py
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/rasterize.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/sampling.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/split_grid.py
+-rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/testing.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/training.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/pipelines/zipmap.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/__init__.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/batch_to_eopatch.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/common.py
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/features.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/prediction.py
+-rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/spatial.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/tasks/testing.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/batch.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/eopatch_list.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/filter.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/fs.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/general.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/grid.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/logging.py
+-rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/map.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/meta.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/ray.py
+-rw-r--r--   0        0        0    16448 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/testing.py
+-rw-r--r--   0        0        0    10294 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/validators.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/vector.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 eo_grow-1.5.1/eogrow/utils/zipmap.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 eo_grow-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 eo_grow-1.5.1/LICENSE
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 eo_grow-1.5.1/README.md
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 eo_grow-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10156 2020-02-02 00:00:00.000000 eo_grow-1.5.1/PKG-INFO
```

### Comparing `eo_grow-1.5.0/eogrow/cli.py` & `eo_grow-1.5.1/eogrow/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 )
 
 
 @click.command()
 @click.argument("config_path", type=click.Path())
 @variables_option
 @test_patches_option
-def run_pipeline(config_path: str, cli_variables: Tuple[str], test_patches: Tuple[int]) -> None:
+def run_pipeline(config_path: str, cli_variables: Tuple[str, ...], test_patches: Tuple[int, ...]) -> None:
     """Execute eo-grow pipeline using CLI.
 
     \b
     Example:
         eogrow config_files/config.json
     """
 
@@ -101,16 +101,16 @@
 def run_pipeline_on_cluster(
     config_path: str,
     cluster_yaml: str,
     start_cluster: bool,
     stop_cluster: bool,
     use_screen: bool,
     use_tmux: bool,
-    cli_variables: Tuple[str],
-    test_patches: Tuple[int],
+    cli_variables: Tuple[str, ...],
+    test_patches: Tuple[int, ...],
 ) -> None:
     """Command for running an eo-grow pipeline on a remote Ray cluster of AWS EC2 instances. The provided config is
     fully constructed and uploaded to the cluster head in the `~/.synced_configs/` directory, where it is then
     executed. A custom suffix is added to distinguish runs which use the same config multiple times.
 
     \b
     Example:
```

### Comparing `eo_grow-1.5.0/eogrow/types.py` & `eo_grow-1.5.1/eogrow/types.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/base.py` & `eo_grow-1.5.1/eogrow/core/base.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/config.py` & `eo_grow-1.5.1/eogrow/core/config.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/logging.py` & `eo_grow-1.5.1/eogrow/core/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         include_logs_to_report: bool = Field(
             False,
             description=(
                 "If log files should be parsed into an EOExecution report file or just linked. When working "
                 "with larger number of EOPatches the recommended option is False."
             ),
         )
-        eoexecution_ignore_packages: Tuple[str] = Field(
+        eoexecution_ignore_packages: Tuple[str, ...] = Field(
             (DEFAULT_PACKAGES_TOKEN,),
             description=(
                 "Names of packages for which the logs will not be written to EOExecution log files. You can reference"
                 ' the defaults with "...", for example, adding another package can be done with ["...", "some_package"]'
             ),
         )
 
-        pipeline_ignore_packages: Tuple[str] = Field(
+        pipeline_ignore_packages: Tuple[str, ...] = Field(
             (DEFAULT_PACKAGES_TOKEN,),
             description=(
                 "Names of packages for which the logs will not be written to the main pipeline log file. You can"
                 ' reference the defaults with "...", for example, adding another package can be done with'
                 ' ["...", "some_package"]'
             ),
         )
@@ -67,15 +67,15 @@
             description=(
                 "When working with a remote storage this parameter defines a minimal number of seconds between "
                 "two consecutive times when pipeline log file will be copied into the remote storage."
             ),
         )
 
         show_logs: bool = Field(False, description="Shows basic pipeline execution logs at stdout.")
-        stdout_log_packages: Tuple[str] = Field(
+        stdout_log_packages: Tuple[str, ...] = Field(
             (DEFAULT_PACKAGES_TOKEN,),
             description=(
                 "Names of packages for which the logs will be written to stdout. You can reference the defaults with"
                 ' "...", for example, adding another package can be done with ["...", "package_to_display"]'
             ),
         )
```

### Comparing `eo_grow-1.5.0/eogrow/core/pipeline.py` & `eo_grow-1.5.1/eogrow/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/schemas.py` & `eo_grow-1.5.1/eogrow/core/schemas.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/storage.py` & `eo_grow-1.5.1/eogrow/core/storage.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/area/base.py` & `eo_grow-1.5.1/eogrow/core/area/base.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/area/batch.py` & `eo_grow-1.5.1/eogrow/core/area/batch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/area/custom_grid.py` & `eo_grow-1.5.1/eogrow/core/area/custom_grid.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/core/area/utm.py` & `eo_grow-1.5.1/eogrow/core/area/utm.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/batch_to_eopatch.py` & `eo_grow-1.5.1/eogrow/pipelines/batch_to_eopatch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/byoc.py` & `eo_grow-1.5.1/eogrow/pipelines/byoc.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/download.py` & `eo_grow-1.5.1/eogrow/pipelines/download.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/download_batch.py` & `eo_grow-1.5.1/eogrow/pipelines/download_batch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/export_maps.py` & `eo_grow-1.5.1/eogrow/pipelines/export_maps.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/features.py` & `eo_grow-1.5.1/eogrow/pipelines/features.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/import_tiff.py` & `eo_grow-1.5.1/eogrow/pipelines/import_tiff.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/import_vector.py` & `eo_grow-1.5.1/eogrow/pipelines/import_vector.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/merge_samples.py` & `eo_grow-1.5.1/eogrow/pipelines/merge_samples.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/prediction.py` & `eo_grow-1.5.1/eogrow/pipelines/prediction.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/rasterize.py` & `eo_grow-1.5.1/eogrow/pipelines/rasterize.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/sampling.py` & `eo_grow-1.5.1/eogrow/pipelines/sampling.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/split_grid.py` & `eo_grow-1.5.1/eogrow/pipelines/split_grid.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/testing.py` & `eo_grow-1.5.1/eogrow/pipelines/testing.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/training.py` & `eo_grow-1.5.1/eogrow/pipelines/training.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/pipelines/zipmap.py` & `eo_grow-1.5.1/eogrow/pipelines/zipmap.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/tasks/batch_to_eopatch.py` & `eo_grow-1.5.1/eogrow/tasks/batch_to_eopatch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/tasks/common.py` & `eo_grow-1.5.1/eogrow/tasks/common.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/tasks/features.py` & `eo_grow-1.5.1/eogrow/tasks/features.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/tasks/prediction.py` & `eo_grow-1.5.1/eogrow/tasks/prediction.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/tasks/spatial.py` & `eo_grow-1.5.1/eogrow/tasks/spatial.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/tasks/testing.py` & `eo_grow-1.5.1/eogrow/tasks/testing.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/batch.py` & `eo_grow-1.5.1/eogrow/utils/batch.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/eopatch_list.py` & `eo_grow-1.5.1/eogrow/utils/eopatch_list.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/filter.py` & `eo_grow-1.5.1/eogrow/utils/filter.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/fs.py` & `eo_grow-1.5.1/eogrow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/general.py` & `eo_grow-1.5.1/eogrow/utils/general.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/grid.py` & `eo_grow-1.5.1/eogrow/utils/grid.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/logging.py` & `eo_grow-1.5.1/eogrow/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/map.py` & `eo_grow-1.5.1/eogrow/utils/map.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/meta.py` & `eo_grow-1.5.1/eogrow/utils/meta.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/ray.py` & `eo_grow-1.5.1/eogrow/utils/ray.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/testing.py` & `eo_grow-1.5.1/eogrow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/validators.py` & `eo_grow-1.5.1/eogrow/utils/validators.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/vector.py` & `eo_grow-1.5.1/eogrow/utils/vector.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/eogrow/utils/zipmap.py` & `eo_grow-1.5.1/eogrow/utils/zipmap.py`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/.gitignore` & `eo_grow-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/LICENSE` & `eo_grow-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/README.md` & `eo_grow-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/pyproject.toml` & `eo_grow-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eo_grow-1.5.0/PKG-INFO` & `eo_grow-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-grow
-Version: 1.5.0
+Version: 1.5.1
 Summary: Earth observation framework for scaled-up processing in Python
 Project-URL: Homepage, https://github.com/sentinel-hub/eo-grow
 Project-URL: Documentation, https://eo-grow.readthedocs.io
 Project-URL: Issues, https://github.com/sentinel-hub/eo-grow/issues
 Project-URL: Source, https://github.com/sentinel-hub/eo-grow
 Project-URL: Forum, https://forum.sentinel-hub.com
 Author-email: Sinergise EO research team <eoresearch@sinergise.com>
```

