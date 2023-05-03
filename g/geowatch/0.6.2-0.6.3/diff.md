# Comparing `tmp/geowatch-0.6.2.tar.gz` & `tmp/geowatch-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geowatch-0.6.2.tar", last modified: Wed May  3 00:23:05 2023, max compression
+gzip compressed data, was "geowatch-0.6.3.tar", last modified: Wed May  3 04:02:52 2023, max compression
```

## Comparing `geowatch-0.6.2.tar` & `geowatch-0.6.3.tar`

### file list

```diff
@@ -1,1042 +1,1042 @@
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.798164 geowatch-0.6.2/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19164 2023-05-03 00:21:52.000000 geowatch-0.6.2/CHANGELOG.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7765 2023-04-29 23:47:47.000000 geowatch-0.6.2/Dockerfile
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11343 2022-12-02 18:15:30.000000 geowatch-0.6.2/LICENSE
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      313 2022-06-07 15:49:12.000000 geowatch-0.6.2/MANIFEST.in
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-03 00:23:05.798164 geowatch-0.6.2/PKG-INFO
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6414 2023-05-03 00:21:52.000000 geowatch-0.6.2/README.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1646 2023-05-02 02:20:39.000000 geowatch-0.6.2/conda_env.yml
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      406 2022-06-07 15:49:12.000000 geowatch-0.6.2/conftest.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      642 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/README.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/algorithms/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1556 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/algorithms/fusion_overview.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2557 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/algorithms/sensorchan_specs.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      533 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/algorithms/ta2_deep_dive_info.md
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6892 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/data/access_dvc_repos.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1625 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/data/internal_resources.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1269 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/data/using_smartwatch_dvc.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/debugging/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1598 2023-04-03 19:39:09.000000 geowatch-0.6.2/docs/debugging/debugging_cmdqueue.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/development/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/development/coding_conventions.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3525 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/development/coding_tips.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1903 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/development/contribution_instructions.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3258 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/development/rebasing_procedure.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11705 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/development/ta2_feature_integration.md
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/environment/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10365 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/environment/getting_started_aws.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6890 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/environment/getting_started_dvc.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1172 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/environment/getting_started_kubectl.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6599 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/environment/getting_started_ssh_keys.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      544 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/environment/install_python.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2234 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/environment/install_python_conda.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/environment/install_python_pyenv.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3099 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/environment/installing_geowatch.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6804 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/environment/windows.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       24 2023-03-21 17:57:36.000000 geowatch-0.6.2/docs/index.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/misc/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6162 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/misc/structure_proposal.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1986 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/misc/supporting_projects.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11380 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/mlops.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5235 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/onboarding.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/smartflow/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2767 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/smartflow/getting_started_smartflow.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3465 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/smartflow/smartflow_copying_large_files_to_efs.md
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20420 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/smartflow/smartflow_running_the_system.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3164 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/smartflow/smartflow_training_fusion_models.md
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/docs/testing/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2015 2023-04-29 23:47:47.000000 geowatch-0.6.2/docs/testing/running_ci_locally.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2139 2023-05-02 02:20:39.000000 geowatch-0.6.2/docs/testing/testing_practices.rst
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14398 2023-05-03 00:21:52.000000 geowatch-0.6.2/docs/watch_cli.rst
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/geowatch/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      163 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       69 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/__main__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/cli/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       73 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/animate_visualizations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/baseline_framework_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/baseline_framework_ingress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/baseline_framework_kwcoco_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/baseline_framework_kwcoco_ingress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/cluster_sites.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_add_watch_fields.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_align.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_align_geotiffs.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_average_features.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_clean_geotiffs.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_combine_features.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_crop_tracks.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_intensity_histograms.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_reformat_channels.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_remove_bad_images.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_remove_empty_images.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_shard.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_spectra.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_time_combine.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_update_geotiff_metadata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/coco_visualize_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/concat_kwcoco_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/crop_sites_to_regions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/cli/dag_cli/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_bas_datagen.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_bas_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_pseudolive_consolidate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_psuedolive_copy_previous.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_sc_datagen.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_sc_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/dag_cli/run_teamfeat_invariants.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/extend_sc_sites.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/find_dvc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/geojson_site_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/geotiffs_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/gifify.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/kwcoco_to_geojson.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/merge_region_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/mlops_cli.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/prepare_splits.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/prepare_ta2_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/prepare_teamfeats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/pseudolive_consolidate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/reproject_annotations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/run_fusion_predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/run_metrics_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/run_tracker.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/split_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/stac_search.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/ta1_stac_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/torch_model_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/validate_annotation_schemas.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/cli/watch_coco_stats.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/demo_region.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/dummy_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/landsat_demodata.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/demo/metrics_demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/metrics_demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/metrics_demo/demo_rendering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/metrics_demo/demo_truth.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/metrics_demo/demo_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/metrics_demo/generate_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/metrics_demo/site_perterbing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/nitf_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/sentinel2_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/smart_kwcoco_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/demo/stac_demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/exceptions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/geoannots/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/geoannots/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/geoannots/geomodels.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/geoannots/make_region_from_sites.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/gis/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/digital_globe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/elevation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/geotiff.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.742164 geowatch-0.6.2/geowatch/gis/sensors/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/sensors/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/sensors/sentinel2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/gis/spatial_reference.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/heuristics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/mlops/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       75 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/aggregate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/aggregate_loader.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/confusion_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/confusor_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/manager.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/mlops/old/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/expt_manager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/expt_report.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/expt_state.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/old_pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/old_plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/pipeline_v1.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/old/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/repackager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/schedule_evaluation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/smart_global_helper.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/smart_pipeline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/mlops/smart_result_parser.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/monkey/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      170 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/_monkey_fbeta.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_albumentations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_lightning.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_numpy.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_pil.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_tensorflow.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_torch.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/monkey/monkey_torchmetrics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/rc/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      166 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/rc/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/rc/registry.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/stac/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/stac/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/stac/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/stac/stac_search_builder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/stac/util_stac.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/tasks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/tasks/cold/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/assemble_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/export_change_map.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/export_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/prepare_ard.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/prepare_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/tile_processing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/cold/tile_processing_kwcoco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/tasks/depth/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/backbone.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/demo_transform.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/dzyne_img_util.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/modules_monkeypatch.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/pl_highres_verify.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/depth/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/tasks/dino_detector/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/dino_detector/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/dino_detector/package_building_detector.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/dino_detector/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.746165 geowatch-0.6.2/geowatch/tasks/fusion/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       82 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/aggregate_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/fusion/architectures/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/architectures/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/architectures/segmenter_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/architectures/sits.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/architectures/transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/architectures/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/architectures/wu_mae.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/coco_stitcher.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/batch_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/data_augment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/data_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/demos_for_slides.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/kwcoco_datamodule.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/kwcoco_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/kwcoco_video_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/qa_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/smart_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/spacetime_grid_builder.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      216 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/affinity.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/sampler.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      226 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/datamodules/temporal_sampling/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/evaluate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/fit_lightning.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/fusion/methods/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/channelwise_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/heterogeneous.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/network_modules.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/noop_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/unet_baseline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/methods/watch_module_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/organize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      367 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/production.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/fusion/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/invariants/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/change.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/invariants/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/data/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/data/multi_image_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/data/other_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/fit_segment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/pretext_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/invariants/segmentation_model.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/landcover/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/detector.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/model_info.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/nets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/landcover/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/metrics/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/metrics/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/metrics/merge_iarpa_metrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/metrics/viz_sc_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.750165 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.754165 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/apnb.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/base_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/discritizers.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      232 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      238 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/peri_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/pos_embedding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/self_attention.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/simple_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/timesformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/unet_lstm.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/models/vit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/predict_sc.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.754165 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/util_config.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/util_misc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/util_paths.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_change_detection/utils/util_visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.754165 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.754165 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/bigearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/deepglobe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/hrscd.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/inria.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/s2_self.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/s2mcp.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/spacenet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/spacenet2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/datasets/sysucd.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.758165 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/inria_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/moco_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      239 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/onera_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      230 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      234 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/setr_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.758165 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/canny_edge.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/deeplab.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/deeplabWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/deeplab_diff.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/encoding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/gci.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/linear_classifier.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/losses.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/moco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/quantizer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/resnetGNWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/sg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/shallow_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/supcon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/tex_refine.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/transformer_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/models/transformer_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/predict_patchwise.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/predict_test.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.758165 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/scripts/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/scripts/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.758165 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/cva.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/eval_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/rutgers_material_seg/utils/visualization.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.758165 geowatch-0.6.2/geowatch/tasks/tracking/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/from_heatmap.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/from_polygon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/normalize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/phase.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/tracking/visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.758165 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/drop0_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.762164 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/models/resnets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/models/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.762164 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.762164 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.762164 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      246 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/spacenet/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/time_sort_S7.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/time_sort_module.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/tasks/uky_temporal_prediction/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.762164 geowatch-0.6.2/geowatch/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/configargparse_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/ext_monai.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/ijson_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/kwcoco_extensions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.762164 geowatch-0.6.2/geowatch/utils/lightning_ext/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/argparse_ext.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.766164 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/auto_resumer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/batch_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/packager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/state_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/tensorboard_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/callbacks/text_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/lightning_cli_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/monkeypatches.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/old_parser_devices.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/util_device.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/lightning_ext/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/partial_format.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/process_context.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/result_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/reverse_hashid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/simple_dvc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/slugify_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_codes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_dotdict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_environ.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_eval.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_gdal.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_girder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_gis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_hardware.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_iter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_json.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_kwarray.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_kwimage.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_kwplot.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_locks.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_logging.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_nesting.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_netharn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_pandas.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_parallel.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_param_grid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_path.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_pattern.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_progress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_raster.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_regex.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_resolution.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_resources.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_rgdc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_s3.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_stringalgo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_time.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_torchmetrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.2/geowatch/utils/util_yaml.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.738165 geowatch-0.6.2/geowatch.egg-info/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-03 00:23:05.000000 geowatch-0.6.2/geowatch.egg-info/PKG-INFO
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40654 2023-05-03 00:23:05.000000 geowatch-0.6.2/geowatch.egg-info/SOURCES.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-05-03 00:23:05.000000 geowatch-0.6.2/geowatch.egg-info/dependency_links.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-05-03 00:23:05.000000 geowatch-0.6.2/geowatch.egg-info/entry_points.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-04-27 14:57:33.000000 geowatch-0.6.2/geowatch.egg-info/not-zip-safe
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18527 2023-05-03 00:23:05.000000 geowatch-0.6.2/geowatch.egg-info/requires.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       15 2023-05-03 00:23:05.000000 geowatch-0.6.2/geowatch.egg-info/top_level.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2429 2023-04-29 23:47:47.000000 geowatch-0.6.2/pyproject.toml
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.766164 geowatch-0.6.2/requirements/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-05-02 02:20:39.000000 geowatch-0.6.2/requirements/cold.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      562 2023-05-03 00:21:52.000000 geowatch-0.6.2/requirements/development.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       19 2023-05-02 02:20:39.000000 geowatch-0.6.2/requirements/dvc.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      445 2023-04-29 21:01:30.000000 geowatch-0.6.2/requirements/gdal.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      889 2023-04-03 19:39:09.000000 geowatch-0.6.2/requirements/graphics.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      979 2023-04-03 19:39:09.000000 geowatch-0.6.2/requirements/headless.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      110 2023-05-02 02:20:39.000000 geowatch-0.6.2/requirements/linting.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.2/requirements/mmcv.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      318 2023-05-02 02:20:39.000000 geowatch-0.6.2/requirements/optional.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9002 2023-05-03 00:21:52.000000 geowatch-0.6.2/requirements/runtime.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       86 2023-05-02 02:20:39.000000 geowatch-0.6.2/requirements/tensorflow.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       88 2023-04-29 21:01:30.000000 geowatch-0.6.2/requirements/tests.txt
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2023-04-29 21:01:30.000000 geowatch-0.6.2/requirements.txt
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      823 2023-04-03 19:39:09.000000 geowatch-0.6.2/run_tests.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       38 2023-05-03 00:23:05.798164 geowatch-0.6.2/setup.cfg
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10526 2023-05-03 00:21:52.000000 geowatch-0.6.2/setup.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.766164 geowatch-0.6.2/tests/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1271 2023-04-29 23:47:47.000000 geowatch-0.6.2/tests/test_cli.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2530 2023-04-29 23:47:47.000000 geowatch-0.6.2/tests/test_heterogeneous_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4038 2022-12-02 18:15:30.000000 geowatch-0.6.2/tests/test_init_from_pretrained.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2277 2023-03-21 17:57:36.000000 geowatch-0.6.2/tests/test_kwcoco_dataloader.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8409 2023-05-03 00:21:52.000000 geowatch-0.6.2/tests/test_lightning_cli_fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4446 2023-04-29 21:01:30.000000 geowatch-0.6.2/tests/test_load_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4367 2023-04-29 23:47:47.000000 geowatch-0.6.2/tests/test_mlops_scheduler.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7349 2023-04-29 21:01:30.000000 geowatch-0.6.2/tests/test_predict_latest_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4669 2023-04-29 21:01:30.000000 geowatch-0.6.2/tests/test_predict_old_fusion_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3440 2023-04-29 23:47:47.000000 geowatch-0.6.2/tests/test_predict_small_region.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6717 2023-04-29 21:01:30.000000 geowatch-0.6.2/tests/test_save_packages.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2514 2022-12-20 16:17:52.000000 geowatch-0.6.2/tests/test_sensor_metadata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13860 2023-04-29 23:47:47.000000 geowatch-0.6.2/tests/test_tracker.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      134 2022-06-07 15:49:12.000000 geowatch-0.6.2/tests/test_version.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.766164 geowatch-0.6.2/watch/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      139 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/__main__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/cli/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       98 2023-01-18 16:43:36.000000 geowatch-0.6.2/watch/cli/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5627 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/__main__.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7854 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/animate_visualizations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6116 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/cli/baseline_framework_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16017 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/cli/baseline_framework_ingress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6070 2022-12-14 20:49:04.000000 geowatch-0.6.2/watch/cli/baseline_framework_kwcoco_egress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3673 2022-12-14 20:49:04.000000 geowatch-0.6.2/watch/cli/baseline_framework_kwcoco_ingress.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10809 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/cluster_sites.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5800 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/cli/coco_add_watch_fields.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    95340 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/cli/coco_align.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      215 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/coco_align_geotiffs.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32128 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/coco_average_features.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    34654 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/coco_clean_geotiffs.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9577 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/coco_combine_features.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22525 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/coco_crop_tracks.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      224 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/coco_intensity_histograms.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10091 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/coco_reformat_channels.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    11078 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/coco_remove_bad_images.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2653 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/coco_shard.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32293 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/coco_spectra.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    42369 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/coco_time_combine.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4771 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/coco_update_geotiff_metadata.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    61267 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/cli/coco_visualize_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1814 2022-12-14 20:49:04.000000 geowatch-0.6.2/watch/cli/concat_kwcoco_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15924 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/crop_sites_to_regions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/cli/dag_cli/
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)       89 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/dag_cli/__init__.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15320 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/dag_cli/run_bas_datagen.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    13342 2023-05-01 17:33:03.000000 geowatch-0.6.2/watch/cli/dag_cli/run_bas_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10286 2023-05-01 17:33:03.000000 geowatch-0.6.2/watch/cli/dag_cli/run_dino_sv.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6939 2023-05-01 19:59:37.000000 geowatch-0.6.2/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3529 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/dag_cli/run_pseudolive_consolidate.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3062 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/dag_cli/run_psuedolive_copy_previous.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7796 2023-05-01 17:33:03.000000 geowatch-0.6.2/watch/cli/dag_cli/run_sc_datagen.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12667 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/cli/dag_cli/run_sc_fusion.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6224 2023-05-01 17:33:03.000000 geowatch-0.6.2/watch/cli/dag_cli/run_sv_datagen.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5581 2023-04-03 20:48:44.000000 geowatch-0.6.2/watch/cli/dag_cli/run_teamfeat_invariants.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5448 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/dag_cli/run_teamfeat_landcover.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11711 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/cli/extend_sc_sites.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4586 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/find_dvc.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12269 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/geojson_site_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14799 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/geotiffs_to_kwcoco.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10815 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/cli/gifify.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    60306 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/kwcoco_to_geojson.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4375 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/cli/merge_region_models.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/mlops_cli.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10349 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/prepare_splits.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    38053 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/prepare_ta2_dataset.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    29934 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/prepare_teamfeats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14855 2022-12-14 20:49:04.000000 geowatch-0.6.2/watch/cli/pseudolive_consolidate.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    69727 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/reproject_annotations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       84 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/cli/run_fusion_predict.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    20415 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/run_metrics_framework.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      271 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/cli/run_tracker.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4224 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/split_videos.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22737 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/stac_search.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    27798 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/cli/ta1_stac_to_kwcoco.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9391 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/torch_model_stats.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16252 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/cli/validate_annotation_schemas.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15553 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/cli/watch_coco_stats.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2624 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20892 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/demo/demo_region.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      563 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/demo/dummy_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7543 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/demo/landsat_demodata.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/demo/metrics_demo/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      138 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/demo/metrics_demo/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7448 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/demo/metrics_demo/demo_rendering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24604 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/demo/metrics_demo/demo_truth.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13005 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/demo/metrics_demo/demo_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6307 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/demo/metrics_demo/generate_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15545 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/demo/metrics_demo/site_perterbing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29938 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/demo/nitf_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3676 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/demo/sentinel2_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25225 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/demo/smart_kwcoco_demodata.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4089 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/demo/stac_demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/exceptions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/geoannots/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      989 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/geoannots/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2308 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/geoannots/geococo_objects.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16872 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/geoannots/geomodels.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/gis/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1645 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/gis/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9291 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/gis/digital_globe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10020 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/gis/elevation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51299 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/gis/geotiff.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.770164 geowatch-0.6.2/watch/gis/sensors/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      326 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/gis/sensors/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6516 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/gis/sensors/sentinel2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13106 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/gis/spatial_reference.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26467 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/heuristics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/mlops/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/mlops/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      670 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/mlops/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70579 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/mlops/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70055 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/mlops/aggregate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17109 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/mlops/aggregate_loader.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23469 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/mlops/confusion_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25565 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/mlops/confusor_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40297 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/mlops/manager.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/mlops/old/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/mlops/old/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18067 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/mlops/old/expt_manager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39383 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/mlops/old/expt_report.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44820 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/mlops/old/expt_state.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39219 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/mlops/old/old_pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10290 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/mlops/old/old_plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8717 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/mlops/old/pipeline_v1.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39647 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/mlops/old/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55208 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/mlops/pipeline_nodes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12686 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/mlops/repackager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16868 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/mlops/schedule_evaluation.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22712 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/mlops/smart_global_helper.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32124 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/mlops/smart_pipeline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33368 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/mlops/smart_result_parser.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/monkey/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       62 2022-12-14 20:49:53.000000 geowatch-0.6.2/watch/monkey/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4095 2022-12-14 20:49:53.000000 geowatch-0.6.2/watch/monkey/_monkey_fbeta.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4047 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/monkey/monkey_albumentations.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      280 2022-12-14 20:49:53.000000 geowatch-0.6.2/watch/monkey/monkey_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1187 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/monkey/monkey_lightning.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/monkey/monkey_numpy.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2022-12-14 20:49:53.000000 geowatch-0.6.2/watch/monkey/monkey_pil.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/monkey/monkey_tensorflow.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/monkey/monkey_torch.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      601 2022-12-14 20:49:53.000000 geowatch-0.6.2/watch/monkey/monkey_torchmetrics.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/rc/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1715 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/rc/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9626 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/rc/registry.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/stac/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       66 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/stac/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17312 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/stac/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14251 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/stac/stac_search_builder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9733 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/stac/util_stac.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/tasks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1677 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/tasks/cold/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/tasks/cold/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17557 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/cold/assemble_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21171 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/tasks/cold/export_change_map.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18314 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/cold/export_cold_result_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15969 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/cold/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    73485 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/cold/prepare_ard.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23475 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/cold/prepare_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30062 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/tasks/cold/tile_processing.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28290 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/cold/tile_processing_kwcoco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.774165 geowatch-0.6.2/watch/tasks/depth/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/depth/__init__.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4501 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/depth/backbone.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6559 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/depth/config.json
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6816 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/depth/datasets.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4372 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/depth/demo_transform.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     8379 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/depth/dzyne_img_util.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      295 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/depth/modules_monkeypatch.py
--rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5239 2022-08-09 13:10:41.000000 geowatch-0.6.2/watch/tasks/depth/pl_highres_verify.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24371 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/depth/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5689 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/depth/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/depthPCD/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-01 19:59:37.000000 geowatch-0.6.2/watch/tasks/depthPCD/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6700 2023-05-01 19:59:37.000000 geowatch-0.6.2/watch/tasks/depthPCD/model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      407 2023-05-01 19:59:37.000000 geowatch-0.6.2/watch/tasks/depthPCD/model_test.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20132 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/depthPCD/score_tracks.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/dino_detector/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/dino_detector/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24608 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/dino_detector/building_validator.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10562 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/dino_detector/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/fusion/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2501 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/fusion/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       72 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/fusion/__main__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    82304 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/fusion/aggregate_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/fusion/architectures/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/fusion/architectures/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11883 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/architectures/segmenter_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5979 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/tasks/fusion/architectures/sits.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51015 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/architectures/transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4989 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/fusion/architectures/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6302 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/architectures/wu_mae.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    36730 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/fusion/coco_stitcher.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/fusion/datamodules/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      336 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9680 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48055 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/batch_visualization.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8458 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/data_augment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18677 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/data_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9780 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/demos_for_slides.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29470 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/kwcoco_datamodule.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   149541 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/kwcoco_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      373 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/kwcoco_video_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23364 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/qa_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14225 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/smart_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    53890 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/spacetime_grid_builder.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1527 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10375 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44675 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       44 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9422 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/plots.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39631 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3384 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7352 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55018 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/evaluate.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28542 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19157 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/fusion/fit_lightning.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.778164 geowatch-0.6.2/watch/tasks/fusion/methods/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      741 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/tasks/fusion/methods/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    81666 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/methods/channelwise_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    79880 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/methods/heterogeneous.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25464 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/methods/network_modules.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8960 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/methods/noop_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28643 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/methods/unet_baseline.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32192 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/methods/watch_module_mixins.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4468 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/fusion/organize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61751 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/fusion/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14896 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/fusion/production.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16789 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/fusion/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/invariants/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/invariants/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13603 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/invariants/change.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/invariants/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/invariants/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35389 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/invariants/data/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20577 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/invariants/data/multi_image_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25778 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/invariants/data/other_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5589 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/invariants/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4483 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/invariants/fit_segment.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6709 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/invariants/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24584 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/invariants/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15963 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/invariants/pretext_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12941 2022-08-09 13:10:41.000000 geowatch-0.6.2/watch/tasks/invariants/segmentation_model.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/landcover/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/landcover/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6028 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/landcover/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5623 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/landcover/detector.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      103 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/landcover/fit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2377 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/landcover/model_info.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2360 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/tasks/landcover/nets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12281 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/landcover/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      349 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/landcover/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/metrics/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/tasks/metrics/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26517 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/tasks/metrics/merge_iarpa_metrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11867 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/metrics/viz_sc_results.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8025 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33579 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    31719 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19805 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    34195 2022-08-09 13:10:41.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22473 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9162 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/apnb.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5007 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/base_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8375 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/discritizers.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4272 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1276 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3510 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7979 2022-08-09 13:10:41.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5652 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16573 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2864 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11476 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6888 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15931 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3732 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/self_attention.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6771 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3779 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1833 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9772 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24297 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/timesformer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6020 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8684 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4982 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/vit.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10698 2022-08-09 13:10:41.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9087 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/predict_sc.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.782164 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_config.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10512 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_misc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2112 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1508 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_paths.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9883 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.786164 geowatch-0.6.2/watch/tasks/rutgers_material_seg/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.786164 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3274 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11109 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4313 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/deepglobe.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5959 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/hrscd.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13129 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8257 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6702 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/inria.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3910 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/s2_self.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3309 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/s2mcp.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/spacenet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6266 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/spacenet2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3830 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/sysucd.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.786164 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42088 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19562 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26483 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    52228 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40645 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17085 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    46366 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42111 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45628 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16504 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/moco_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21771 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10831 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4437 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61390 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    49788 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    65883 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    78136 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56648 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70057 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67609 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    66954 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30059 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/setr_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32133 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35336 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48335 2023-04-19 20:35:11.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7030 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    60321 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       70 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1466 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7650 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/canny_edge.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13281 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/deeplab.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17807 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/deeplabWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13507 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/deeplab_diff.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2845 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/encoding.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3794 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/gci.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/linear_classifier.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11714 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/losses.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5727 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/moco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9085 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/quantizer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11438 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7592 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnetGNWS.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12182 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19182 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnet_enc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1414 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/sg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4967 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/shallow_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7222 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/supcon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4278 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/tex_refine.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12022 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/transformer_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6462 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/transformer_seg.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33755 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/predict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14703 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/predict_patchwise.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14964 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/predict_test.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/rutgers_material_seg/scripts/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/scripts/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1884 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3932 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5761 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3861 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/cva.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12756 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/eval_utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13993 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9925 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/visualization.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1728 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7209 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11244 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11762 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      446 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5883 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6146 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/sam/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/tasks/sam/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17730 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/sam/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/tracking/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1582 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/tracking/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    58501 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/tracking/from_heatmap.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2904 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/tracking/from_polygon.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30472 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/tracking/normalize.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21464 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/tasks/tracking/phase.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23668 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/tasks/tracking/utils.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7531 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/tasks/tracking/visualize.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15495 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/drop0_datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3118 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/fit.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.790164 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5614 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/resnets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5466 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/unet.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10027 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/unet_blur.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8395 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/predict.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.794164 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/__init__.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.794164 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2057 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.794164 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2093 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16199 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/datasets.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5987 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/time_sort_S7.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4070 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/time_sort_module.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      594 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/tasks/uky_temporal_prediction/utils.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.798164 geowatch-0.6.2/watch/utils/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2803 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12992 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/configargparse_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48556 2023-02-02 14:12:29.000000 geowatch-0.6.2/watch/utils/ext_monai.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11626 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/utils/ijson_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   116465 2023-05-02 20:05:02.000000 geowatch-0.6.2/watch/utils/kwcoco_extensions.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.798164 geowatch-0.6.2/watch/utils/lightning_ext/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      376 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/utils/lightning_ext/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21356 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20330 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7034 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/argparse_ext.py
-drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:23:05.798164 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1244 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/__init__.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5735 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/auto_resumer.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8793 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/batch_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10112 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/packager.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2693 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/state_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16120 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13026 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/callbacks/text_logger.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4371 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/lightning_ext/demo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3211 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/lightning_ext/lightning_cli_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2022-12-14 20:49:53.000000 geowatch-0.6.2/watch/utils/lightning_ext/monkeypatches.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7558 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/utils/lightning_ext/old_parser_devices.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5712 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/utils/lightning_ext/util_device.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      303 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/utils/lightning_ext/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      434 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/utils/lightning_ext/util_model.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10606 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/partial_format.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11208 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/process_context.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56465 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/result_analysis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5456 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/reverse_hashid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13733 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/simple_dvc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8514 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/utils/slugify_ext.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41201 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/util_bands.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1059 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/utils/util_codes.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12129 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/utils/util_data.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7144 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_dotdict.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1813 2023-02-27 18:47:15.000000 geowatch-0.6.2/watch/utils/util_environ.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2733 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_eval.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7920 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/utils/util_framework.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    47570 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_gdal.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/utils/util_girder.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    43860 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/util_gis.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2747 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/utils/util_globals.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2039 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/utils/util_hardware.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2589 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/utils/util_iter.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3455 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_json.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41820 2023-05-01 17:33:03.000000 geowatch-0.6.2/watch/utils/util_kwarray.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67297 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/util_kwimage.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14504 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/util_kwplot.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3771 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/utils/util_locks.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8978 2022-12-14 20:49:04.000000 geowatch-0.6.2/watch/utils/util_logging.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1035 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_nesting.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12514 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_netharn.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10172 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/util_nvidia.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10275 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_pandas.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5746 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_parallel.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25992 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/utils/util_param_grid.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18404 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_path.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13282 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_pattern.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23235 2023-04-29 21:01:30.000000 geowatch-0.6.2/watch/utils/util_progress.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15872 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/utils/util_raster.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3028 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/utils/util_regex.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7614 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/utils/util_resolution.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3542 2023-05-02 02:20:39.000000 geowatch-0.6.2/watch/utils/util_resources.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3083 2022-06-07 15:49:12.000000 geowatch-0.6.2/watch/utils/util_rgdc.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      570 2022-12-02 18:15:30.000000 geowatch-0.6.2/watch/utils/util_s3.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7307 2023-03-21 17:57:36.000000 geowatch-0.6.2/watch/utils/util_stringalgo.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13699 2023-04-03 19:39:09.000000 geowatch-0.6.2/watch/utils/util_time.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1786 2022-12-20 16:17:52.000000 geowatch-0.6.2/watch/utils/util_torchmetrics.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2133 2023-05-03 00:21:52.000000 geowatch-0.6.2/watch/utils/util_windows.py
--rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9413 2023-04-29 23:47:47.000000 geowatch-0.6.2/watch/utils/util_yaml.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.957887 geowatch-0.6.3/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19164 2023-05-03 00:21:52.000000 geowatch-0.6.3/CHANGELOG.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7765 2023-04-29 23:47:47.000000 geowatch-0.6.3/Dockerfile
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11343 2022-12-02 18:15:30.000000 geowatch-0.6.3/LICENSE
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      313 2022-06-07 15:49:12.000000 geowatch-0.6.3/MANIFEST.in
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-03 04:02:52.957887 geowatch-0.6.3/PKG-INFO
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6414 2023-05-03 00:21:52.000000 geowatch-0.6.3/README.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1646 2023-05-02 02:20:39.000000 geowatch-0.6.3/conda_env.yml
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      406 2022-06-07 15:49:12.000000 geowatch-0.6.3/conftest.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      642 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/README.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/algorithms/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1556 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/algorithms/fusion_overview.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2557 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/algorithms/sensorchan_specs.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      533 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/algorithms/ta2_deep_dive_info.md
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6892 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/data/access_dvc_repos.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1625 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/data/internal_resources.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1269 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/data/using_smartwatch_dvc.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/debugging/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1598 2023-04-03 19:39:09.000000 geowatch-0.6.3/docs/debugging/debugging_cmdqueue.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/development/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/coding_conventions.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3525 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/coding_tips.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1903 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/contribution_instructions.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3258 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/rebasing_procedure.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11705 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/development/ta2_feature_integration.md
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/environment/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10365 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_aws.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6890 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_dvc.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1172 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_kubectl.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6599 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/getting_started_ssh_keys.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      544 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/environment/install_python.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2234 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/environment/install_python_conda.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/environment/install_python_pyenv.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3099 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/environment/installing_geowatch.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6791 2023-05-03 04:02:03.000000 geowatch-0.6.3/docs/environment/windows.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       24 2023-03-21 17:57:36.000000 geowatch-0.6.3/docs/index.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/misc/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6162 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/misc/structure_proposal.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1986 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/misc/supporting_projects.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11380 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/mlops.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5235 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/onboarding.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/smartflow/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2767 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/smartflow/getting_started_smartflow.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3465 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/smartflow/smartflow_copying_large_files_to_efs.md
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20420 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/smartflow/smartflow_running_the_system.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3164 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/smartflow/smartflow_training_fusion_models.md
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/docs/testing/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2015 2023-04-29 23:47:47.000000 geowatch-0.6.3/docs/testing/running_ci_locally.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2139 2023-05-02 02:20:39.000000 geowatch-0.6.3/docs/testing/testing_practices.rst
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14398 2023-05-03 00:21:52.000000 geowatch-0.6.3/docs/watch_cli.rst
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.881887 geowatch-0.6.3/geowatch/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      163 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       69 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/__main__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/cli/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       73 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/animate_visualizations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_ingress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_kwcoco_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/baseline_framework_kwcoco_ingress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/cluster_sites.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_add_watch_fields.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_align.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_align_geotiffs.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_average_features.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_clean_geotiffs.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_combine_features.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_crop_tracks.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_intensity_histograms.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_reformat_channels.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_remove_bad_images.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_remove_empty_images.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_shard.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_spectra.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_time_combine.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_update_geotiff_metadata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/coco_visualize_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/concat_kwcoco_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/crop_sites_to_regions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/cli/dag_cli/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_bas_datagen.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_bas_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_pseudolive_consolidate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_psuedolive_copy_previous.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_sc_datagen.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_sc_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/dag_cli/run_teamfeat_invariants.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/extend_sc_sites.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/find_dvc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/geojson_site_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/geotiffs_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/gifify.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/kwcoco_to_geojson.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/merge_region_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/mlops_cli.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/prepare_splits.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/prepare_ta2_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/prepare_teamfeats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/pseudolive_consolidate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/reproject_annotations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/run_fusion_predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/run_metrics_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/run_tracker.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/split_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/stac_search.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/ta1_stac_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/torch_model_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/validate_annotation_schemas.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/cli/watch_coco_stats.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/demo_region.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/dummy_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/landsat_demodata.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/demo/metrics_demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/demo_rendering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/demo_truth.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/demo_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/generate_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/metrics_demo/site_perterbing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/nitf_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/sentinel2_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/smart_kwcoco_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/demo/stac_demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/exceptions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/geoannots/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/geoannots/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/geoannots/geomodels.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/geoannots/make_region_from_sites.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/gis/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      167 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/digital_globe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/elevation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/geotiff.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.889887 geowatch-0.6.3/geowatch/gis/sensors/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/sensors/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/sensors/sentinel2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/gis/spatial_reference.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/heuristics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/mlops/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       75 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/aggregate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/aggregate_loader.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/confusion_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/confusor_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/manager.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/mlops/old/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      173 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/expt_manager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/expt_report.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/expt_state.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/old_pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/old_plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/pipeline_v1.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/old/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/repackager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/schedule_evaluation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/smart_global_helper.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/smart_pipeline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/mlops/smart_result_parser.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/monkey/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      170 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/_monkey_fbeta.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_albumentations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_lightning.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_numpy.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_pil.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_tensorflow.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_torch.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/monkey/monkey_torchmetrics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/rc/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      166 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/rc/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/rc/registry.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/stac/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      168 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/stac_search_builder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/stac/util_stac.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/tasks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/tasks/cold/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/assemble_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/export_change_map.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/export_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      186 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/prepare_ard.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      189 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/prepare_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/tile_processing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/cold/tile_processing_kwcoco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.893887 geowatch-0.6.3/geowatch/tasks/depth/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/backbone.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/demo_transform.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/dzyne_img_util.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/modules_monkeypatch.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/pl_highres_verify.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/depth/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/dino_detector/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/dino_detector/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/dino_detector/package_building_detector.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/dino_detector/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      176 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       82 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/aggregate_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/architectures/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/segmenter_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/sits.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/architectures/wu_mae.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/coco_stitcher.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/batch_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/data_augment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/data_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/demos_for_slides.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/kwcoco_datamodule.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/kwcoco_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/kwcoco_video_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/qa_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/smart_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/spacetime_grid_builder.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      216 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/affinity.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/sampler.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      226 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/datamodules/temporal_sampling/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/evaluate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/fit_lightning.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/fusion/methods/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/channelwise_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/heterogeneous.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/network_modules.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/noop_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/unet_baseline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/methods/watch_module_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/organize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      367 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/production.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/fusion/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.897887 geowatch-0.6.3/geowatch/tasks/invariants/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/change.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/invariants/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/multi_image_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/data/other_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/fit_segment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/pretext_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/invariants/segmentation_model.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/landcover/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/detector.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/model_info.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/nets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/landcover/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/metrics/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/metrics/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/metrics/merge_iarpa_metrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      192 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/metrics/viz_sc_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/apnb.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/base_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/discritizers.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      232 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      238 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/peri_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/pos_embedding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/self_attention.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/simple_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/timesformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/unet_lstm.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/models/vit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/predict_sc.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.901887 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_config.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_misc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_paths.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_change_detection/utils/util_visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.905887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      190 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.905887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/bigearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/deepglobe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/hrscd.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/inria.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/s2_self.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/s2mcp.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/spacenet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/spacenet2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/datasets/sysucd.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.905887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      225 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      222 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      231 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      217 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/inria_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/moco_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      229 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      239 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      237 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      218 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      214 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/onera_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      227 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      230 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      234 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/setr_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      220 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      224 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      219 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/canny_edge.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/deeplab.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/deeplabWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/deeplab_diff.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/encoding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/gci.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/linear_classifier.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/losses.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/moco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/quantizer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnetGNWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      228 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/sg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/shallow_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      204 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/supcon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/tex_refine.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/transformer_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/models/transformer_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/predict_patchwise.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      203 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/predict_test.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      198 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      215 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      212 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/cva.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/eval_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/rutgers_material_seg/utils/visualization.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/tracking/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/from_heatmap.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      191 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/from_polygon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/normalize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/phase.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/tracking/visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/drop0_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      200 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      208 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/resnets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/models/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      221 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.909887 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      246 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      211 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/spacenet/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/time_sort_S7.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      210 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/time_sort_module.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/tasks/uky_temporal_prediction/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.913887 geowatch-0.6.3/geowatch/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      169 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/configargparse_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/ext_monai.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/ijson_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/kwcoco_extensions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.913887 geowatch-0.6.3/geowatch/utils/lightning_ext/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/argparse_ext.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      193 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/auto_resumer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/batch_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/packager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      206 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/state_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      213 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/tensorboard_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      205 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/callbacks/text_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      188 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      201 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/lightning_cli_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      197 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/monkeypatches.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      202 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/old_parser_devices.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      195 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/util_device.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      196 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      194 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/lightning_ext/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/partial_format.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/process_context.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/result_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/reverse_hashid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/simple_dvc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/slugify_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_codes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_dotdict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_environ.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_eval.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_gdal.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_girder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      178 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_gis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_hardware.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_iter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_json.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_kwarray.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_kwimage.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_kwplot.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_locks.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_logging.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_nesting.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_netharn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_pandas.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_parallel.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_param_grid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_path.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      182 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_pattern.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      183 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_progress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      181 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_raster.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_regex.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_resolution.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      184 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_resources.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_rgdc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      177 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_s3.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      185 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_stringalgo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_time.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      187 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_torchmetrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      179 2023-04-29 23:47:47.000000 geowatch-0.6.3/geowatch/utils/util_yaml.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.885887 geowatch-0.6.3/geowatch.egg-info/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7494 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/PKG-INFO
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40654 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/entry_points.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        1 2023-04-27 14:57:33.000000 geowatch-0.6.3/geowatch.egg-info/not-zip-safe
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18527 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/requires.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       15 2023-05-03 04:02:52.000000 geowatch-0.6.3/geowatch.egg-info/top_level.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2429 2023-04-29 23:47:47.000000 geowatch-0.6.3/pyproject.toml
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/requirements/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/cold.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      562 2023-05-03 00:21:52.000000 geowatch-0.6.3/requirements/development.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       19 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/dvc.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      445 2023-04-29 21:01:30.000000 geowatch-0.6.3/requirements/gdal.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      889 2023-04-03 19:39:09.000000 geowatch-0.6.3/requirements/graphics.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      979 2023-04-03 19:39:09.000000 geowatch-0.6.3/requirements/headless.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      110 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/linting.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2023-04-29 23:47:47.000000 geowatch-0.6.3/requirements/mmcv.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      318 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/optional.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9002 2023-05-03 00:21:52.000000 geowatch-0.6.3/requirements/runtime.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       86 2023-05-02 02:20:39.000000 geowatch-0.6.3/requirements/tensorflow.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       88 2023-04-29 21:01:30.000000 geowatch-0.6.3/requirements/tests.txt
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2023-04-29 21:01:30.000000 geowatch-0.6.3/requirements.txt
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      823 2023-04-03 19:39:09.000000 geowatch-0.6.3/run_tests.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       38 2023-05-03 04:02:52.957887 geowatch-0.6.3/setup.cfg
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10526 2023-05-03 00:21:52.000000 geowatch-0.6.3/setup.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/tests/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1271 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_cli.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2530 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_heterogeneous_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4038 2022-12-02 18:15:30.000000 geowatch-0.6.3/tests/test_init_from_pretrained.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2277 2023-03-21 17:57:36.000000 geowatch-0.6.3/tests/test_kwcoco_dataloader.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8409 2023-05-03 00:21:52.000000 geowatch-0.6.3/tests/test_lightning_cli_fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4446 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_load_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4367 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_mlops_scheduler.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7349 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_predict_latest_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4669 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_predict_old_fusion_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3440 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_predict_small_region.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6717 2023-04-29 21:01:30.000000 geowatch-0.6.3/tests/test_save_packages.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2514 2022-12-20 16:17:52.000000 geowatch-0.6.3/tests/test_sensor_metadata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13860 2023-04-29 23:47:47.000000 geowatch-0.6.3/tests/test_tracker.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      134 2022-06-07 15:49:12.000000 geowatch-0.6.3/tests/test_version.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.917887 geowatch-0.6.3/watch/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6332 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      139 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/__main__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.921887 geowatch-0.6.3/watch/cli/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       98 2023-01-18 16:43:36.000000 geowatch-0.6.3/watch/cli/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5685 2023-05-03 00:37:18.000000 geowatch-0.6.3/watch/cli/__main__.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7854 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/animate_visualizations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6116 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/cli/baseline_framework_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16017 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/cli/baseline_framework_ingress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6070 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_egress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3673 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_ingress.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10809 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/cluster_sites.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     6201 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/coco_add_watch_fields.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    95340 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/cli/coco_align.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      215 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/coco_align_geotiffs.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32128 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_average_features.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    34654 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_clean_geotiffs.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9577 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_combine_features.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22525 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_crop_tracks.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      224 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/coco_intensity_histograms.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10091 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_reformat_channels.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    11078 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_remove_bad_images.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2653 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_shard.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    32293 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/coco_spectra.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    44062 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/coco_time_combine.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4771 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/coco_update_geotiff_metadata.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    61339 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/coco_visualize_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1814 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/concat_kwcoco_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15924 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/crop_sites_to_regions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/cli/dag_cli/
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)       89 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/__init__.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15320 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/dag_cli/run_bas_datagen.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    13342 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_bas_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10286 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_dino_sv.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6939 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3529 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/run_pseudolive_consolidate.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     3062 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/run_psuedolive_copy_previous.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     7796 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_sc_datagen.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12667 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/cli/dag_cli/run_sc_fusion.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6224 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/cli/dag_cli/run_sv_datagen.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5581 2023-04-03 20:48:44.000000 geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_invariants.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5448 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_landcover.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11711 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/cli/extend_sc_sites.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4586 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/find_dvc.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    12269 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/geojson_site_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14799 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/geotiffs_to_kwcoco.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10815 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/cli/gifify.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    60306 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/kwcoco_to_geojson.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4375 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/cli/merge_region_models.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      209 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/mlops_cli.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    10349 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/prepare_splits.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    38053 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/prepare_ta2_dataset.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    29934 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/prepare_teamfeats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14855 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/cli/pseudolive_consolidate.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    69727 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/cli/reproject_annotations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       84 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/cli/run_fusion_predict.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    20415 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/run_metrics_framework.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)      271 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/cli/run_tracker.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4224 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/split_videos.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22737 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/stac_search.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    27798 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/cli/ta1_stac_to_kwcoco.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     9391 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/torch_model_stats.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16252 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/cli/validate_annotation_schemas.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)    15553 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/cli/watch_coco_stats.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2624 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20892 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/demo/demo_region.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      563 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/demo/dummy_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7543 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/landsat_demodata.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/demo/metrics_demo/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      138 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/demo/metrics_demo/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7448 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/demo/metrics_demo/demo_rendering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24604 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/demo/metrics_demo/demo_truth.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13005 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/metrics_demo/demo_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6307 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/metrics_demo/generate_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15545 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/demo/metrics_demo/site_perterbing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29938 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/demo/nitf_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3676 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/demo/sentinel2_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25225 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/demo/smart_kwcoco_demodata.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4089 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/demo/stac_demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      223 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/exceptions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/geoannots/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      989 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/geoannots/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2308 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/geoannots/geococo_objects.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16872 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/geoannots/geomodels.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/gis/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1645 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/gis/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9291 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/digital_globe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10020 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/gis/elevation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51299 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/geotiff.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.925887 geowatch-0.6.3/watch/gis/sensors/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      326 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/gis/sensors/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6516 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/sensors/sentinel2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13106 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/gis/spatial_reference.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26467 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/heuristics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/mlops/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      174 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/mlops/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      670 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70579 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70055 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/aggregate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17109 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/mlops/aggregate_loader.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23469 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/confusion_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25565 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/confusor_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40297 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/manager.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/mlops/old/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/mlops/old/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18067 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/old/expt_manager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39383 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/old/expt_report.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44820 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/old/expt_state.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39219 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/old/old_pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10290 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/mlops/old/old_plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8717 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/mlops/old/pipeline_v1.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39647 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/old/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55208 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/pipeline_nodes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12686 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/mlops/repackager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16868 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/mlops/schedule_evaluation.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22712 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/mlops/smart_global_helper.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32124 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/mlops/smart_pipeline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33368 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/mlops/smart_result_parser.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/monkey/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       62 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4095 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/_monkey_fbeta.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4047 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/monkey/monkey_albumentations.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      280 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/monkey_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1187 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/monkey/monkey_lightning.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       68 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/monkey/monkey_numpy.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      180 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/monkey_pil.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      207 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/monkey/monkey_tensorflow.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/monkey/monkey_torch.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      601 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/monkey/monkey_torchmetrics.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/rc/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1715 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/rc/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9626 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/rc/registry.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/stac/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       66 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/stac/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17312 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/stac/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14251 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/stac/stac_search_builder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9733 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/stac/util_stac.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/tasks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1677 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.929887 geowatch-0.6.3/watch/tasks/cold/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/cold/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17557 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/cold/assemble_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21171 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/cold/export_change_map.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18314 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/cold/export_cold_result_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17004 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/tasks/cold/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    73485 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/cold/prepare_ard.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23475 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/cold/prepare_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30062 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/cold/tile_processing.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28290 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/cold/tile_processing_kwcoco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/depth/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/__init__.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4501 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/backbone.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6559 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/config.json
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6816 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/depth/datasets.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     4372 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/depth/demo_transform.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     8379 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/depth/dzyne_img_util.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      295 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/depth/modules_monkeypatch.py
+-rwxrwxr-x   0 joncrall  (1000) joncrall  (1000)     5239 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/depth/pl_highres_verify.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24371 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/depth/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5689 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/depth/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/depthPCD/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/tasks/depthPCD/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6700 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/tasks/depthPCD/model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      407 2023-05-01 19:59:37.000000 geowatch-0.6.3/watch/tasks/depthPCD/model_test.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20132 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/depthPCD/score_tracks.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/dino_detector/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/dino_detector/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24608 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/dino_detector/building_validator.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10562 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/dino_detector/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/fusion/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2501 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/fusion/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       72 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/fusion/__main__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    82304 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/aggregate_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.933887 geowatch-0.6.3/watch/tasks/fusion/architectures/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      233 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11883 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/segmenter_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5979 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/sits.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    51015 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4989 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6302 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/architectures/wu_mae.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    36730 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/coco_stitcher.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/fusion/datamodules/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      336 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9680 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48055 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/batch_visualization.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8458 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/data_augment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18677 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/data_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9780 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/demos_for_slides.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    29470 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_datamodule.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   149541 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      373 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_video_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23364 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/qa_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14225 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/smart_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    53890 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/spacetime_grid_builder.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1527 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10375 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    44675 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       44 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/exceptions.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9422 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/plots.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    39631 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3384 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7352 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    55018 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/evaluate.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28542 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19157 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/fusion/fit_lightning.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/fusion/methods/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      741 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/fusion/methods/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    81666 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/methods/channelwise_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    79880 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/methods/heterogeneous.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25464 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/network_modules.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8960 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/noop_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    28643 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/unet_baseline.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32192 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/methods/watch_module_mixins.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4468 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/fusion/organize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61763 2023-05-03 04:02:03.000000 geowatch-0.6.3/watch/tasks/fusion/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14896 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/fusion/production.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16789 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/fusion/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/invariants/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/invariants/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13603 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/change.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/invariants/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35389 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20577 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/multi_image_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25778 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/data/other_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5589 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/invariants/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4483 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/fit_segment.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6709 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/invariants/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24584 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/invariants/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15963 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/invariants/pretext_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12941 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/invariants/segmentation_model.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/landcover/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/landcover/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6028 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5623 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/detector.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      103 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/landcover/fit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2377 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/model_info.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2360 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/tasks/landcover/nets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12281 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/landcover/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      349 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/landcover/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/metrics/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/metrics/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26517 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/tasks/metrics/merge_iarpa_metrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11867 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/metrics/viz_sc_results.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.937887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8025 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33579 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    31719 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19805 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    34195 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    22473 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9162 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/apnb.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5007 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/base_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8375 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/discritizers.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4272 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1276 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3510 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7979 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5652 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16573 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2864 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11476 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6888 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15931 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3732 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/self_attention.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6771 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3779 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1833 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9772 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    24297 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/timesformer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6020 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8684 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4982 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/vit.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10698 2022-08-09 13:10:41.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9087 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict_sc.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      115 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_config.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10512 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_misc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2112 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1508 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_paths.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9883 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.941887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3274 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11109 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4313 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/deepglobe.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5959 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/hrscd.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13129 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8257 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6702 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/inria.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3910 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2_self.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3309 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2mcp.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4659 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6266 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3830 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/sysucd.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.945887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42088 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19562 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    26483 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    52228 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    40645 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17085 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    46366 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    42111 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45628 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/iarpa_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    45044 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16504 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21771 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10831 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4437 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    61390 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    49788 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    65883 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    78136 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56648 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    70057 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67609 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    66954 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30059 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/setr_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    32133 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    35336 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48335 2023-04-19 20:35:11.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7030 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    60321 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)       70 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1466 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7650 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/canny_edge.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13281 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17807 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplabWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13507 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab_diff.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2845 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/encoding.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3794 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/gci.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      658 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/linear_classifier.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11714 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/losses.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5727 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/moco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9085 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/quantizer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11438 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7592 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnetGNWS.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12182 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    19182 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_enc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1414 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/sg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4967 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/shallow_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7222 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/supcon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4278 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/tex_refine.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12022 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6462 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_seg.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    33755 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14703 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_patchwise.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14964 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_test.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1884 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3932 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5761 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3861 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/cva.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12756 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/eval_utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13993 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9925 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/visualization.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1728 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7209 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11244 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11762 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      446 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5883 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6146 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/sam/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/tasks/sam/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    17730 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/sam/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/tracking/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1582 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/tracking/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    58501 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/from_heatmap.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2904 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/from_polygon.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    30472 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/normalize.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21464 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/tasks/tracking/phase.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23668 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/tasks/tracking/utils.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7531 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/tasks/tracking/visualize.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15495 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/drop0_datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3118 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/fit.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      175 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5614 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/resnets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5466 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10027 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet_blur.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8395 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/predict.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/__init__.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2057 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.949887 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)        0 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2093 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16199 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/datasets.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5987 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_S7.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4070 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_module.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      594 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/tasks/uky_temporal_prediction/utils.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.953887 geowatch-0.6.3/watch/utils/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2803 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12992 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/configargparse_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    48556 2023-02-02 14:12:29.000000 geowatch-0.6.3/watch/utils/ext_monai.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11626 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/ijson_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)   116465 2023-05-02 20:05:02.000000 geowatch-0.6.3/watch/utils/kwcoco_extensions.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.957887 geowatch-0.6.3/watch/utils/lightning_ext/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      376 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/lightning_ext/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    21356 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    20330 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7034 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/argparse_ext.py
+drwxrwxr-x   0 joncrall  (1000) joncrall  (1000)        0 2023-05-03 04:02:52.957887 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1244 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/__init__.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5735 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/auto_resumer.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8793 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/batch_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10112 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/packager.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2693 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/state_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    16120 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13026 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/callbacks/text_logger.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     4371 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/lightning_ext/demo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3211 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/lightning_ext/lightning_cli_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      199 2022-12-14 20:49:53.000000 geowatch-0.6.3/watch/utils/lightning_ext/monkeypatches.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7558 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/lightning_ext/old_parser_devices.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5712 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/lightning_ext/util_device.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      303 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/lightning_ext/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      434 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/lightning_ext/util_model.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10606 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/partial_format.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    11208 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/process_context.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    56465 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/result_analysis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5456 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/reverse_hashid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13733 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/simple_dvc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8514 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/slugify_ext.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41201 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_bands.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1059 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/util_codes.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12129 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/utils/util_data.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7144 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_dotdict.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1813 2023-02-27 18:47:15.000000 geowatch-0.6.3/watch/utils/util_environ.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2733 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_eval.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7920 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/util_framework.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    47570 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_gdal.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     6368 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_girder.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    43860 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_gis.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2747 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/utils/util_globals.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2039 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_hardware.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2589 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/util_iter.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3455 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_json.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    41820 2023-05-01 17:33:03.000000 geowatch-0.6.3/watch/utils/util_kwarray.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    67297 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_kwimage.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    14504 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_kwplot.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3771 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_locks.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     8978 2022-12-14 20:49:04.000000 geowatch-0.6.3/watch/utils/util_logging.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1035 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_nesting.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    12514 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_netharn.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10172 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_nvidia.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    10275 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_pandas.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     5746 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_parallel.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    25992 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/utils/util_param_grid.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    18404 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_path.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13282 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_pattern.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    23235 2023-04-29 21:01:30.000000 geowatch-0.6.3/watch/utils/util_progress.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    15872 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_raster.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3028 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_regex.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7614 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/util_resolution.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3542 2023-05-02 02:20:39.000000 geowatch-0.6.3/watch/utils/util_resources.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     3083 2022-06-07 15:49:12.000000 geowatch-0.6.3/watch/utils/util_rgdc.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)      570 2022-12-02 18:15:30.000000 geowatch-0.6.3/watch/utils/util_s3.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     7307 2023-03-21 17:57:36.000000 geowatch-0.6.3/watch/utils/util_stringalgo.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)    13699 2023-04-03 19:39:09.000000 geowatch-0.6.3/watch/utils/util_time.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     1786 2022-12-20 16:17:52.000000 geowatch-0.6.3/watch/utils/util_torchmetrics.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     2133 2023-05-03 00:21:52.000000 geowatch-0.6.3/watch/utils/util_windows.py
+-rw-rw-r--   0 joncrall  (1000) joncrall  (1000)     9413 2023-04-29 23:47:47.000000 geowatch-0.6.3/watch/utils/util_yaml.py
```

### Comparing `geowatch-0.6.2/CHANGELOG.md` & `geowatch-0.6.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/Dockerfile` & `geowatch-0.6.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/LICENSE` & `geowatch-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/PKG-INFO` & `geowatch-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geowatch
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://gitlab.kitware.com/computer-vision/geowatch.git
 Author: GEOWATCH developers
 Author-email: kitware@kitware.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `geowatch-0.6.2/README.rst` & `geowatch-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/conda_env.yml` & `geowatch-0.6.3/conda_env.yml`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/README.rst` & `geowatch-0.6.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/algorithms/fusion_overview.rst` & `geowatch-0.6.3/docs/algorithms/fusion_overview.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/algorithms/sensorchan_specs.rst` & `geowatch-0.6.3/docs/algorithms/sensorchan_specs.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/algorithms/ta2_deep_dive_info.md` & `geowatch-0.6.3/docs/algorithms/ta2_deep_dive_info.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/data/access_dvc_repos.rst` & `geowatch-0.6.3/docs/data/access_dvc_repos.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/data/internal_resources.rst` & `geowatch-0.6.3/docs/data/internal_resources.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/data/using_smartwatch_dvc.rst` & `geowatch-0.6.3/docs/data/using_smartwatch_dvc.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/debugging/debugging_cmdqueue.rst` & `geowatch-0.6.3/docs/debugging/debugging_cmdqueue.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/development/coding_conventions.rst` & `geowatch-0.6.3/docs/development/coding_conventions.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/development/coding_tips.rst` & `geowatch-0.6.3/docs/development/coding_tips.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/development/contribution_instructions.rst` & `geowatch-0.6.3/docs/development/contribution_instructions.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/development/rebasing_procedure.rst` & `geowatch-0.6.3/docs/development/rebasing_procedure.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/development/ta2_feature_integration.md` & `geowatch-0.6.3/docs/development/ta2_feature_integration.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/getting_started_aws.rst` & `geowatch-0.6.3/docs/environment/getting_started_aws.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/getting_started_dvc.rst` & `geowatch-0.6.3/docs/environment/getting_started_dvc.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/getting_started_kubectl.rst` & `geowatch-0.6.3/docs/environment/getting_started_kubectl.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/getting_started_ssh_keys.rst` & `geowatch-0.6.3/docs/environment/getting_started_ssh_keys.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/install_python.rst` & `geowatch-0.6.3/docs/environment/install_python.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/install_python_conda.rst` & `geowatch-0.6.3/docs/environment/install_python_conda.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/install_python_pyenv.rst` & `geowatch-0.6.3/docs/environment/install_python_pyenv.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/installing_geowatch.rst` & `geowatch-0.6.3/docs/environment/installing_geowatch.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/environment/windows.rst` & `geowatch-0.6.3/docs/environment/windows.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 It is recommened to be in a virtual enviornment
 
 .. code:: bash
 
    conda create -n geowatch python=3.10 -y
    conda activate geowatch
 
-   conda install gdal jq scikit-learn ffmpeg -c conda-forge -y
+   conda install gdal jq scikit-learn ffmpeg curl -c conda-forge -y
 
    # If you don't have a GPU
    conda install pytorch torchvision cpuonly -c pytorch -y
 
    # If you have a NVIDIA GPU (untested)
    conda install pytorch torchvision pytorch-cuda=11.8 -c pytorch nvidia -y
 
@@ -97,22 +97,21 @@
 
 The bash tutorial lives `here
 <https://gitlab.kitware.com/computer-vision/geowatch/-/blob/main/tutorial/tutorial1_rgb_network.sh>`_,
 and can be downloaded and run via:
 
 .. code:: bash
 
-    conda install curl
     curl -LJO https://gitlab.kitware.com/computer-vision/geowatch/-/raw/main/tutorial/tutorial1_rgb_network.sh
 
     # Show the tutorial (it's readable)
     cat tutorial1_rgb_network.sh
 
     # The tutorial is self-executing.
-    ./tutorial1_rgb_network.sh
+    source tutorial1_rgb_network.sh
 
 
 OR if you cloned the source repo:
 
 .. code:: bash
 
     cd geowatch
```

### Comparing `geowatch-0.6.2/docs/misc/structure_proposal.md` & `geowatch-0.6.3/docs/misc/structure_proposal.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/misc/supporting_projects.rst` & `geowatch-0.6.3/docs/misc/supporting_projects.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/mlops.md` & `geowatch-0.6.3/docs/mlops.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/onboarding.rst` & `geowatch-0.6.3/docs/onboarding.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/smartflow/getting_started_smartflow.rst` & `geowatch-0.6.3/docs/smartflow/getting_started_smartflow.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/smartflow/smartflow_copying_large_files_to_efs.md` & `geowatch-0.6.3/docs/smartflow/smartflow_copying_large_files_to_efs.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/smartflow/smartflow_running_the_system.rst` & `geowatch-0.6.3/docs/smartflow/smartflow_running_the_system.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/smartflow/smartflow_training_fusion_models.md` & `geowatch-0.6.3/docs/smartflow/smartflow_training_fusion_models.md`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/testing/running_ci_locally.rst` & `geowatch-0.6.3/docs/testing/running_ci_locally.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/testing/testing_practices.rst` & `geowatch-0.6.3/docs/testing/testing_practices.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/docs/watch_cli.rst` & `geowatch-0.6.3/docs/watch_cli.rst`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/geowatch.egg-info/PKG-INFO` & `geowatch-0.6.3/geowatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geowatch
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://gitlab.kitware.com/computer-vision/geowatch.git
 Author: GEOWATCH developers
 Author-email: kitware@kitware.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `geowatch-0.6.2/geowatch.egg-info/SOURCES.txt` & `geowatch-0.6.3/geowatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/geowatch.egg-info/requires.txt` & `geowatch-0.6.3/geowatch.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/pyproject.toml` & `geowatch-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/requirements/development.txt` & `geowatch-0.6.3/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/requirements/graphics.txt` & `geowatch-0.6.3/requirements/graphics.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/requirements/headless.txt` & `geowatch-0.6.3/requirements/headless.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/requirements/runtime.txt` & `geowatch-0.6.3/requirements/runtime.txt`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/run_tests.py` & `geowatch-0.6.3/run_tests.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/setup.py` & `geowatch-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_cli.py` & `geowatch-0.6.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_heterogeneous_model.py` & `geowatch-0.6.3/tests/test_heterogeneous_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_init_from_pretrained.py` & `geowatch-0.6.3/tests/test_init_from_pretrained.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_kwcoco_dataloader.py` & `geowatch-0.6.3/tests/test_kwcoco_dataloader.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_lightning_cli_fit.py` & `geowatch-0.6.3/tests/test_lightning_cli_fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_load_models.py` & `geowatch-0.6.3/tests/test_load_models.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_mlops_scheduler.py` & `geowatch-0.6.3/tests/test_mlops_scheduler.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_predict_latest_models.py` & `geowatch-0.6.3/tests/test_predict_latest_models.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_predict_old_fusion_model.py` & `geowatch-0.6.3/tests/test_predict_old_fusion_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_predict_small_region.py` & `geowatch-0.6.3/tests/test_predict_small_region.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_save_packages.py` & `geowatch-0.6.3/tests/test_save_packages.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_sensor_metadata.py` & `geowatch-0.6.3/tests/test_sensor_metadata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/tests/test_tracker.py` & `geowatch-0.6.3/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/__init__.py` & `geowatch-0.6.3/watch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import os
 import sys
 import ubelt as ub
 import warnings
 
 
-__version__ = '0.6.2'
+__version__ = '0.6.3'
 
 
 # ~/code/watch/dev/maintain/generate_authors.py
 __author__ = 'GEOWATCH Developers, Kitware Inc., Jon Crall, David Joy, Matthew Bernstein, Connor Greenwell, Benjamin Brodie, Peri Akiva, Usman Rafique, Jacob DeRosa, Matthew Purri, Ajay Upadhyaya, Ji Won Suh, Jacob Birge, Ryan LaClair, Scott Workman, Dexter Lau, Sergii Skakun, Aram Ansary Ogholbake, Cohen Archbold, Bane Sullivan, Srikumar Sastry, Armin Hadzic'
 
 __author_email__ = 'kitware@kitware.com, jon.crall@kitware.com'
 __url__ = 'https://gitlab.kitware.com/computer-vision/geowatch'
```

### Comparing `geowatch-0.6.2/watch/cli/__main__.py` & `geowatch-0.6.3/watch/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,18 @@
 
     import os
     from scriptconfig.modal import ModalCLI
     import watch
     WATCH_LOOSE_CLI = os.environ.get('WATCH_LOOSE_CLI', '')
 
     # https://emojiterra.com/time/
+    # Not sure how to make this consistent on different terminals
     fun_header = ub.codeblock(
         '''
-        🛰️ ⌚🛰️           🧠       🛰️ ⌚🛰️
+        🛰️⌚🛰️           🧠       🛰️⌚🛰️
         🌍🌎🌏        👁️   👁️      🌏🌎🌍
         ''')
 
     boring_description =  ub.codeblock(
         f'''
         🌐🌐🌐 The GEO-WATCH CLI 🌐🌐🌐
 
@@ -99,15 +100,15 @@
         segmentation and detection with geospatial awareness.
 
         Developed by [link=https://www.kitware.com/]Kitware[/link]. Funded by the [link=https://www.iarpa.gov/research-programs/smart]IARPA SMART[/link] challenge.
 
         Version: {watch.__version__}
         ''')
 
-    FUN = (os.getenv('FUN', '') or 1) and not os.getenv('NOFUN', '')
+    FUN = os.getenv('FUN', '1') and not os.getenv('NOFUN', '')
     if FUN:
         description = fun_header + '\n' + boring_description
     else:
         description = boring_description
 
     modal = ModalCLI(description)
```

### Comparing `geowatch-0.6.2/watch/cli/animate_visualizations.py` & `geowatch-0.6.3/watch/cli/animate_visualizations.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/baseline_framework_egress.py` & `geowatch-0.6.3/watch/cli/baseline_framework_egress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/baseline_framework_ingress.py` & `geowatch-0.6.3/watch/cli/baseline_framework_ingress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/baseline_framework_kwcoco_egress.py` & `geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_egress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/baseline_framework_kwcoco_ingress.py` & `geowatch-0.6.3/watch/cli/baseline_framework_kwcoco_ingress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/cluster_sites.py` & `geowatch-0.6.3/watch/cli/cluster_sites.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_add_watch_fields.py` & `geowatch-0.6.3/watch/cli/coco_add_watch_fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,29 @@
 and image processing. Note a video GSD will typically be much higher (i.e.
 lower resolution) than an image GSD.
 """
 import ubelt as ub
 import scriptconfig as scfg
 
 
-class AddWatchFieldsConfig(scfg.Config):
+class AddWatchFieldsConfig(scfg.DataConfig):
     """
     Updates image transforms in a kwcoco json file to align all videos to a
     target GSD.
     """
     __default__ = {
         'src': scfg.Value('data.kwcoco.json', help='input kwcoco filepath', position=1),
 
         'dst': scfg.Value(None, help='output kwcoco filepath', position=2),
 
+        'inplace': scfg.Value(False, isflag=True, help=ub.paragraph(
+            '''
+            if True and dst is unspecified then the output will overwrite the input
+            ''')),
+
         'target_gsd': scfg.Value(10.0, help='compute transforms for a target gsd'),
 
         'overwrite': scfg.Value(False, help='if True overwrites introspectable fields'),
 
         'edit_geotiff_metadata': scfg.Value(False, help='if True MODIFIES THE UNDERLYING IMAGES to ensure geodata is propogated'),
 
         'default_gsd': scfg.Value(None, help='if specified, assumed any images without geo-metadata have this GSD'),
@@ -97,14 +102,20 @@
     import kwcoco
     import kwimage
     from watch.utils import util_parallel
     from watch.utils import kwcoco_extensions
     config = AddWatchFieldsConfig(kwargs, cmdline=cmdline)
     print('config = {}'.format(ub.urepr(dict(config), nl=1)))
 
+    if config['dst'] is None:
+        if config['inplace']:
+            config['dst'] = config['dst'] = config['src']
+        else:
+            raise ValueError('must specify dst: {}'.format(config['dst']))
+
     print('read dataset')
     dset = kwcoco.CocoDataset.coerce(config['src'])
     print('dset = {!r}'.format(dset))
 
     # valid_gids = kwcoco_extensions.filter_image_ids(
     #     dset,
     #     include_sensors=config['include_sensors'],
```

### Comparing `geowatch-0.6.2/watch/cli/coco_align.py` & `geowatch-0.6.3/watch/cli/coco_align.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_average_features.py` & `geowatch-0.6.3/watch/cli/coco_average_features.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_clean_geotiffs.py` & `geowatch-0.6.3/watch/cli/coco_clean_geotiffs.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_combine_features.py` & `geowatch-0.6.3/watch/cli/coco_combine_features.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_crop_tracks.py` & `geowatch-0.6.3/watch/cli/coco_crop_tracks.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_reformat_channels.py` & `geowatch-0.6.3/watch/cli/coco_reformat_channels.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_remove_bad_images.py` & `geowatch-0.6.3/watch/cli/coco_remove_bad_images.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_shard.py` & `geowatch-0.6.3/watch/cli/coco_shard.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_spectra.py` & `geowatch-0.6.3/watch/cli/coco_spectra.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_time_combine.py` & `geowatch-0.6.3/watch/cli/coco_time_combine.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,19 +154,19 @@
     spatial_tile_size = scfg.Value(None, help=ub.paragraph(
         '''
             The size of the tiling over space to use when computing the average.
             If None, the average is computed on the entire stack of images at
             once.
         '''))
 
-    filter_season = scfg.Value(None, help=ub.paragraph(
+    filter_season = scfg.Value([], nargs='+', help=ub.paragraph(
         '''
             Images within this season(s) will be excluded from the average operation.
             Season options: ['spring', 'summer', 'fall', 'winter']
-        '''))
+        '''), alias=['remove_seasons'])
 
 
 def main(cmdline=1, **kwargs):
     """
     CommandLine:
         DEVEL_TEST=1 xdoctest -m watch.cli.coco_time_combine main
 
@@ -464,15 +464,14 @@
     import kwcoco
     import numpy as np
     from watch.utils import util_progress
     from watch.utils import util_time
     from watch.utils import kwcoco_extensions
     from watch.utils import util_parallel
     from watch.utils.util_yaml import Yaml
-    from watch.tasks.rutgers_material_seg_v2.utils.util_misc import filter_image_ids_by_season
     # Check inputs.
 
     space = 'video'
 
     workers = util_parallel.coerce_num_workers(config.workers)
 
     ## Check input kwcoco file path exists.
@@ -984,14 +983,75 @@
                                     scale_asset_from_stitchspace=scale_asset_from_vid)
     stitch_manager.finalize_image(gid)
     final_img = tmp_dset.imgs[gid]
 
     return final_img
 
 
+def filter_image_ids_by_season(coco_dset, image_ids, filtered_seasons):
+    from watch.utils import util_time
+    hemipshere_to_season_map = {
+        'northern': {
+            'spring': [3, 4, 5],
+            'summer': [6, 7, 8],
+            'fall': [9, 10, 11],
+            'winter': [12, 1, 2]
+        },
+        'southern': {
+            'spring': [9, 10, 11],
+            'summer': [12, 1, 2],
+            'fall': [3, 4, 5],
+            'winter': [6, 7, 8]
+        }
+    }
+
+    if len(image_ids) == 0:
+        print('WARNING: No images to filter.')
+        return []
+
+    if not isinstance(filtered_seasons, list):
+        filtered_seasons = [filtered_seasons]
+
+    filtered_seasons = set(filtered_seasons)
+    valid_seasons = {'spring', 'summer', 'fall', 'winter'}
+
+    invalid_seasons = filtered_seasons - valid_seasons
+    if invalid_seasons:
+        raise ValueError(f'Invalid seasons: {invalid_seasons}')
+
+    # Get hemisphere of region.
+    coco_img = coco_dset.coco_image(image_ids[0])
+    lon, _ = coco_img.img['geos_corners']['coordinates'][0][0]
+
+    if lon > 0:
+        hemisphere = 'northern'
+    else:
+        hemisphere = 'southern'
+
+    month_to_season_map = {}
+    for season, months in hemipshere_to_season_map[hemisphere].items():
+        for month in months:
+            month_to_season_map[month] = season
+
+    final_image_ids = []
+    for image_id in image_ids:
+        coco_img = coco_dset.coco_image(image_id)
+
+        # Get month.
+        dt = util_time.coerce_datetime(coco_img['date_captured'])
+        month = dt.month
+
+        # Get season of month.
+        img_season = month_to_season_map[month]
+        if img_season not in filtered_seasons:
+            final_image_ids.append(image_id)
+
+    return final_image_ids
+
+
 __config__ = TimeCombineConfig
 
 if __name__ == '__main__':
     """
 
     CommandLine:
         python -m watch.cli.coco_time_combine
```

### Comparing `geowatch-0.6.2/watch/cli/coco_update_geotiff_metadata.py` & `geowatch-0.6.3/watch/cli/coco_update_geotiff_metadata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/coco_visualize_videos.py` & `geowatch-0.6.3/watch/cli/coco_visualize_videos.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,14 +372,16 @@
                     keep.append(coco_img.img['id'])
             else:
                 if requested_channels & code:
                     keep.append(coco_img.img['id'])
         rich.print(f'Filtered {len(coco_images) - len(keep)} images without requested channels. Keeping {len(keep)}')
         selected_gids = keep
 
+    rich.print(f'Will write to: [link={viz_dpath}]{viz_dpath}[/link]')
+
     video_names = []
     for vidid, video in prog:
 
         sub_dpath = viz_dpath / video['name']
 
         gids = coco_dset.index.vidid_to_gids[vidid]
         if selected_gids is not None:
```

### Comparing `geowatch-0.6.2/watch/cli/concat_kwcoco_videos.py` & `geowatch-0.6.3/watch/cli/concat_kwcoco_videos.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/crop_sites_to_regions.py` & `geowatch-0.6.3/watch/cli/crop_sites_to_regions.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_bas_datagen.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_bas_datagen.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_bas_fusion.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_bas_fusion.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_dino_sv.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_dino_sv.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_dzyne_parallel_site_vali.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_pseudolive_consolidate.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_pseudolive_consolidate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_psuedolive_copy_previous.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_psuedolive_copy_previous.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_sc_datagen.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_sc_datagen.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_sc_fusion.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_sc_fusion.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_sv_datagen.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_sv_datagen.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_teamfeat_invariants.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_invariants.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/dag_cli/run_teamfeat_landcover.py` & `geowatch-0.6.3/watch/cli/dag_cli/run_teamfeat_landcover.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/extend_sc_sites.py` & `geowatch-0.6.3/watch/cli/extend_sc_sites.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/find_dvc.py` & `geowatch-0.6.3/watch/cli/find_dvc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/geojson_site_stats.py` & `geowatch-0.6.3/watch/cli/geojson_site_stats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/geotiffs_to_kwcoco.py` & `geowatch-0.6.3/watch/cli/geotiffs_to_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/gifify.py` & `geowatch-0.6.3/watch/cli/gifify.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/kwcoco_to_geojson.py` & `geowatch-0.6.3/watch/cli/kwcoco_to_geojson.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/merge_region_models.py` & `geowatch-0.6.3/watch/cli/merge_region_models.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/prepare_splits.py` & `geowatch-0.6.3/watch/cli/prepare_splits.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/prepare_ta2_dataset.py` & `geowatch-0.6.3/watch/cli/prepare_ta2_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/prepare_teamfeats.py` & `geowatch-0.6.3/watch/cli/prepare_teamfeats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/pseudolive_consolidate.py` & `geowatch-0.6.3/watch/cli/pseudolive_consolidate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/reproject_annotations.py` & `geowatch-0.6.3/watch/cli/reproject_annotations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -201,24 +201,24 @@
         >>>     'workers': 4,
         >>>     'io_workers': 8,
         >>>     'site_models': dvc_dpath / 'annotations/drop6/site_models/KR_R001*',
         >>>     'region_models': dvc_dpath / 'annotations/drop6/region_models/KR_R001*',
         >>> }
         >>> main(cmdline=cmdline, **kwargs)
     """
+    config = ReprojectAnnotationsConfig.cli(data=kwargs, cmdline=cmdline)
     import geopandas as gpd  # NOQA
     from watch.utils import util_gis
     from watch.utils import util_parallel
     from watch.utils.util_yaml import Yaml
     from watch import heuristics
     from watch.utils import kwcoco_extensions
     import kwcoco
     import rich
     import numpy as np
-    config = ReprojectAnnotationsConfig.cli(data=kwargs, cmdline=cmdline)
     rich.print('config = {}'.format(ub.urepr(config, nl=1)))
 
     output_fpath = config['dst']
     if output_fpath is None:
         if config['inplace']:
             output_fpath = config['dst'] = config['src']
         else:
```

### Comparing `geowatch-0.6.2/watch/cli/run_metrics_framework.py` & `geowatch-0.6.3/watch/cli/run_metrics_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/split_videos.py` & `geowatch-0.6.3/watch/cli/split_videos.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/stac_search.py` & `geowatch-0.6.3/watch/cli/stac_search.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/ta1_stac_to_kwcoco.py` & `geowatch-0.6.3/watch/cli/ta1_stac_to_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/torch_model_stats.py` & `geowatch-0.6.3/watch/cli/torch_model_stats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/validate_annotation_schemas.py` & `geowatch-0.6.3/watch/cli/validate_annotation_schemas.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/cli/watch_coco_stats.py` & `geowatch-0.6.3/watch/cli/watch_coco_stats.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/__init__.py` & `geowatch-0.6.3/watch/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/demo_region.py` & `geowatch-0.6.3/watch/demo/demo_region.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/dummy_demodata.py` & `geowatch-0.6.3/watch/demo/dummy_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/landsat_demodata.py` & `geowatch-0.6.3/watch/demo/landsat_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/metrics_demo/demo_rendering.py` & `geowatch-0.6.3/watch/demo/metrics_demo/demo_rendering.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/metrics_demo/demo_truth.py` & `geowatch-0.6.3/watch/demo/metrics_demo/demo_truth.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/metrics_demo/demo_utils.py` & `geowatch-0.6.3/watch/demo/metrics_demo/demo_utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/metrics_demo/generate_demodata.py` & `geowatch-0.6.3/watch/demo/metrics_demo/generate_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/metrics_demo/site_perterbing.py` & `geowatch-0.6.3/watch/demo/metrics_demo/site_perterbing.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/nitf_demodata.py` & `geowatch-0.6.3/watch/demo/nitf_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/sentinel2_demodata.py` & `geowatch-0.6.3/watch/demo/sentinel2_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/smart_kwcoco_demodata.py` & `geowatch-0.6.3/watch/demo/smart_kwcoco_demodata.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/demo/stac_demo.py` & `geowatch-0.6.3/watch/demo/stac_demo.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/geoannots/__init__.py` & `geowatch-0.6.3/watch/geoannots/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/geoannots/geococo_objects.py` & `geowatch-0.6.3/watch/geoannots/geococo_objects.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/geoannots/geomodels.py` & `geowatch-0.6.3/watch/geoannots/geomodels.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/gis/__init__.py` & `geowatch-0.6.3/watch/gis/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/gis/digital_globe.py` & `geowatch-0.6.3/watch/gis/digital_globe.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/gis/elevation.py` & `geowatch-0.6.3/watch/gis/elevation.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/gis/geotiff.py` & `geowatch-0.6.3/watch/gis/geotiff.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/gis/sensors/sentinel2.py` & `geowatch-0.6.3/watch/gis/sensors/sentinel2.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/gis/spatial_reference.py` & `geowatch-0.6.3/watch/gis/spatial_reference.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/heuristics.py` & `geowatch-0.6.3/watch/heuristics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/__main__.py` & `geowatch-0.6.3/watch/mlops/__main__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/_notebook.py` & `geowatch-0.6.3/watch/mlops/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/aggregate.py` & `geowatch-0.6.3/watch/mlops/aggregate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/aggregate_loader.py` & `geowatch-0.6.3/watch/mlops/aggregate_loader.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/confusion_visualization.py` & `geowatch-0.6.3/watch/mlops/confusion_visualization.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/confusor_analysis.py` & `geowatch-0.6.3/watch/mlops/confusor_analysis.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/manager.py` & `geowatch-0.6.3/watch/mlops/manager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/expt_manager.py` & `geowatch-0.6.3/watch/mlops/old/expt_manager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/expt_report.py` & `geowatch-0.6.3/watch/mlops/old/expt_report.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/expt_state.py` & `geowatch-0.6.3/watch/mlops/old/expt_state.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/old_pipeline_nodes.py` & `geowatch-0.6.3/watch/mlops/old/old_pipeline_nodes.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/old_plots.py` & `geowatch-0.6.3/watch/mlops/old/old_plots.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/pipeline_v1.py` & `geowatch-0.6.3/watch/mlops/old/pipeline_v1.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/old/plots.py` & `geowatch-0.6.3/watch/mlops/old/plots.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/pipeline_nodes.py` & `geowatch-0.6.3/watch/mlops/pipeline_nodes.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/repackager.py` & `geowatch-0.6.3/watch/mlops/repackager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/schedule_evaluation.py` & `geowatch-0.6.3/watch/mlops/schedule_evaluation.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/smart_global_helper.py` & `geowatch-0.6.3/watch/mlops/smart_global_helper.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/smart_pipeline.py` & `geowatch-0.6.3/watch/mlops/smart_pipeline.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/mlops/smart_result_parser.py` & `geowatch-0.6.3/watch/mlops/smart_result_parser.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/monkey/_monkey_fbeta.py` & `geowatch-0.6.3/watch/monkey/_monkey_fbeta.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/monkey/monkey_albumentations.py` & `geowatch-0.6.3/watch/monkey/monkey_albumentations.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/monkey/monkey_lightning.py` & `geowatch-0.6.3/watch/monkey/monkey_lightning.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/monkey/monkey_torch.py` & `geowatch-0.6.3/watch/monkey/monkey_torch.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/monkey/monkey_torchmetrics.py` & `geowatch-0.6.3/watch/monkey/monkey_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/rc/__init__.py` & `geowatch-0.6.3/watch/rc/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/rc/registry.py` & `geowatch-0.6.3/watch/rc/registry.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/stac/_notebook.py` & `geowatch-0.6.3/watch/stac/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/stac/stac_search_builder.py` & `geowatch-0.6.3/watch/stac/stac_search_builder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/stac/util_stac.py` & `geowatch-0.6.3/watch/stac/util_stac.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/__init__.py` & `geowatch-0.6.3/watch/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/assemble_cold_result_kwcoco.py` & `geowatch-0.6.3/watch/tasks/cold/assemble_cold_result_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/export_change_map.py` & `geowatch-0.6.3/watch/tasks/cold/export_change_map.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/export_cold_result_kwcoco.py` & `geowatch-0.6.3/watch/tasks/cold/export_cold_result_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/predict.py` & `geowatch-0.6.3/watch/tasks/cold/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,38 +103,68 @@
         --prob=0.99 \
         --conse=6 \
         --cm_interval=60 \
         --year_lowbound=None \
         --year_highbound=None \
         --coefs=cv,rmse,a0,a1,b1,c1 \
         --coefs_bands=0,1,2,3,4,5 \
-        --timestamp=False \
-        --combine=False \
+        --timestamp=True \
+        --combine=True \
         --resolution='10GSD' \
         --workermode='serial' \
         --workers=0
 
     kwcoco stats "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip
     geowatch stats "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip
 
     # Fix path problem because we wrote a different directory
     # TODO: fix this script so the output always uses absolute paths?
     # or at least doesn't write invalid data that needs fixing?
     DATA_DVC_DPATH=$(geowatch_dvc --tags=phase2_data --hardware="auto")
     kwcoco reroot \
         --src="$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip \
         --dst="$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold_fixed.kwcoco.zip \
+        --absolute=True
+
         --old_prefix="KR_R001" --new_prefix="../KR_R001"
 
     DATA_DVC_DPATH=$(geowatch_dvc --tags=phase2_data --hardware="auto")
+    kwcoco validate "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold_fixed.kwcoco.zip
+
     smartwatch visualize \
         "$DATA_DVC_DPATH"/Drop6-MeanYear10GSD-V2/imgonly_KR_R001_cold.kwcoco.zip \
         --channels="L8:(red|green|blue,red_COLD_a1|green_COLD_a1|blue_COLD_a1,red_COLD_cv|green_COLD_cv|blue_COLD_cv,red_COLD_rmse|green_COLD_rmse|blue_COLD_rmse)" \
         --smart=True
 
+    ####################
+    ### FULL REGION TEST V2
+    ####################
+
+    DATA_DVC_DPATH=$(smartwatch_dvc --tags=phase2_data --hardware="auto")
+    EXPT_DVC_DPATH=$(smartwatch_dvc --tags=phase2_expt --hardware="auto")
+    python -m watch.tasks.cold.predict \
+        --coco_fpath="$DATA_DVC_DPATH/Drop6/imgonly-KR_R001.kwcoco.json" \
+        --combined_coco_fpath="$DATA_DVC_DPATH/Drop6/imgonly-KR_R001.kwcoco.json" \
+        --out_dpath="$DATA_DVC_DPATH/Drop6/_pycold_combine" \
+        --sensors='L8' \
+        --adj_cloud=False \
+        --method='COLD' \
+        --prob=0.99 \
+        --conse=6 \
+        --cm_interval=60 \
+        --year_lowbound=None \
+        --year_highbound=None \
+        --coefs=cv,rmse,a0,a1,b1,c1 \
+        --coefs_bands=0,1,2,3,4,5 \
+        --timestamp=False \
+        --combine=False \
+        --resolution='10GSD' \
+        --workermode='serial' \
+        --workers=0
+
 
     ########################
     ### MULTIPLE REGION TEST
     ########################
     DVC_DATA_DPATH=$(geowatch_dvc --tags='phase2_data' --hardware=auto)
 
     echo "$DVC_DATA_DPATH"
```

### Comparing `geowatch-0.6.2/watch/tasks/cold/prepare_ard.py` & `geowatch-0.6.3/watch/tasks/cold/prepare_ard.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/prepare_kwcoco.py` & `geowatch-0.6.3/watch/tasks/cold/prepare_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/tile_processing.py` & `geowatch-0.6.3/watch/tasks/cold/tile_processing.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/cold/tile_processing_kwcoco.py` & `geowatch-0.6.3/watch/tasks/cold/tile_processing_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/backbone.py` & `geowatch-0.6.3/watch/tasks/depth/backbone.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/config.json` & `geowatch-0.6.3/watch/tasks/depth/config.json`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/datasets.py` & `geowatch-0.6.3/watch/tasks/depth/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/demo_transform.py` & `geowatch-0.6.3/watch/tasks/depth/demo_transform.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/dzyne_img_util.py` & `geowatch-0.6.3/watch/tasks/depth/dzyne_img_util.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/pl_highres_verify.py` & `geowatch-0.6.3/watch/tasks/depth/pl_highres_verify.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/predict.py` & `geowatch-0.6.3/watch/tasks/depth/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depth/utils.py` & `geowatch-0.6.3/watch/tasks/depth/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depthPCD/model.py` & `geowatch-0.6.3/watch/tasks/depthPCD/model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/depthPCD/score_tracks.py` & `geowatch-0.6.3/watch/tasks/depthPCD/score_tracks.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/dino_detector/building_validator.py` & `geowatch-0.6.3/watch/tasks/dino_detector/building_validator.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/dino_detector/predict.py` & `geowatch-0.6.3/watch/tasks/dino_detector/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/__init__.py` & `geowatch-0.6.3/watch/tasks/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/aggregate_results.py` & `geowatch-0.6.3/watch/tasks/fusion/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/architectures/segmenter_decoder.py` & `geowatch-0.6.3/watch/tasks/fusion/architectures/segmenter_decoder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/architectures/sits.py` & `geowatch-0.6.3/watch/tasks/fusion/architectures/sits.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/architectures/transformer.py` & `geowatch-0.6.3/watch/tasks/fusion/architectures/transformer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/architectures/unet_blur.py` & `geowatch-0.6.3/watch/tasks/fusion/architectures/unet_blur.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/architectures/wu_mae.py` & `geowatch-0.6.3/watch/tasks/fusion/architectures/wu_mae.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/coco_stitcher.py` & `geowatch-0.6.3/watch/tasks/fusion/coco_stitcher.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/_notebook.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/batch_visualization.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/batch_visualization.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/data_augment.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/data_augment.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/data_utils.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/data_utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/demos_for_slides.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/demos_for_slides.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/kwcoco_datamodule.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_datamodule.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/kwcoco_dataset.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/kwcoco_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/qa_bands.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/qa_bands.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/smart_mixins.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/smart_mixins.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/spacetime_grid_builder.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/spacetime_grid_builder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/_notebook.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/affinity.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/plots.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/plots.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/time_kernel_grammar.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/datamodules/temporal_sampling/utils.py` & `geowatch-0.6.3/watch/tasks/fusion/datamodules/temporal_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/evaluate.py` & `geowatch-0.6.3/watch/tasks/fusion/evaluate.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/fit.py` & `geowatch-0.6.3/watch/tasks/fusion/fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/fit_lightning.py` & `geowatch-0.6.3/watch/tasks/fusion/fit_lightning.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/__init__.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/channelwise_transformer.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/channelwise_transformer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/heterogeneous.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/network_modules.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/network_modules.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/noop_model.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/noop_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/unet_baseline.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/unet_baseline.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/methods/watch_module_mixins.py` & `geowatch-0.6.3/watch/tasks/fusion/methods/watch_module_mixins.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/organize.py` & `geowatch-0.6.3/watch/tasks/fusion/organize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/predict.py` & `geowatch-0.6.3/watch/tasks/fusion/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,20 +68,20 @@
         ...
 
 
 class PredictConfig(DataModuleConfigMixin):
     """
     Prediction script for the fusion task
     """
-    config_file = scfg.Value(None, alias=['config'], help='config file path')
-    write_out_config_file_to_this_path = scfg.Value(None, alias=['dump'], help=ub.paragraph(
-            '''
-            takes the current command line args and writes them out to a
-            config file at the given path, then exits
-            '''))
+    # config_file = scfg.Value(None, alias=['config'], help='config file path')
+    # write_out_config_file_to_this_path = scfg.Value(None, alias=['dump'], help=ub.paragraph(
+    #         '''
+    #         takes the current command line args and writes them out to a
+    #         config file at the given path, then exits
+    #         '''))
     datamodule = scfg.Value('KWCocoVideoDataModule', help='This must always be KWCocoVideoDataModule for now')
     pred_dataset = scfg.Value(None, help=ub.paragraph(
             '''
             path to the output dataset (note: test_dataset is the input
             dataset)
             '''))
     package_fpath = scfg.Value(None, type=str, help=None)
```

### Comparing `geowatch-0.6.2/watch/tasks/fusion/production.py` & `geowatch-0.6.3/watch/tasks/fusion/production.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/fusion/utils.py` & `geowatch-0.6.3/watch/tasks/fusion/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/change.py` & `geowatch-0.6.3/watch/tasks/invariants/change.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/data/datasets.py` & `geowatch-0.6.3/watch/tasks/invariants/data/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/data/multi_image_datasets.py` & `geowatch-0.6.3/watch/tasks/invariants/data/multi_image_datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/data/other_datasets.py` & `geowatch-0.6.3/watch/tasks/invariants/data/other_datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/fit.py` & `geowatch-0.6.3/watch/tasks/invariants/fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/fit_segment.py` & `geowatch-0.6.3/watch/tasks/invariants/fit_segment.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/iarpa_dataset.py` & `geowatch-0.6.3/watch/tasks/invariants/iarpa_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/predict.py` & `geowatch-0.6.3/watch/tasks/invariants/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/pretext_model.py` & `geowatch-0.6.3/watch/tasks/invariants/pretext_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/invariants/segmentation_model.py` & `geowatch-0.6.3/watch/tasks/invariants/segmentation_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/landcover/datasets.py` & `geowatch-0.6.3/watch/tasks/landcover/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/landcover/detector.py` & `geowatch-0.6.3/watch/tasks/landcover/detector.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/landcover/model_info.py` & `geowatch-0.6.3/watch/tasks/landcover/model_info.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/landcover/nets.py` & `geowatch-0.6.3/watch/tasks/landcover/nets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/landcover/predict.py` & `geowatch-0.6.3/watch/tasks/landcover/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/metrics/merge_iarpa_metrics.py` & `geowatch-0.6.3/watch/tasks/metrics/merge_iarpa_metrics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/metrics/viz_sc_results.py` & `geowatch-0.6.3/watch/tasks/metrics/viz_sc_results.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/__init__.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_kwdataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/iarpa_sc_kwdataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/datasets/peo_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/__init__.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/apnb.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/apnb.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/base_model.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/base_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/discritizers.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/discritizers.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/dynamic_unet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/early_fusion_mat_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/late_fusion_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/mat_ed_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/patch_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/peri_resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/pos_embedding.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/resnet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/self_attention.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/self_attention.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_feature_diff_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/siamese_fusion_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/simple_decoder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/timesformer.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/timesformer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/unet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/unet_lstm.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/models/vit.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/models/vit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/predict.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/predict_sc.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/predict_sc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_misc.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_misc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_model.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_paths.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_paths.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_change_detection/utils/util_visualize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/__init__.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/bigearthnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/deepglobe.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/deepglobe.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/dynamicearthnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/hrscd.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/hrscd.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_contrastive_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/iarpa_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/inria.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/inria.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/s2_self.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2_self.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/s2mcp.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/s2mcp.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/spacenet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/spacenet2.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/spacenet2.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/datasets/sysucd.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/datasets/sysucd.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/bigearthnet_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/change_vector_analysis.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/cluster_labeling.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/compare_vw_maps.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/deepglobe_train_val.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/dynamicearthnet_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/evaluation_method_comparison.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/hrscd_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/iarpa_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/inria_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/moco_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/moco_unsupervised_material.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/mt_material_clustering_tranfer_learn.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/multi_temporal_material_clustering.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_fine_tune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_finetune2.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_patch_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/onera_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/onera_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_net.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/pretrain_contrastive_resnet_enc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/setr_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/setr_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/shallow_seg_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sim_contrastive_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/spacenet2_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/supervised_clustering.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/experiments/sysu_patch_train.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/__init__.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/canny_edge.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/canny_edge.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/deeplab.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/deeplabWS.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplabWS.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/deeplab_diff.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/deeplab_diff.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/encoding.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/encoding.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/gci.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/gci.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/linear_classifier.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/losses.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/losses.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/moco.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/moco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/quantizer.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/quantizer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnet.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnetGNWS.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnetGNWS.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_classification_finetune.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/resnet_enc.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/resnet_enc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/sg.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/sg.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/shallow_seg.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/shallow_seg.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/supcon.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/supcon.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/tex_refine.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/tex_refine.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/transformer_model.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_model.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/models/transformer_seg.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/models/transformer_seg.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/predict.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/predict_patchwise.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_patchwise.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/predict_test.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/predict_test.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/filter_by_sensor.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/scripts/labelbox2coco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/convert_sysucd_to_kwcoco.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/cva.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/cva.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/eval_utils.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/utils.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg/utils/visualization.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/datasets/material_pixel_dataset.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/models/material_mlp.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/rutgers_material_seg_v2/predict.py` & `geowatch-0.6.3/watch/tasks/rutgers_material_seg_v2/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/sam/predict.py` & `geowatch-0.6.3/watch/tasks/sam/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/__init__.py` & `geowatch-0.6.3/watch/tasks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/from_heatmap.py` & `geowatch-0.6.3/watch/tasks/tracking/from_heatmap.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/from_polygon.py` & `geowatch-0.6.3/watch/tasks/tracking/from_polygon.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/normalize.py` & `geowatch-0.6.3/watch/tasks/tracking/normalize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/phase.py` & `geowatch-0.6.3/watch/tasks/tracking/phase.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/utils.py` & `geowatch-0.6.3/watch/tasks/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/tracking/visualize.py` & `geowatch-0.6.3/watch/tasks/tracking/visualize.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/drop0_datasets.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/drop0_datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/fit.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/fit.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/resnets.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/resnets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/unet.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/models/unet_blur.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/models/unet_blur.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/predict.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/predict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/create_splits.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/data/splits_unmasked/create_splits_unmasked.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/spacenet/datasets.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/spacenet/datasets.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/time_sort_S7.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_S7.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/time_sort_module.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/time_sort_module.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/tasks/uky_temporal_prediction/utils.py` & `geowatch-0.6.3/watch/tasks/uky_temporal_prediction/utils.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/__init__.py` & `geowatch-0.6.3/watch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/configargparse_ext.py` & `geowatch-0.6.3/watch/utils/configargparse_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/ext_monai.py` & `geowatch-0.6.3/watch/utils/ext_monai.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/ijson_ext.py` & `geowatch-0.6.3/watch/utils/ijson_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/kwcoco_extensions.py` & `geowatch-0.6.3/watch/utils/kwcoco_extensions.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py` & `geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_ge_4_21.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py` & `geowatch-0.6.3/watch/utils/lightning_ext/_jsonargparse_ext_lt_4_21.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/argparse_ext.py` & `geowatch-0.6.3/watch/utils/lightning_ext/argparse_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/__init__.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/auto_resumer.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/auto_resumer.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/batch_plotter.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/batch_plotter.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/packager.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/packager.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/state_logger.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/state_logger.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/tensorboard_plotter.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/callbacks/text_logger.py` & `geowatch-0.6.3/watch/utils/lightning_ext/callbacks/text_logger.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/demo.py` & `geowatch-0.6.3/watch/utils/lightning_ext/demo.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/lightning_cli_ext.py` & `geowatch-0.6.3/watch/utils/lightning_ext/lightning_cli_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/old_parser_devices.py` & `geowatch-0.6.3/watch/utils/lightning_ext/old_parser_devices.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/lightning_ext/util_device.py` & `geowatch-0.6.3/watch/utils/lightning_ext/util_device.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/partial_format.py` & `geowatch-0.6.3/watch/utils/partial_format.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/process_context.py` & `geowatch-0.6.3/watch/utils/process_context.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/result_analysis.py` & `geowatch-0.6.3/watch/utils/result_analysis.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/reverse_hashid.py` & `geowatch-0.6.3/watch/utils/reverse_hashid.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/simple_dvc.py` & `geowatch-0.6.3/watch/utils/simple_dvc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/slugify_ext.py` & `geowatch-0.6.3/watch/utils/slugify_ext.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_bands.py` & `geowatch-0.6.3/watch/utils/util_bands.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_codes.py` & `geowatch-0.6.3/watch/utils/util_codes.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_data.py` & `geowatch-0.6.3/watch/utils/util_data.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_dotdict.py` & `geowatch-0.6.3/watch/utils/util_dotdict.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_environ.py` & `geowatch-0.6.3/watch/utils/util_environ.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_eval.py` & `geowatch-0.6.3/watch/utils/util_eval.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_framework.py` & `geowatch-0.6.3/watch/utils/util_framework.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_gdal.py` & `geowatch-0.6.3/watch/utils/util_gdal.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_girder.py` & `geowatch-0.6.3/watch/utils/util_girder.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_gis.py` & `geowatch-0.6.3/watch/utils/util_gis.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_globals.py` & `geowatch-0.6.3/watch/utils/util_globals.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_hardware.py` & `geowatch-0.6.3/watch/utils/util_hardware.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_iter.py` & `geowatch-0.6.3/watch/utils/util_iter.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_json.py` & `geowatch-0.6.3/watch/utils/util_json.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_kwarray.py` & `geowatch-0.6.3/watch/utils/util_kwarray.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_kwimage.py` & `geowatch-0.6.3/watch/utils/util_kwimage.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_kwplot.py` & `geowatch-0.6.3/watch/utils/util_kwplot.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_locks.py` & `geowatch-0.6.3/watch/utils/util_locks.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_logging.py` & `geowatch-0.6.3/watch/utils/util_logging.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_nesting.py` & `geowatch-0.6.3/watch/utils/util_nesting.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_netharn.py` & `geowatch-0.6.3/watch/utils/util_netharn.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_nvidia.py` & `geowatch-0.6.3/watch/utils/util_nvidia.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_pandas.py` & `geowatch-0.6.3/watch/utils/util_pandas.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_parallel.py` & `geowatch-0.6.3/watch/utils/util_parallel.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_param_grid.py` & `geowatch-0.6.3/watch/utils/util_param_grid.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_path.py` & `geowatch-0.6.3/watch/utils/util_path.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_pattern.py` & `geowatch-0.6.3/watch/utils/util_pattern.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_progress.py` & `geowatch-0.6.3/watch/utils/util_progress.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_raster.py` & `geowatch-0.6.3/watch/utils/util_raster.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_regex.py` & `geowatch-0.6.3/watch/utils/util_regex.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_resolution.py` & `geowatch-0.6.3/watch/utils/util_resolution.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_resources.py` & `geowatch-0.6.3/watch/utils/util_resources.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_rgdc.py` & `geowatch-0.6.3/watch/utils/util_rgdc.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_s3.py` & `geowatch-0.6.3/watch/utils/util_s3.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_stringalgo.py` & `geowatch-0.6.3/watch/utils/util_stringalgo.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_time.py` & `geowatch-0.6.3/watch/utils/util_time.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_torchmetrics.py` & `geowatch-0.6.3/watch/utils/util_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_windows.py` & `geowatch-0.6.3/watch/utils/util_windows.py`

 * *Files identical despite different names*

### Comparing `geowatch-0.6.2/watch/utils/util_yaml.py` & `geowatch-0.6.3/watch/utils/util_yaml.py`

 * *Files identical despite different names*

