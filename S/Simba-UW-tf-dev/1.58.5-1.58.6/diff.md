# Comparing `tmp/Simba-UW-tf-dev-1.58.5.tar.gz` & `tmp/Simba-UW-tf-dev-1.58.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.5.tar", last modified: Tue May  2 00:50:33 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.58.6.tar", last modified: Wed May  3 19:07:50 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.58.5.tar` & `Simba-UW-tf-dev-1.58.6.tar`

### file list

```diff
@@ -1,478 +1,482 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:49.000000 Simba-UW-tf-dev-1.58.5/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9311 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15058 2023-04-30 14:52:21.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5064 2023-04-29 19:45:45.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12964 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5996 2023-04-28 23:45:44.000000 Simba-UW-tf-dev-1.58.5/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12788 2023-05-01 23:51:03.000000 Simba-UW-tf-dev-1.58.5/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10867 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13243 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/ui/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)    33818 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.5/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.5/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.5/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    20637 2023-05-02 00:47:44.000000 Simba-UW-tf-dev-1.58.5/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3419 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.5/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3385 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9955 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41575 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    36868 2023-05-01 00:37:11.000000 Simba-UW-tf-dev-1.58.5/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2335 2023-04-28 17:41:31.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.5/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    40521 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    22224 2023-04-29 19:18:55.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60505 2023-04-30 15:39:23.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6161 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.5/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16894 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12198 2023-05-01 19:31:25.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11588 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    19886 2023-04-30 16:53:25.000000 Simba-UW-tf-dev-1.58.5/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.5/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)    33751 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.5/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    14068 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.5/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8347 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.5/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9092 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10173 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8563 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12304 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    16589 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15891 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10168 2023-04-30 15:51:37.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5754 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12242 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11210 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15137 2023-04-30 15:05:27.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9888 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2023-04-30 14:48:28.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13133 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8979 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8267 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6329 2023-04-28 18:51:08.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7407 2023-04-28 19:12:39.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12822 2023-05-01 13:08:33.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4821 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16794 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9551 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.5/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18624 2023-05-01 20:34:07.000000 Simba-UW-tf-dev-1.58.5/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.5/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6503 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19691 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/sleap_csv_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.5/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    41580 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.5/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65306 2023-05-01 20:29:10.000000 Simba-UW-tf-dev-1.58.5/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.5/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.5/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.5/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.5/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.5/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-02 00:50:32.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18244 2023-05-02 00:50:32.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-02 00:50:32.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-02 00:50:32.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-02 00:50:32.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-02 00:50:32.000000 Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.5/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.5/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.5/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-02 00:50:26.000000 Simba-UW-tf-dev-1.58.5/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-02 00:50:33.000000 Simba-UW-tf-dev-1.58.5/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-03 18:36:16.000000 Simba-UW-tf-dev-1.58.6/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3477 2023-05-03 16:54:51.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8366 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9311 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-29 16:41:16.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9494 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15058 2023-05-03 16:56:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4066 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5463 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8697 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7928 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6409 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7536 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5064 2023-04-29 19:45:45.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4098 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2798 2023-05-03 18:37:08.000000 Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12964 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5996 2023-04-28 23:45:44.000000 Simba-UW-tf-dev-1.58.6/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12788 2023-05-01 23:51:03.000000 Simba-UW-tf-dev-1.58.6/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10867 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    33818 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.6/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.58.6/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-28 20:24:21.000000 Simba-UW-tf-dev-1.58.6/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    20637 2023-05-02 00:47:44.000000 Simba-UW-tf-dev-1.58.6/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3419 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26652 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.6/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6543 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11932 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-23 19:55:32.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8187 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5693 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7268 2023-04-28 12:30:12.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9910 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     9915 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2347 2023-04-28 12:22:34.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20886 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10289 2023-04-28 13:09:30.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6698 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     6790 2023-04-28 00:15:19.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23590 2023-04-28 20:48:50.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8521 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6067 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11228 2023-04-28 00:28:29.000000 Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    43012 2023-05-03 18:35:59.000000 Simba-UW-tf-dev-1.58.6/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42323 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2023-04-28 15:16:26.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27783 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3491 2023-05-03 13:59:23.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13322 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8282 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46269 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28134 2023-04-28 18:40:57.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23897 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16825 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.58.6/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41772 2023-05-03 16:41:23.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29306 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    17367 2023-05-01 18:54:03.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    23305 2023-05-03 14:22:51.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60449 2023-05-03 18:46:32.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    55362 2023-05-01 20:52:34.000000 Simba-UW-tf-dev-1.58.6/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6228 2023-04-26 18:27:58.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9945 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9063 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16894 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18248 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8173 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6859 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5331 2023-04-25 01:50:43.000000 Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7594 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12198 2023-05-01 19:31:25.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16737 2023-05-01 19:58:28.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1690 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15289 2023-05-01 19:38:38.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12615 2023-05-01 19:51:32.000000 Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11588 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20258 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.58.6/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.58.6/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5592 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)    33751 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     7034 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.6/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    14068 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1573 2023-04-29 19:08:53.000000 Simba-UW-tf-dev-1.58.6/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8347 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5223 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     2613 2023-04-25 15:16:24.000000 Simba-UW-tf-dev-1.58.6/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5617 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9092 2023-04-29 19:43:53.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13238 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14636 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10173 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15981 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8563 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12304 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    15119 2023-05-03 19:00:40.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15891 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12739 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10168 2023-04-30 15:51:37.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5754 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12771 2023-04-26 14:16:42.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12242 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7917 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11210 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15174 2023-05-03 19:01:38.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11330 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9467 2023-05-03 00:36:49.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13232 2023-05-03 18:58:48.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11482 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15610 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13133 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8979 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8267 2023-04-30 15:54:10.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9761 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16321 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6329 2023-04-28 18:51:08.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11575 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7407 2023-04-28 19:12:39.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12822 2023-05-01 13:08:33.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6317 2023-04-25 18:03:32.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9366 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4821 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16794 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9551 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7698 2023-05-03 14:34:44.000000 Simba-UW-tf-dev-1.58.6/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19187 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3542 2023-04-28 20:13:23.000000 Simba-UW-tf-dev-1.58.6/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18624 2023-05-01 20:34:07.000000 Simba-UW-tf-dev-1.58.6/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3170 2023-04-28 20:11:10.000000 Simba-UW-tf-dev-1.58.6/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6487 2023-05-03 18:24:03.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1753 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43131 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3403 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19758 2023-05-03 16:31:29.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11332 2023-04-26 21:13:20.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11384 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13793 2023-04-26 14:59:42.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     7349 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/sleap_csv_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9719 2023-05-01 00:05:15.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6451 2023-05-01 17:30:49.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10945 2023-05-01 17:21:29.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    22015 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23524 2023-04-30 23:21:29.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    23603 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 16:49:14.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21021 2023-04-30 23:23:03.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7783 2023-04-28 20:16:23.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6949 2023-04-28 20:19:13.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.58.6/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    41580 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24645 2023-04-28 20:51:11.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7174 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8214 2023-04-28 19:26:14.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11106 2023-04-25 13:26:59.000000 Simba-UW-tf-dev-1.58.6/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7377 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8190 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2913 2023-04-28 17:39:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64875 2023-05-03 18:36:47.000000 Simba-UW-tf-dev-1.58.6/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-25 19:14:34.000000 Simba-UW-tf-dev-1.58.6/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.58.6/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.58.6/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.58.6/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.58.6/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18464 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-03 19:07:49.000000 Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.58.6/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.58.6/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.58.6/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-03 19:07:11.000000 Simba-UW-tf-dev-1.58.6/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-03 19:07:50.000000 Simba-UW-tf-dev-1.58.6/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.58.5/PKG-INFO` & `Simba-UW-tf-dev-1.58.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.5
+Version: 1.58.6
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/.DS_Store`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000a  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00000130: 0000 0001 80a5 0000 000b 005f 005f 0070  ..........._._.p
+00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00000150: 6d6f 4444 626c 6f62 0000 0008 1c4c ed42  moDDblob.....L.B
+00000160: 5efb c441 0000 000b 005f 005f 0070 0079  ^..A....._._.p.y
+00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000180: 6444 626c 6f62 0000 0008 3ec7 3173 23f2  dDblob....>.1s#.
+00000190: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000001b0: 636f 6d70 0000 0000 0001 c000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,52 +58,52 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 000a 0000 000b  ................
-00000410: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000420: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000430: 0000 0003 7637 0000 000b 005f 005f 0070  ....v7....._._.p
-00000440: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000450: 6d6f 4444 626c 6f62 0000 0008 29d7 a4d0  moDDblob....)...
-00000460: 97fe c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
-00000470: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000480: 6444 626c 6f62 0000 0008 29d7 a4d0 97fe  dDblob....).....
-00000490: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000004a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000004b0: 636f 6d70 0000 0000 0003 b000 0000 0007  comp............
-000004c0: 0070 006f 0070 005f 0075 0070 0073 6277  .p.o.p._.u.p.sbw
-000004d0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
-000004e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
-000004f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00000500: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
-00000510: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00000520: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00000530: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00000540: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00000550: 6261 7208 0809 0809 5f10 187b 7b33 3532  bar....._..{{352
-00000560: 2c20 3234 377d 2c20 7b39 3839 2c20 3433  , 247}, {989, 43
-00000570: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
-00000580: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
-00000590: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 9a00 0000 0700 7000 6f00 7000 5f00  ........p.o.p._.
-000005b0: 7500 7000 736c 6731 5363 6f6d 7000 0000  u.p.slg1Scomp...
-000005c0: 0000 03c1 2a00 0000 0700 7000 6f00 7000  ....*.....p.o.p.
-000005d0: 5f00 7500 7000 736d 6f44 4462 6c6f 6200  _.u.p.smoDDblob.
-000005e0: 0000 0892 a674 16c0 fec4 4100 0000 0700  .....t....A.....
-000005f0: 7000 6f00 7000 5f00 7500 7000 736d 6f64  p.o.p._.u.p.smod
-00000600: 4462 6c6f 6200 0000 0892 a674 16c0 fec4  Dblob......t....
-00000610: 4100 0000 0700 7000 6f00 7000 5f00 7500  A.....p.o.p._.u.
-00000620: 7000 7370 6831 5363 6f6d 7000 0000 0000  p.sph1Scomp.....
-00000630: 04f0 0000 0000 0700 7000 6f00 7000 5f00  ........p.o.p._.
-00000640: 7500 7000 7376 5372 6e6c 6f6e 6700 0000  u.p.svSrnlong...
-00000650: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 040a 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,16 +318,16 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001450: 0100 0002 0000 0000 0000 0000 0200 0008  ................
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 
 
 class PathPlotPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
-        PopUpMixin.__init__(self, title='CREATE PATH PLOTS')
         ConfigReader.__init__(self, config_path=config_path)
         self.data_path = os.path.join(self.project_path, Paths.MACHINE_RESULTS_DIR.value)
         self.files_found_dict = get_file_name_info_in_directory(directory=self.data_path, file_type=self.file_type)
         check_if_filepath_list_is_empty(filepaths=list(self.files_found_dict.keys()),
                                         error_msg='SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. Create classification results before visualizing path plots')
 
+        PopUpMixin.__init__(self, title='CREATE PATH PLOTS')
         self.resolutions.insert(0, 'As input')
         self.animal_cnt_options = list(range(1, self.animal_cnt+1))
 
         self.style_settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='STYLE SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.PATH_PLOTS.value)
         self.autocompute_var = BooleanVar(value=True)
         self.auto_compute_styles = Checkbutton(self.style_settings_frm, text='Auto-compute styles', variable=self.autocompute_var, command=self.enable_style_settings)
         self.resolution_dropdown = DropDownMenu(self.style_settings_frm, 'Resolution:', self.resolutions, '16')
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.58.6/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.58.6/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.58.6/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.58.6/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.58.6/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     ALL_FEATURES_EXCLUDING_POSE = 'ALL FEATURES (EXCLUDING POSE)'
     ALL_FEATURES_INCLUDING_POSE = 'ALL FEATURES (INCLUDING POSE)'
     USER_DEFINED_SET = 'USER-DEFINED FEATURE SET'
     NAMES = 'NAMES'
     START_FRAME = 'START_FRAME'
     END_FRAME = 'END_FRAME'
     CLASSIFIER = 'CLASSIFIER'
-    SCALER_NAMES = ['MIN-MAX', 'STANDARD', 'QUANTILE']
     PROBABILITY = 'PROBABILITY'
     FRAME = 'FRAME'
     VIDEO = 'VIDEO'
     FEATURE_PATH = 'feature_path'
     BOUT_AGGREGATION_TYPE = 'bout_aggregation_type'
     MIN_BOUT_LENGTH = 'min_bout_length'
     N_NEIGHBORS = 'n_neighbors'
@@ -52,32 +51,30 @@
     BOUTS_TARGETS = 'BOUTS_TARGETS'
     DATASET_DATA_FIELDS = [FRAME_FEATURES, FRAME_POSE, FRAME_TARGETS, BOUTS_FEATURES, BOUTS_TARGETS]
     MIN_MAX = 'MIN-MAX'
     STANDARD = 'STANDARD'
     QUANTILE = 'QUANTILE'
     LOW_VARIANCE_FIELDS = 'LOW_VARIANCE_FIELDS'
 
-
 class Clustering(Enum):
     ALPHA = 'alpha'
     MIN_CLUSTER_SIZE = 'min_cluster_size'
     MIN_SAMPLES = 'min_samples'
     EPSILON = 'cluster_selection_epsilon'
     CLUSTER_MODEL = 'CLUSTER_MODEL'
 
-
-class UnsupervisedOptions(Enum):
+class UMLOptions(Enum):
     FEATURE_SLICE_OPTIONS = [Unsupervised.ALL_FEATURES_INCLUDING_POSE.value,
                           Unsupervised.ALL_FEATURES_EXCLUDING_POSE.value,
                           Unsupervised.USER_DEFINED_SET.value]
     BOUT_AGGREGATION_METHODS = ['MEAN', 'MEDIAN']
     DATA_FORMATS = ['NONE', 'SCALED', 'RAW']
     SAVE_FORMATS = ['CSV', 'PICKLE']
     CORRELATION_OPTIONS = ['SPEARMAN', 'PEARSONS', 'KENDALL']
-
+    SCALER_OPTIONS = ['MIN-MAX', 'STANDARD', 'QUANTILE']
     CATEGORICAL_OPTIONS = ['VIDEO', 'CLASSIFIER', 'CLUSTER']
     CONTINUOUS_OPTIONS = ['START_FRAME', 'END_FRAME', 'PROBABILITY']
     SPEED_OPTIONS = [round(x, 1) for x in list(np.arange(0.1, 2.1, 0.1))]
     SHAP_CLUSTER_METHODS = ['Paired clusters']
     DR_ALGO_OPTIONS = ['UMAP', 'TSNE']
     CLUSTERING_ALGO_OPTIONS = ['HDBSCAN']
     VARIANCE_OPTIONS = list(range(0, 100, 10))
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                                         Entry_Box,
                                         DropDownMenu,
                                         FileSelect)
 import tkinter.ttk as ttk
 from simba.utils.enums import Formats
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
-from simba.unsupervised.enums import UnsupervisedOptions, Unsupervised
+from simba.unsupervised.enums import UMLOptions, Unsupervised
 from simba.unsupervised.dataset_creator import DatasetCreator
 from simba.unsupervised.pop_up_classes import (GridSearchVisualizerPopUp,
                                                DataExtractorPopUp,
                                                FitDimReductionPopUp,
                                                FitClusterModelsPopUp,
                                                TransformDimReductionPopUp,
                                                TransformClustererPopUp,
@@ -50,21 +50,21 @@
         self.main_frm.grid(row=0)
 
         self.clf_slice_options = [f'ALL CLASSIFIERS ({len(self.clf_names)})']
         for clf_name in self.clf_names: self.clf_slice_options.append(f'{clf_name}')
         create_dataset_frm = LabelFrame(self.create_dataset_tab, text='CREATE DATASET', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.feature_file_selected = FileSelect(create_dataset_frm, "FEATURE FILE (CSV)", lblwidth=25)
 
-        self.data_slice_dropdown = DropDownMenu(create_dataset_frm, 'FEATURE SLICE:', UnsupervisedOptions.FEATURE_SLICE_OPTIONS.value, '25', com= lambda x: self.change_status_of_file_select())
-        self.data_slice_dropdown.setChoices(UnsupervisedOptions.FEATURE_SLICE_OPTIONS.value[0])
+        self.data_slice_dropdown = DropDownMenu(create_dataset_frm, 'FEATURE SLICE:', UMLOptions.FEATURE_SLICE_OPTIONS.value, '25', com= lambda x: self.change_status_of_file_select())
+        self.data_slice_dropdown.setChoices(UMLOptions.FEATURE_SLICE_OPTIONS.value[0])
         self.clf_slice_dropdown = DropDownMenu(create_dataset_frm, 'CLASSIFIER SLICE:', self.clf_slice_options, '25')
         self.clf_slice_dropdown.setChoices(self.clf_slice_options[0])
         self.change_status_of_file_select()
-        self.bout_dropdown = DropDownMenu(create_dataset_frm, 'BOUT AGGREGATION METHOD:', UnsupervisedOptions.BOUT_AGGREGATION_METHODS.value, '25')
-        self.bout_dropdown.setChoices(choice=UnsupervisedOptions.BOUT_AGGREGATION_METHODS.value[0])
+        self.bout_dropdown = DropDownMenu(create_dataset_frm, 'BOUT AGGREGATION METHOD:', UMLOptions.BOUT_AGGREGATION_METHODS.value, '25')
+        self.bout_dropdown.setChoices(choice=UMLOptions.BOUT_AGGREGATION_METHODS.value[0])
         self.min_bout_length = Entry_Box(create_dataset_frm, 'MINIMUM BOUT LENGTH (MS): ', '25', validation='numeric')
         self.min_bout_length.entry_set(val=0)
         self.create_btn = Button(create_dataset_frm, text='CREATE DATASET', fg='blue', command= lambda: self.create_dataset())
 
         create_dataset_frm.grid(row=0, column=0, sticky=NW)
         self.data_slice_dropdown.grid(row=0, column=0, sticky=NW)
         self.clf_slice_dropdown.grid(row=1, column=0, sticky=NW)
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/pop_up_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                                         Entry_Box)
 
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.unsupervised_mixin import UnsupervisedMixin
 
 from simba.utils.enums import Formats, Options
-from simba.unsupervised.enums import UnsupervisedOptions, Unsupervised, Clustering
+from simba.unsupervised.enums import UMLOptions, Unsupervised, Clustering
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty, check_if_dir_exists, check_int
 
 
 from simba.unsupervised.grid_search_visualizers import GridSearchVisualizer
 from simba.unsupervised.data_extractor import DataExtractor
 from simba.utils.errors import NoSpecifiedOutputError
 from simba.unsupervised.umap_embedder import UmapEmbedder
@@ -41,31 +41,31 @@
         data_frm = LabelFrame(self.main_frm, text='DATA', fg='black', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.data_dir_select = FolderSelect(data_frm, "DATA DIRECTORY:", lblwidth=25)
         self.save_dir_select = FolderSelect(data_frm, "OUTPUT DIRECTORY: ", lblwidth=25)
         data_frm.grid(row=0, column=0, sticky=NW)
         self.data_dir_select.grid(row=0, column=0, sticky=NW)
         self.save_dir_select.grid(row=1, column=0, sticky=NW)
 
-        self.visualization_options = UnsupervisedOptions.CATEGORICAL_OPTIONS.value + UnsupervisedOptions.CONTINUOUS_OPTIONS.value
+        self.visualization_options = UMLOptions.CATEGORICAL_OPTIONS.value + UMLOptions.CONTINUOUS_OPTIONS.value
         settings_frm = LabelFrame(self.main_frm,text='SETTINGS',font=Formats.LABELFRAME_HEADER_FORMAT.value,padx=5,pady=5,fg='black')
-        self.scatter_size_dropdown = DropDownMenu(settings_frm, 'SCATTER SIZE:', UnsupervisedOptions.SCATTER_SIZE.value, '25')
+        self.scatter_size_dropdown = DropDownMenu(settings_frm, 'SCATTER SIZE:', UMLOptions.SCATTER_SIZE.value, '25')
         self.scatter_size_dropdown.setChoices(5)
         self.categorical_palette_dropdown = DropDownMenu(settings_frm, 'CATEGORICAL PALETTE:', Options.PALETTE_OPTIONS_CATEGORICAL.value, '25')
         self.categorical_palette_dropdown.setChoices('Set1')
         self.continuous_palette_dropdown = DropDownMenu(settings_frm, 'CONTINUOUS PALETTE:', Options.PALETTE_OPTIONS.value, '25')
         self.continuous_palette_dropdown.setChoices('magma')
 
         settings_frm.grid(row=1, column=0, sticky=NW)
         self.scatter_size_dropdown.grid(row=0, column=0, sticky=NW)
         self.categorical_palette_dropdown.grid(row=1, column=0, sticky=NW)
         self.continuous_palette_dropdown.grid(row=2, column=0, sticky=NW)
 
         self.define_plots_frm = LabelFrame(self.main_frm, text='DEFINE PLOTS', font=Formats.LABELFRAME_HEADER_FORMAT.value, padx=5, pady=5, fg='black')
-        self.plot_cnt_dropdown = DropDownMenu(self.define_plots_frm, '# PLOTS:', UnsupervisedOptions.GRAPH_CNT.value, '25', com= lambda x:self.show_plot_table())
-        self.plot_cnt_dropdown.setChoices(UnsupervisedOptions.GRAPH_CNT.value[0])
+        self.plot_cnt_dropdown = DropDownMenu(self.define_plots_frm, '# PLOTS:', UMLOptions.GRAPH_CNT.value, '25', com= lambda x:self.show_plot_table())
+        self.plot_cnt_dropdown.setChoices(UMLOptions.GRAPH_CNT.value[0])
         self.show_plot_table()
         self.define_plots_frm.grid(row=2, column=0, sticky=NW)
         self.plot_cnt_dropdown.grid(row=0, column=0, sticky=NW)
 
         self.create_run_frm(title='RUN', run_function=self.run)
         self.main_frm.mainloop()
 
@@ -93,15 +93,15 @@
         settings = {}
         settings['SCATTER_SIZE'] = int(self.scatter_size_dropdown.getChoices())
         settings['CATEGORICAL_PALETTE'] = self.categorical_palette_dropdown.getChoices()
         settings['CONTINUOUS_PALETTE'] = self.continuous_palette_dropdown.getChoices()
 
         continuous_vars, categorical_vars = [], []
         for k, v in self.plot_data.items():
-            if v['variable'].getChoices() in UnsupervisedOptions.CONTINUOUS_OPTIONS.value:
+            if v['variable'].getChoices() in UMLOptions.CONTINUOUS_OPTIONS.value:
                 continuous_vars.append(v['variable'].getChoices())
             else:
                 categorical_vars.append(v['variable'].getChoices())
         grid_search_visualizer = GridSearchVisualizer(model_dir=self.data_dir_select.folder_path,
                                                       save_dir=self.save_dir_select.folder_path,
                                                       settings=settings)
         grid_search_visualizer.continuous_visualizer(continuous_vars=continuous_vars)
@@ -119,16 +119,16 @@
         data_frm = LabelFrame(self.main_frm, text='DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.data_dir_select = FolderSelect(data_frm, "DATA DIRECTORY:", lblwidth=25)
 
         data_frm.grid(row=0, column=0, sticky=NW)
         self.data_dir_select.grid(row=0, column=0, sticky=NW)
 
         data_type_frm = LabelFrame(self.main_frm, text='DATA TYPE', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
-        self.data_type_dropdown = DropDownMenu(data_type_frm, 'DATA TYPE:', UnsupervisedOptions.DATA_TYPES.value, '25')
-        self.data_type_dropdown.setChoices(UnsupervisedOptions.DATA_TYPES.value[0])
+        self.data_type_dropdown = DropDownMenu(data_type_frm, 'DATA TYPE:', UMLOptions.DATA_TYPES.value, '25')
+        self.data_type_dropdown.setChoices(UMLOptions.DATA_TYPES.value[0])
         data_type_frm.grid(row=1, column=0, sticky=NW)
         self.data_type_dropdown.grid(row=0, column=0, sticky=NW)
         self.create_run_frm(run_function=self.run, title='RUN')
         self.main_frm.mainloop()
 
     def run(self):
         check_if_dir_exists(self.data_dir_select.folder_path)
@@ -139,15 +139,15 @@
 #_ = DataExtractorPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/project_folder/project_config.ini')
 
 
 class FitDimReductionPopUp(PopUpMixin, ConfigReader):
 
     def __init__(self):
         super().__init__(title='FIT DIMENSIONALITY REDUCTION MODELS')
-        self.variance_options = [str(x) + '%' for x in UnsupervisedOptions.VARIANCE_OPTIONS.value]
+        self.variance_options = [str(x) + '%' for x in UMLOptions.VARIANCE_OPTIONS.value]
 
         self.dataset_frm = LabelFrame(self.main_frm, text='DATASET', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.dataset_file_selected = FileSelect(self.dataset_frm, "DATASET (PICKLE):", lblwidth=25)
         self.dataset_frm.grid(row=0, column=0, sticky=NW)
         self.dataset_file_selected.grid(row=0, column=0, sticky=NW)
 
         self.save_frm = LabelFrame(self.main_frm, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
@@ -156,16 +156,16 @@
         self.save_dir.grid(row=0, column=0, sticky=NW)
 
         settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.scaling_dropdown = DropDownMenu(settings_frm, 'SCALING:', Options.SCALER_NAMES.value, '25')
         self.scaling_dropdown.setChoices(Options.SCALER_NAMES.value[0])
         self.var_threshold_dropdown = DropDownMenu(settings_frm, 'VARIANCE THRESHOLD:', self.variance_options, '25')
         self.var_threshold_dropdown.setChoices(self.variance_options[0])
-        self.algo_dropdown = DropDownMenu(settings_frm, 'ALGORITHM:', UnsupervisedOptions.DR_ALGO_OPTIONS.value, '25', com=lambda x: self.show_dr_hyperparameters())
-        self.algo_dropdown.setChoices(UnsupervisedOptions.DR_ALGO_OPTIONS.value[0])
+        self.algo_dropdown = DropDownMenu(settings_frm, 'ALGORITHM:', UMLOptions.DR_ALGO_OPTIONS.value, '25', com=lambda x: self.show_dr_hyperparameters())
+        self.algo_dropdown.setChoices(UMLOptions.DR_ALGO_OPTIONS.value[0])
         self.show_dr_hyperparameters()
 
         settings_frm.grid(row=2, column=0, sticky=NW)
         self.scaling_dropdown.grid(row=0, column=0, sticky=NW)
         self.var_threshold_dropdown.grid(row=1, column=0, sticky=NW)
         self.algo_dropdown.grid(row=2, column=0, sticky=NW)
         self.main_frm.mainloop()
@@ -267,18 +267,18 @@
 class TransformDimReductionPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='DIMENSIONALITY REDUCTION: TRANSFORM')
         self.dim_reduction_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.model_select = FileSelect(self.dim_reduction_frm, 'MODEL (PICKLE):', lblwidth=25)
         self.dataset_select = FileSelect(self.dim_reduction_frm, 'DATASET (PICKLE):', lblwidth=25)
         self.save_dir = FolderSelect(self.dim_reduction_frm, "SAVE DIRECTORY: ", lblwidth=25)
-        self.features_dropdown = DropDownMenu(self.dim_reduction_frm, 'INCLUDE FEATURES:', UnsupervisedOptions.DATA_FORMATS.value, '25')
-        self.features_dropdown.setChoices(UnsupervisedOptions.DATA_FORMATS.value[0])
-        self.save_format_dropdown = DropDownMenu(self.dim_reduction_frm, 'SAVE FORMATS:', UnsupervisedOptions.SAVE_FORMATS.value, '25')
-        self.save_format_dropdown.setChoices(UnsupervisedOptions.SAVE_FORMATS.value[0])
+        self.features_dropdown = DropDownMenu(self.dim_reduction_frm, 'INCLUDE FEATURES:', UMLOptions.DATA_FORMATS.value, '25')
+        self.features_dropdown.setChoices(UMLOptions.DATA_FORMATS.value[0])
+        self.save_format_dropdown = DropDownMenu(self.dim_reduction_frm, 'SAVE FORMATS:', UMLOptions.SAVE_FORMATS.value, '25')
+        self.save_format_dropdown.setChoices(UMLOptions.SAVE_FORMATS.value[0])
 
         self.dim_reduction_frm.grid(row=0, column=0, sticky=NW)
         self.model_select.grid(row=0, column=0, sticky=NW)
         self.dataset_select.grid(row=1, column=0, sticky=NW)
         self.save_dir.grid(row=2, column=0, sticky=NW)
         self.features_dropdown.grid(row=3, column=0, sticky=NW)
         self.save_format_dropdown.grid(row=4, column=0, sticky=NW)
@@ -303,16 +303,16 @@
     def __init__(self):
         super().__init__(title='CLUSTERING FIT: GRID SEARCH')
         self.dataset_frm = LabelFrame(self.main_frm, text='DATASET', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.data_dir_selected = FolderSelect(self.dataset_frm, "DATA DIRECTORY (PICKLES): ", lblwidth=25)
         self.save_frm = LabelFrame(self.main_frm, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.save_dir = FolderSelect(self.save_frm, "SAVE DIRECTORY: ", lblwidth=25)
         self.algo_frm = LabelFrame(self.main_frm, text='ALGORITHM', pady=5, padx=5,font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
-        self.algo_dropdown = DropDownMenu(self.algo_frm, 'ALGORITHM:', UnsupervisedOptions.CLUSTERING_ALGO_OPTIONS.value, '25', com=lambda x: self.show_hyperparameters())
-        self.algo_dropdown.setChoices(UnsupervisedOptions.CLUSTERING_ALGO_OPTIONS.value[0])
+        self.algo_dropdown = DropDownMenu(self.algo_frm, 'ALGORITHM:', UMLOptions.CLUSTERING_ALGO_OPTIONS.value, '25', com=lambda x: self.show_hyperparameters())
+        self.algo_dropdown.setChoices(UMLOptions.CLUSTERING_ALGO_OPTIONS.value[0])
         self.value_frm = LabelFrame(self.main_frm, fg='black')
         self.value_entry_box = Entry_Box(self.value_frm, 'VALUE:', '25')
 
         self.dataset_frm.grid(row=0, column=0, sticky=NW)
         self.data_dir_selected.grid(row=0, column=0, sticky=NW)
         self.save_frm.grid(row=1, column=0, sticky=NW)
         self.save_dir.grid(row=0, column=0, sticky=NW)
@@ -397,18 +397,18 @@
 class TransformClustererPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='CLUSTERING: TRANSFORM')
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.model_select = FileSelect(self.settings_frm, 'CLUSTER MODEL (PICKLE):', lblwidth=25)
         self.data_select = FileSelect(self.settings_frm, 'DATASET (PICKLE):',  lblwidth=25)
         self.save_dir = FolderSelect(self.settings_frm, "SAVE DIRECTORY:",  lblwidth=25)
-        self.features_dropdown = DropDownMenu(self.settings_frm, 'INCLUDE FEATURES:', UnsupervisedOptions.DATA_FORMATS.value, '25')
-        self.features_dropdown.setChoices(UnsupervisedOptions.DATA_FORMATS.value[0])
-        self.save_format_dropdown = DropDownMenu(self.settings_frm, 'SAVE FORMATS:', UnsupervisedOptions.SAVE_FORMATS.value, '25')
-        self.save_format_dropdown.setChoices(UnsupervisedOptions.SAVE_FORMATS.value[0])
+        self.features_dropdown = DropDownMenu(self.settings_frm, 'INCLUDE FEATURES:', UMLOptions.DATA_FORMATS.value, '25')
+        self.features_dropdown.setChoices(UMLOptions.DATA_FORMATS.value[0])
+        self.save_format_dropdown = DropDownMenu(self.settings_frm, 'SAVE FORMATS:', UMLOptions.SAVE_FORMATS.value, '25')
+        self.save_format_dropdown.setChoices(UMLOptions.SAVE_FORMATS.value[0])
         self.settings_frm.grid(row=0, column=0, sticky=NW)
         self.model_select.grid(row=0, column=0, sticky=NW)
         self.data_select.grid(row=1, column=0, sticky=NW)
         self.save_dir.grid(row=2, column=0, sticky=NW)
         self.features_dropdown.grid(row=3, column=0, sticky=NW)
         self.save_format_dropdown.grid(row=4, column=0, sticky=NW)
         self.create_run_frm(run_function=self.run)
@@ -447,15 +447,15 @@
 
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value,fg='black')
         self.include_pose = Checkbutton(self.settings_frm, text='INCLUDE POSE-ESTIMATION', variable=self.include_pose_var, command=lambda: self.enable_entrybox_from_checkbox(check_box_var=self.include_pose_var,entry_boxes=[self.circle_size_entry]))
         self.circle_size_entry = Entry_Box(self.settings_frm, 'CIRCLE SIZE: ', '25', validation='numeric')
         self.circle_size_entry.entry_set(val=5)
         self.circle_size_entry.set_state(setstatus='disable')
 
-        self.speed_dropdown = DropDownMenu(self.settings_frm, 'VIDEO SPEED:', UnsupervisedOptions.SPEED_OPTIONS.value, '25')
+        self.speed_dropdown = DropDownMenu(self.settings_frm, 'VIDEO SPEED:', UMLOptions.SPEED_OPTIONS.value, '25')
         self.speed_dropdown.setChoices(1.0)
         self.settings_frm.grid(row=1, column=0, sticky=NW)
         self.include_pose.grid(row=0, column=0, sticky=NW)
         self.circle_size_entry.grid(row=1, column=0, sticky=NW)
         self.speed_dropdown.grid(row=2, column=0, sticky=NW)
         self.create_run_frm(run_function=self.run)
 
@@ -540,17 +540,17 @@
         self.model_select = FileSelect(self.data_frm, 'MODEL PATH:', lblwidth=25)
         self.data_frm.grid(row=0, column=0, sticky=NW)
         self.model_select.grid(row=0, column=0, sticky=NW)
 
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.gini_importance_cb = Checkbutton(self.settings_frm, text='CLUSTER RF GINI IMPORTANCE', variable=self.gini_importance_var)
         self.permutation_cb = Checkbutton(self.settings_frm, text='CLUSTER RF PERMUTATION IMPORTANCE', variable=self.permutation_importance_var)
-        self.shap_method_dropdown = DropDownMenu(self.settings_frm, 'SHAP METHOD:', UnsupervisedOptions.SHAP_CLUSTER_METHODS.value, '25')
-        self.shap_method_dropdown.setChoices(UnsupervisedOptions.SHAP_CLUSTER_METHODS.value[0])
-        self.shap_sample_dropdown = DropDownMenu(self.settings_frm, 'SHAP SAMPLES:', UnsupervisedOptions.SHAP_SAMPLE_OPTIONS.value, '25')
+        self.shap_method_dropdown = DropDownMenu(self.settings_frm, 'SHAP METHOD:', UMLOptions.SHAP_CLUSTER_METHODS.value, '25')
+        self.shap_method_dropdown.setChoices(UMLOptions.SHAP_CLUSTER_METHODS.value[0])
+        self.shap_sample_dropdown = DropDownMenu(self.settings_frm, 'SHAP SAMPLES:', UMLOptions.SHAP_SAMPLE_OPTIONS.value, '25')
         self.shap_sample_dropdown.setChoices(100)
         self.shap_method_dropdown.disable()
         self.shap_sample_dropdown.disable()
         self.shap_cb = Checkbutton(self.settings_frm, text='CLUSTER RF SHAP VALUES', variable=self.shap_var, command= lambda:self.enable_dropdown_from_checkbox(check_box_var=self.shap_var, dropdown_menus=[self.shap_method_dropdown, self.shap_sample_dropdown]))
 
         self.settings_frm.grid(row=1, column=0, sticky=NW)
         self.gini_importance_cb.grid(row=0, column=0, sticky=NW)
@@ -590,17 +590,17 @@
         self.data_frm.grid(row=0, column=0, sticky=NW)
         self.data_file_selected.grid(row=0, column=0, sticky=NW)
 
         self.settings_frm = LabelFrame(self.main_frm, text='SETTINGS', pady=5, padx=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.spearman_cb = Checkbutton(self.settings_frm, text='SPEARMAN', variable=self.spearman_var)
         self.pearsons_cb = Checkbutton(self.settings_frm, text='PEARSONS', variable=self.pearsons_var)
         self.kendall_cb = Checkbutton(self.settings_frm, text='KENDALL', variable=self.kendall_var)
-        self.plot_correlation_dropdown = DropDownMenu(self.settings_frm, 'PLOT CORRELATION:', UnsupervisedOptions.CORRELATION_OPTIONS.value, '25')
+        self.plot_correlation_dropdown = DropDownMenu(self.settings_frm, 'PLOT CORRELATION:', UMLOptions.CORRELATION_OPTIONS.value, '25')
         self.plot_correlation_clr_dropdown = DropDownMenu(self.settings_frm, 'PLOT CORRELATION:', Options.PALETTE_OPTIONS.value, '25')
-        self.plot_correlation_dropdown.setChoices(UnsupervisedOptions.CORRELATION_OPTIONS.value[0])
+        self.plot_correlation_dropdown.setChoices(UMLOptions.CORRELATION_OPTIONS.value[0])
         self.plot_correlation_dropdown.disable()
         self.plot_correlation_clr_dropdown.setChoices(Options.PALETTE_OPTIONS.value[0])
         self.plot_correlation_clr_dropdown.disable()
         self.plots_cb = Checkbutton(self.settings_frm, text='PLOTS', variable=self.plots_var, command=lambda: self.enable_dropdown_from_checkbox(check_box_var=self.plots_var, dropdown_menus=[self.plot_correlation_dropdown, self.plot_correlation_clr_dropdown]))
 
         self.settings_frm.grid(row=1, column=0, sticky=NW)
         self.spearman_cb.grid(row=0, column=0, sticky=NW)
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.58.6/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.58.6/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/.DS_Store`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-00000000: 0000 0001 4275 6431 0000 7800 0000 0800  ....Bud1..x.....
-00000010: 0000 7800 0000 100c 0000 800c 0000 200c  ..x........... .
+00000000: 0000 0001 4275 6431 0000 a000 0000 0800  ....Bud1........
+00000010: 0000 a000 0000 100c 0000 900c 0000 200c  .............. .
 00000020: 0000 300c 0000 0000 0000 0000 0000 0800  ..0.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 00a6  ................
-00000050: 0000 0008 0000 1000 0075 006e 0064 0069  .........u.n.d.i
+00000040: 0000 0000 0000 0003 0000 0001 0000 00ac  ................
+00000050: 0000 0009 0000 1000 0075 006e 0064 0069  .........u.n.d.i
 00000060: 006e 0067 0000 0000 0000 0000 0000 0000  .n.g............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,277 +250,277 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0015 0000 000c  ................
-00001010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-00001020: 0069 0073 0065 0064 6d6f 4444 626c 6f62  .i.s.e.dmoDDblob
-00001030: 0000 0008 644a f89f 34fe c441 0000 000c  ....dJ..4..A....
-00001040: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-00001050: 0069 0073 0065 0064 6d6f 6444 626c 6f62  .i.s.e.dmodDblob
-00001060: 0000 0008 785b 2585 fefd c441 0000 000c  ....x[%....A....
-00001070: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
-00001080: 0069 0073 0065 0064 7068 3153 636f 6d70  .i.s.e.dph1Scomp
-00001090: 0000 0000 0007 4000 0000 000c 0075 006e  ......@......u.n
-000010a0: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
-000010b0: 0065 0064 7653 726e 6c6f 6e67 0000 0001  .e.dvSrnlong....
-000010c0: 0000 0005 0075 0074 0069 006c 0073 6277  .....u.t.i.l.sbw
-000010d0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
-000010e0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
-000010f0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001100: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
-00001110: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00001120: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00001130: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00001140: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001150: 6261 7208 0809 0809 5f10 187b 7b33 3532  bar....._..{{352
-00001160: 2c20 3234 377d 2c20 7b39 3839 2c20 3433  , 247}, {989, 43
-00001170: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
-00001180: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
-00001190: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-000011a0: 0000 9a00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-000011b0: 7364 7363 6c62 6f6f 6c00 0000 0005 0075  sdsclbool......u
-000011c0: 0074 0069 006c 0073 6c67 3153 636f 6d70  .t.i.l.slg1Scomp
-000011d0: 0000 0000 0003 9cc6 0000 0005 0075 0074  .............u.t
-000011e0: 0069 006c 0073 6c73 7643 626c 6f62 0000  .i.l.slsvCblob..
-000011f0: 0297 6270 6c69 7374 3030 d801 0203 0405  ..bplist00......
-00001200: 0607 0809 0a0b 1949 4a0a 4c5f 1012 7669  .......IJ.L_..vi
-00001210: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00001220: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00001230: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00001240: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
-00001250: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
-00001260: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
-00001270: 4461 7465 7358 6963 6f6e 5369 7a65 1001  DatesXiconSize..
-00001280: 09ab 0c15 1d22 262b 3035 3a3f 44d4 0d0e  ....."&+05:?D...
-00001290: 0f10 0a0a 1314 5776 6973 6962 6c65 5961  ......WvisibleYa
-000012a0: 7363 656e 6469 6e67 5577 6964 7468 5a69  scendingUwidthZi
-000012b0: 6465 6e74 6966 6965 7209 0911 0204 546e  dentifier.....Tn
-000012c0: 616d 65d4 1617 1810 191a 191c 5776 6973  ame.........Wvis
-000012d0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-000012e0: 6469 6e67 0810 2308 5875 6269 7175 6974  ding..#.Xubiquit
-000012f0: 79d4 0d0e 0f10 0a19 2021 0908 10b5 5c64  y....... !....\d
-00001300: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
-00001310: 1919 2025 0808 5b64 6174 6543 7265 6174  .. %..[dateCreat
-00001320: 6564 d40d 0e0f 100a 1929 2a09 0810 6154  ed.......)*...aT
-00001330: 7369 7a65 d40d 0e0f 100a 0a2e 2f09 0910  size......../...
-00001340: 7354 6b69 6e64 d40d 0e0f 1019 0a33 3408  sTkind.......34.
-00001350: 0910 6455 6c61 6265 6cd4 0d0e 0f10 190a  ..dUlabel.......
-00001360: 3839 0809 104b 5776 6572 7369 6f6e d40d  89...KWversion..
-00001370: 0e0f 1019 0a3d 3e08 0911 012c 5863 6f6d  .....=>....,Xcom
-00001380: 6d65 6e74 73d4 0d0e 0f10 1919 4243 0808  ments.......BC..
-00001390: 10c8 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-000013a0: 64d4 1617 1810 1920 1947 0808 5964 6174  d...... .G..Ydat
-000013b0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-000013c0: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-000013d0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-000013e0: 8300 8c00 8e00 8f00 9b00 a400 ac00 b600  ................
-000013f0: bc00 c700 c800 c900 cc00 d100 da00 e200  ................
-00001400: e800 f200 f300 f500 f600 ff01 0801 0901  ................
-00001410: 0a01 0c01 1901 2201 2301 2401 3001 3901  ......".#.$.0.9.
-00001420: 3a01 3b01 3d01 4201 4b01 4c01 4d01 4f01  :.;.=.B.K.L.M.O.
-00001430: 5401 5d01 5e01 5f01 6101 6701 7001 7101  T.].^._.a.g.p.q.
-00001440: 7201 7401 7c01 8501 8601 8701 8a01 9301  r.t.|...........
-00001450: 9c01 9d01 9e01 a001 af01 b801 b901 ba01  ................
-00001460: c401 c501 ce01 d301 d400 0000 0000 0002  ................
-00001470: 0100 0000 0000 0000 4d00 0000 0000 0000  ........M.......
-00001480: 0000 0000 0000 0001 dd00 0000 0500 7500  ..............u.
-00001490: 7400 6900 6c00 736c 7376 7062 6c6f 6200  t.i.l.slsvpblob.
-000014a0: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
-000014b0: 0506 0708 090a 0b1d 4546 0a48 5f10 1276  ........EF.H_..v
-000014c0: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-000014d0: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-000014e0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-000014f0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-00001500: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-00001510: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
-00001520: 6544 6174 6573 5869 636f 6e53 697a 6510  eDatesXiconSize.
-00001530: 0109 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
-00001540: 2d32 373c 4158 636f 6d6d 656e 7473 5e64  -27<AXcomments^d
-00001550: 6174 654c 6173 744f 7065 6e65 645b 6461  ateLastOpened[da
-00001560: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-00001570: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-00001580: 6e54 6e61 6d65 5c64 6174 654d 6f64 6966  nTname\dateModif
-00001590: 6965 64d4 1617 1819 1a0a 1c1d 5569 6e64  ied.........Uind
-000015a0: 6578 5961 7363 656e 6469 6e67 5577 6964  exYascendingUwid
-000015b0: 7468 5776 6973 6962 6c65 1007 0911 012c  thWvisible.....,
-000015c0: 08d4 1617 1819 1f1d 211d 1008 0810 c808  ........!.......
-000015d0: d416 1718 1924 1d26 1d10 0208 10b5 08d4  .....$.&........
-000015e0: 1617 1819 291d 2b0a 1003 0810 6109 d416  ....).+.....a...
-000015f0: 1718 192e 0a30 1d10 0509 1064 08d4 1617  .....0.....d....
-00001600: 1819 330a 350a 1004 0910 7309 d416 1718  ..3.5.....s.....
-00001610: 1938 0a3a 1d10 0609 104b 08d4 1617 1819  .8.:.....K......
-00001620: 3d0a 3f0a 1000 0911 0204 09d4 1617 1819  =.?.............
-00001630: 091d 260a 0809 0823 4028 0000 0000 0000  ..&....#@(......
-00001640: 546e 616d 6509 2340 3000 0000 0000 0000  Tname.#@0.......
-00001650: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-00001660: 8300 8c00 8e00 8f00 a200 ab00 ba00 c600  ................
-00001670: cb00 d100 d600 de00 e300 f000 f900 ff01  ................
-00001680: 0901 0f01 1701 1901 1a01 1d01 1e01 2701  ..............'.
-00001690: 2901 2a01 2c01 2d01 3601 3801 3901 3b01  ).*.,.-.6.8.9.;.
-000016a0: 3c01 4501 4701 4801 4a01 4b01 5401 5601  <.E.G.H.J.K.T.V.
-000016b0: 5701 5901 5a01 6301 6501 6601 6801 6901  W.Y.Z.c.e.f.h.i.
-000016c0: 7201 7401 7501 7701 7801 8101 8301 8401  r.t.u.w.x.......
-000016d0: 8701 8801 9101 9201 9301 9401 9d01 a201  ................
-000016e0: a300 0000 0000 0002 0100 0000 0000 0000  ................
-000016f0: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-00001700: ac00 0000 0500 7500 7400 6900 6c00 736d  ......u.t.i.l.sm
-00001710: 6f44 4462 6c6f 6200 0000 0819 6faa 426a  oDDblob.....o.Bj
-00001720: ffc4 4100 0000 0500 7500 7400 6900 6c00  ..A.....u.t.i.l.
-00001730: 736d 6f64 4462 6c6f 6200 0000 08cc dc81  smodDblob.......
-00001740: 8648 fec4 4100 0000 0500 7500 7400 6900  .H..A.....u.t.i.
-00001750: 6c00 7370 6831 5363 6f6d 7000 0000 0000  l.sph1Scomp.....
-00001760: 0420 0000 0000 0500 7500 7400 6900 6c00  . ......u.t.i.l.
-00001770: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
-00001780: 1000 7600 6900 6400 6500 6f00 5f00 7000  ..v.i.d.e.o._.p.
-00001790: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-000017a0: 7362 7773 7062 6c6f 6200 0000 c962 706c  sbwspblob....bpl
-000017b0: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
-000017c0: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-000017d0: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
-000017e0: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-000017f0: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-00001800: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-00001810: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00001820: 6964 6562 6172 0808 0908 095f 1018 7b7b  idebar....._..{{
-00001830: 3335 322c 2032 3437 7d2c 207b 3938 392c  352, 247}, {989,
-00001840: 2034 3336 7d7d 0908 1725 313d 4960 6d79   436}}...%1=I`my
-00001850: 7a7b 7c7d 7e99 0000 0000 0000 0101 0000  z{|}~...........
-00001860: 0000 0000 000f 0000 0000 0000 0000 0000  ................
-00001870: 0000 0000 009a 0000 0010 0076 0069 0064  ...........v.i.d
-00001880: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
-00001890: 0073 0073 006f 0072 0073 6c67 3153 636f  .s.s.o.r.slg1Sco
-000018a0: 6d70 0000 0000 0003 61f1 0000 0010 0076  mp......a......v
-000018b0: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
-000018c0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
-000018d0: 7643 626c 6f62 0000 0307 6270 6c69 7374  vCblob....bplist
-000018e0: 3030 d801 0203 0405 0607 0809 0a0b 1956  00.............V
-000018f0: 570a 5958 6963 6f6e 5369 7a65 5f10 0f73  W.YXiconSize_..s
-00001900: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-00001910: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-00001920: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
-00001930: 697a 655a 736f 7274 436f 6c75 6d6e 5f10  izeZsortColumn_.
-00001940: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-00001950: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
-00001960: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
-00001970: ae0c 151d 2226 2b30 353a 3f44 484d 51d4  ...."&+05:?DHMQ.
-00001980: 0d0e 0f10 1112 0a0a 5a69 6465 6e74 6966  ........Zidentif
-00001990: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
-000019a0: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
-000019b0: 1103 2a09 09d4 1617 180d 191a 191c 5776  ..*...........Wv
-000019c0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-000019d0: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
-000019e0: 6974 79d4 0d0e 0f10 1e1f 190a 5c64 6174  ity.........\dat
-000019f0: 654d 6f64 6966 6965 6410 b508 09d4 0d0e  eModified.......
-00001a00: 0f10 231f 1919 5b64 6174 6543 7265 6174  ..#...[dateCreat
-00001a10: 6564 0808 d40d 0e0f 1027 2819 0a54 7369  ed.......'(..Tsi
-00001a20: 7a65 1061 0809 d40d 0e0f 102c 2d0a 0a54  ze.a.......,-..T
-00001a30: 6b69 6e64 1073 0909 d40d 0e0f 1031 320a  kind.s.......12.
-00001a40: 1955 6c61 6265 6c10 6409 08d4 0d0e 0f10  .Ulabel.d.......
-00001a50: 3637 0a19 5776 6572 7369 6f6e 104b 0908  67..Wversion.K..
-00001a60: d40d 0e0f 103b 3c0a 1958 636f 6d6d 656e  .....;<..Xcommen
-00001a70: 7473 1101 2c09 08d4 0d0e 0f10 4041 1919  ts..,.......@A..
-00001a80: 5e64 6174 654c 6173 744f 7065 6e65 6410  ^dateLastOpened.
-00001a90: c808 08d4 1617 180d 191f 1947 0808 5964  ...........G..Yd
-00001aa0: 6174 6541 6464 6564 d40d 1718 1649 4a19  ateAdded.....IJ.
-00001ab0: 195a 7368 6172 654f 776e 6572 10d2 0808  .ZshareOwner....
-00001ac0: d40d 1718 164e 4a19 195f 100f 7368 6172  .....NJ.._..shar
-00001ad0: 654c 6173 7445 6469 746f 7208 08d4 0d17  eLastEditor.....
-00001ae0: 1816 524a 1919 5f10 1069 6e76 6974 6174  ..RJ.._..invitat
-00001af0: 696f 6e53 7461 7475 7308 0808 2340 2800  ionStatus...#@(.
-00001b00: 0000 0000 0054 6e61 6d65 0910 0100 0800  .....Tname......
-00001b10: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00001b20: 8c00 9500 9600 a500 ae00 b900 bf00 c900  ................
-00001b30: d100 d600 d900 da00 db00 e400 ec00 f200  ................
-00001b40: fc00 fd00 ff01 0001 0901 1201 1f01 2101  ..............!.
-00001b50: 2201 2301 2c01 3801 3901 3a01 4301 4801  ".#.,.8.9.:.C.H.
-00001b60: 4a01 4b01 4c01 5501 5a01 5c01 5d01 5e01  J.K.L.U.Z.\.].^.
-00001b70: 6701 6d01 6f01 7001 7101 7a01 8201 8401  g.m.o.p.q.z.....
-00001b80: 8501 8601 8f01 9801 9b01 9c01 9d01 a601  ................
-00001b90: b501 b701 b801 b901 c201 c301 c401 ce01  ................
-00001ba0: d701 e201 e401 e501 e601 ef02 0102 0202  ................
-00001bb0: 0302 0c02 1f02 2002 2102 2202 2b02 3002  ...... .!.".+.0.
-00001bc0: 3100 0000 0000 0002 0100 0000 0000 0000  1...............
-00001bd0: 5a00 0000 0000 0000 0000 0000 0000 0002  Z...............
-00001be0: 3300 0000 1000 7600 6900 6400 6500 6f00  3.....v.i.d.e.o.
-00001bf0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-00001c00: 6f00 7200 736c 7376 7062 6c6f 6200 0002  o.r.slsvpblob...
-00001c10: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
-00001c20: 0708 090a 0b1a 4647 0a35 5869 636f 6e53  ......FG.5XiconS
-00001c30: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
-00001c40: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00001c50: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00001c60: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00001c70: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00001c80: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
-00001c90: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
-00001ca0: 0000 0000 0000 09d9 0c0d 0e0f 1011 1213  ................
-00001cb0: 1415 1e23 282d 3236 3b40 5863 6f6d 6d65  ...#(-26;@Xcomme
-00001cc0: 6e74 7355 6c61 6265 6c57 7665 7273 696f  ntsUlabelWversio
-00001cd0: 6e5b 6461 7465 4372 6561 7465 6454 7369  n[dateCreatedTsi
-00001ce0: 7a65 5c64 6174 654d 6f64 6966 6965 6454  ze\dateModifiedT
-00001cf0: 6b69 6e64 546e 616d 655e 6461 7465 4c61  kindTname^dateLa
-00001d00: 7374 4f70 656e 6564 d416 1718 191a 1b0a  stOpened........
-00001d10: 1d57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-00001d20: 6173 6365 6e64 696e 6755 696e 6465 7808  ascendingUindex.
-00001d30: 1101 2c09 1007 d416 1718 191a 200a 2208  ..,......... .".
-00001d40: 1064 0910 05d4 1617 1819 1a25 0a27 0810  .d.........%.'..
-00001d50: 4b09 1006 d416 1718 191a 2a1a 2c08 10b5  K.........*.,...
-00001d60: 0810 02d4 1617 1819 0a2f 1a31 0910 6108  ........./.1..a.
-00001d70: 1003 d416 1718 190a 2a1a 3509 0810 01d4  ........*.5.....
-00001d80: 1617 1819 0a38 0a3a 0910 7309 1004 d416  .....8.:..s.....
-00001d90: 1718 190a 3d0a 3f09 1103 2a09 1000 d416  ....=.?...*.....
-00001da0: 1718 191a 421a 4408 10c8 0810 0808 2340  ....B.D.......#@
-00001db0: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
-00001dc0: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00001dd0: 8c00 9500 9600 a900 b200 b800 c000 cc00  ................
-00001de0: d100 de00 e300 e800 f701 0001 0801 0e01  ................
-00001df0: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
-00001e00: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
-00001e10: 4c01 4d01 4f01 5001 5201 5b01 5c01 5e01  L.M.O.P.R.[.\.^.
-00001e20: 5f01 6101 6a01 6b01 6c01 6e01 7701 7801  _.a.j.k.l.n.w.x.
-00001e30: 7a01 7b01 7d01 8601 8701 8a01 8b01 8d01  z.{.}...........
-00001e40: 9601 9701 9901 9a01 9c01 9d01 a601 ab00  ................
-00001e50: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00001e60: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
-00001e70: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-00001e80: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00001e90: 7200 736d 6f44 4462 6c6f 6200 0000 0858  r.smoDDblob....X
-00001ea0: fa45 86d0 fec4 4100 0000 1000 7600 6900  .E....A.....v.i.
-00001eb0: 6400 6500 6f00 5f00 7000 7200 6f00 6300  d.e.o._.p.r.o.c.
-00001ec0: 6500 7300 7300 6f00 7200 736d 6f64 4462  e.s.s.o.r.smodDb
-00001ed0: 6c6f 6200 0000 0858 fa45 86d0 fec4 4100  lob....X.E....A.
-00001ee0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-00001ef0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00001f00: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-00001f10: 0440 0000 0000 1000 7600 6900 6400 6500  .@......v.i.d.e.
-00001f20: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
-00001f30: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
-00001f40: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00001000: 0000 0000 0000 0000 0000 000f 0000 0005  ................
+00001010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
+00001020: 6d70 0000 0000 0003 9e73 0000 0005 0075  mp.......s.....u
+00001030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
+00001040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
+00001050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
+00001060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00001080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000010a0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+000010b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000010c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000010d0: 1001 09ab 0c15 1d22 262b 3035 3a3f 44d4  ......."&+05:?D.
+000010e0: 0d0e 0f10 0a0a 1314 5776 6973 6962 6c65  ........Wvisible
+000010f0: 5961 7363 656e 6469 6e67 5577 6964 7468  YascendingUwidth
+00001100: 5a69 6465 6e74 6966 6965 7209 0911 0204  Zidentifier.....
+00001110: 546e 616d 65d4 1617 1810 191a 191c 5776  Tname.........Wv
+00001120: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00001130: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
+00001140: 6974 79d4 0d0e 0f10 0a19 2021 0908 10b5  ity....... !....
+00001150: 5c64 6174 654d 6f64 6966 6965 64d4 0d0e  \dateModified...
+00001160: 0f10 1919 2025 0808 5b64 6174 6543 7265  .... %..[dateCre
+00001170: 6174 6564 d40d 0e0f 100a 1929 2a09 0810  ated.......)*...
+00001180: 6154 7369 7a65 d40d 0e0f 100a 0a2e 2f09  aTsize......../.
+00001190: 0910 7354 6b69 6e64 d40d 0e0f 1019 0a33  ..sTkind.......3
+000011a0: 3408 0910 6455 6c61 6265 6cd4 0d0e 0f10  4...dUlabel.....
+000011b0: 190a 3839 0809 104b 5776 6572 7369 6f6e  ..89...KWversion
+000011c0: d40d 0e0f 1019 0a3d 3e08 0911 012c 5863  .......=>....,Xc
+000011d0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1919 4243  omments.......BC
+000011e0: 0808 10c8 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
+000011f0: 6e65 64d4 1617 1810 1920 1947 0808 5964  ned...... .G..Yd
+00001200: 6174 6541 6464 6564 0823 4028 0000 0000  ateAdded.#@(....
+00001210: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
+00001220: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+00001230: 7000 8300 8c00 8e00 8f00 9b00 a400 ac00  p...............
+00001240: b600 bc00 c700 c800 c900 cc00 d100 da00  ................
+00001250: e200 e800 f200 f300 f500 f600 ff01 0801  ................
+00001260: 0901 0a01 0c01 1901 2201 2301 2401 3001  ........".#.$.0.
+00001270: 3901 3a01 3b01 3d01 4201 4b01 4c01 4d01  9.:.;.=.B.K.L.M.
+00001280: 4f01 5401 5d01 5e01 5f01 6101 6701 7001  O.T.].^._.a.g.p.
+00001290: 7101 7201 7401 7c01 8501 8601 8701 8a01  q.r.t.|.........
+000012a0: 9301 9c01 9d01 9e01 a001 af01 b801 b901  ................
+000012b0: ba01 c401 c501 ce01 d301 d400 0000 0000  ................
+000012c0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000012d0: 0000 0000 0000 0000 0001 dd00 0000 0500  ................
+000012e0: 7500 7400 6900 6c00 736c 7376 7062 6c6f  u.t.i.l.slsvpblo
+000012f0: 6200 0002 5e62 706c 6973 7430 30d8 0102  b...^bplist00...
+00001300: 0304 0506 0708 090a 0b1d 4546 0a48 5f10  ..........EF.H_.
+00001310: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00001320: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+00001330: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00001340: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00001350: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
+00001360: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
+00001370: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
+00001380: 6510 0109 d90c 0d0e 0f10 1112 1314 151e  e...............
+00001390: 2328 2d32 373c 4158 636f 6d6d 656e 7473  #(-27<AXcomments
+000013a0: 5e64 6174 654c 6173 744f 7065 6e65 645b  ^dateLastOpened[
+000013b0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+000013c0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+000013d0: 696f 6e54 6e61 6d65 5c64 6174 654d 6f64  ionTname\dateMod
+000013e0: 6966 6965 64d4 1617 1819 1a0a 1c1d 5569  ified.........Ui
+000013f0: 6e64 6578 5961 7363 656e 6469 6e67 5577  ndexYascendingUw
+00001400: 6964 7468 5776 6973 6962 6c65 1007 0911  idthWvisible....
+00001410: 012c 08d4 1617 1819 1f1d 211d 1008 0810  .,........!.....
+00001420: c808 d416 1718 1924 1d26 1d10 0208 10b5  .......$.&......
+00001430: 08d4 1617 1819 291d 2b0a 1003 0810 6109  ......).+.....a.
+00001440: d416 1718 192e 0a30 1d10 0509 1064 08d4  .......0.....d..
+00001450: 1617 1819 330a 350a 1004 0910 7309 d416  ....3.5.....s...
+00001460: 1718 1938 0a3a 1d10 0609 104b 08d4 1617  ...8.:.....K....
+00001470: 1819 3d0a 3f0a 1000 0911 0204 09d4 1617  ..=.?...........
+00001480: 1819 091d 260a 0809 0823 4028 0000 0000  ....&....#@(....
+00001490: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
+000014a0: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+000014b0: 7000 8300 8c00 8e00 8f00 a200 ab00 ba00  p...............
+000014c0: c600 cb00 d100 d600 de00 e300 f000 f900  ................
+000014d0: ff01 0901 0f01 1701 1901 1a01 1d01 1e01  ................
+000014e0: 2701 2901 2a01 2c01 2d01 3601 3801 3901  '.).*.,.-.6.8.9.
+000014f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
+00001500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
+00001510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
+00001520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
+00001530: a201 a300 0000 0000 0002 0100 0000 0000  ................
+00001540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
+00001550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
+00001560: 736d 6f44 4462 6c6f 6200 0000 0814 4083  smoDDblob.....@.
+00001570: 1561 01c5 4100 0000 0500 7500 7400 6900  .a..A.....u.t.i.
+00001580: 6c00 736d 6f64 4462 6c6f 6200 0000 08cc  l.smodDblob.....
+00001590: dc81 8648 fec4 4100 0000 0500 7500 7400  ...H..A.....u.t.
+000015a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
+000015b0: 0000 0420 0000 0000 0500 7500 7400 6900  ... ......u.t.i.
+000015c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
+000015d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
+000015e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+000015f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
+00001600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00001610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00001620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00001630: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00001640: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00001650: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00001660: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00001670: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
+00001680: 7b7b 3335 322c 2032 3437 7d2c 207b 3938  {{352, 247}, {98
+00001690: 392c 2034 3336 7d7d 0908 1725 313d 4960  9, 436}}...%1=I`
+000016a0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
+000016b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+000016c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
+000016d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
+000016e0: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
+000016f0: 636f 6d70 0000 0000 0003 61f1 0000 0010  comp......a.....
+00001700: 0076 0069 0064 0065 006f 005f 0070 0072  .v.i.d.e.o._.p.r
+00001710: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
+00001720: 6c73 7643 626c 6f62 0000 0307 6270 6c69  lsvCblob....bpli
+00001730: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00001740: 1956 570a 5958 6963 6f6e 5369 7a65 5f10  .VW.YXiconSize_.
+00001750: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001760: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00001770: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00001780: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00001790: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+000017a0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+000017b0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+000017c0: 0009 ae0c 151d 2226 2b30 353a 3f44 484d  ......"&+05:?DHM
+000017d0: 51d4 0d0e 0f10 1112 0a0a 5a69 6465 6e74  Q.........Zident
+000017e0: 6966 6965 7255 7769 6474 6859 6173 6365  ifierUwidthYasce
+000017f0: 6e64 696e 6757 7669 7369 626c 6554 6e61  ndingWvisibleTna
+00001800: 6d65 1103 2a09 09d4 1617 180d 191a 191c  me..*...........
+00001810: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00001820: 7363 656e 6469 6e67 0810 2308 5875 6269  scending..#.Xubi
+00001830: 7175 6974 79d4 0d0e 0f10 1e1f 190a 5c64  quity.........\d
+00001840: 6174 654d 6f64 6966 6965 6410 b508 09d4  ateModified.....
+00001850: 0d0e 0f10 231f 1919 5b64 6174 6543 7265  ....#...[dateCre
+00001860: 6174 6564 0808 d40d 0e0f 1027 2819 0a54  ated.......'(..T
+00001870: 7369 7a65 1061 0809 d40d 0e0f 102c 2d0a  size.a.......,-.
+00001880: 0a54 6b69 6e64 1073 0909 d40d 0e0f 1031  .Tkind.s.......1
+00001890: 320a 1955 6c61 6265 6c10 6409 08d4 0d0e  2..Ulabel.d.....
+000018a0: 0f10 3637 0a19 5776 6572 7369 6f6e 104b  ..67..Wversion.K
+000018b0: 0908 d40d 0e0f 103b 3c0a 1958 636f 6d6d  .......;<..Xcomm
+000018c0: 656e 7473 1101 2c09 08d4 0d0e 0f10 4041  ents..,.......@A
+000018d0: 1919 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+000018e0: 6410 c808 08d4 1617 180d 191f 1947 0808  d............G..
+000018f0: 5964 6174 6541 6464 6564 d40d 1718 1649  YdateAdded.....I
+00001900: 4a19 195a 7368 6172 654f 776e 6572 10d2  J..ZshareOwner..
+00001910: 0808 d40d 1718 164e 4a19 195f 100f 7368  .......NJ.._..sh
+00001920: 6172 654c 6173 7445 6469 746f 7208 08d4  areLastEditor...
+00001930: 0d17 1816 524a 1919 5f10 1069 6e76 6974  ....RJ.._..invit
+00001940: 6174 696f 6e53 7461 7475 7308 0808 2340  ationStatus...#@
+00001950: 2800 0000 0000 0054 6e61 6d65 0910 0100  (......Tname....
+00001960: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
+00001970: 7700 8c00 9500 9600 a500 ae00 b900 bf00  w...............
+00001980: c900 d100 d600 d900 da00 db00 e400 ec00  ................
+00001990: f200 fc00 fd00 ff01 0001 0901 1201 1f01  ................
+000019a0: 2101 2201 2301 2c01 3801 3901 3a01 4301  !.".#.,.8.9.:.C.
+000019b0: 4801 4a01 4b01 4c01 5501 5a01 5c01 5d01  H.J.K.L.U.Z.\.].
+000019c0: 5e01 6701 6d01 6f01 7001 7101 7a01 8201  ^.g.m.o.p.q.z...
+000019d0: 8401 8501 8601 8f01 9801 9b01 9c01 9d01  ................
+000019e0: a601 b501 b701 b801 b901 c201 c301 c401  ................
+000019f0: ce01 d701 e201 e401 e501 e601 ef02 0102  ................
+00001a00: 0202 0302 0c02 1f02 2002 2102 2202 2b02  ........ .!.".+.
+00001a10: 3002 3100 0000 0000 0002 0100 0000 0000  0.1.............
+00001a20: 0000 5a00 0000 0000 0000 0000 0000 0000  ..Z.............
+00001a30: 0002 3300 0000 1000 7600 6900 6400 6500  ..3.....v.i.d.e.
+00001a40: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
+00001a50: 7300 6f00 7200 736c 7376 7062 6c6f 6200  s.o.r.slsvpblob.
+00001a60: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
+00001a70: 0506 0708 090a 0b1a 4647 0a35 5869 636f  ........FG.5Xico
+00001a80: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
+00001a90: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00001aa0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00001ab0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00001ac0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+00001ad0: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
+00001ae0: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
+00001af0: 4030 0000 0000 0000 09d9 0c0d 0e0f 1011  @0..............
+00001b00: 1213 1415 1e23 282d 3236 3b40 5863 6f6d  .....#(-26;@Xcom
+00001b10: 6d65 6e74 7355 6c61 6265 6c57 7665 7273  mentsUlabelWvers
+00001b20: 696f 6e5b 6461 7465 4372 6561 7465 6454  ion[dateCreatedT
+00001b30: 7369 7a65 5c64 6174 654d 6f64 6966 6965  size\dateModifie
+00001b40: 6454 6b69 6e64 546e 616d 655e 6461 7465  dTkindTname^date
+00001b50: 4c61 7374 4f70 656e 6564 d416 1718 191a  LastOpened......
+00001b60: 1b0a 1d57 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
+00001b70: 6859 6173 6365 6e64 696e 6755 696e 6465  hYascendingUinde
+00001b80: 7808 1101 2c09 1007 d416 1718 191a 200a  x...,......... .
+00001b90: 2208 1064 0910 05d4 1617 1819 1a25 0a27  "..d.........%.'
+00001ba0: 0810 4b09 1006 d416 1718 191a 2a1a 2c08  ..K.........*.,.
+00001bb0: 10b5 0810 02d4 1617 1819 0a2f 1a31 0910  .........../.1..
+00001bc0: 6108 1003 d416 1718 190a 2a1a 3509 0810  a.........*.5...
+00001bd0: 01d4 1617 1819 0a38 0a3a 0910 7309 1004  .......8.:..s...
+00001be0: d416 1718 190a 3d0a 3f09 1103 2a09 1000  ......=.?...*...
+00001bf0: d416 1718 191a 421a 4408 10c8 0810 0808  ......B.D.......
+00001c00: 2340 2800 0000 0000 0054 6e61 6d65 0900  #@(......Tname..
+00001c10: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
+00001c20: 7700 8c00 9500 9600 a900 b200 b800 c000  w...............
+00001c30: cc00 d100 de00 e300 e800 f701 0001 0801  ................
+00001c40: 0e01 1801 1e01 1f01 2201 2301 2501 2e01  ........".#.%...
+00001c50: 2f01 3101 3201 3401 3d01 3e01 4001 4101  /.1.2.4.=.>.@.A.
+00001c60: 4301 4c01 4d01 4f01 5001 5201 5b01 5c01  C.L.M.O.P.R.[.\.
+00001c70: 5e01 5f01 6101 6a01 6b01 6c01 6e01 7701  ^._.a.j.k.l.n.w.
+00001c80: 7801 7a01 7b01 7d01 8601 8701 8a01 8b01  x.z.{.}.........
+00001c90: 8d01 9601 9701 9901 9a01 9c01 9d01 a601  ................
+00001ca0: ab00 0000 0000 0002 0100 0000 0000 0000  ................
+00001cb0: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
+00001cc0: ac00 0000 1000 7600 6900 6400 6500 6f00  ......v.i.d.e.o.
+00001cd0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00001ce0: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
+00001cf0: 0858 fa45 86d0 fec4 4100 0000 1000 7600  .X.E....A.....v.
+00001d00: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
+00001d10: 6300 6500 7300 7300 6f00 7200 736d 6f64  c.e.s.s.o.r.smod
+00001d20: 4462 6c6f 6200 0000 0858 fa45 86d0 fec4  Dblob....X.E....
+00001d30: 4100 0000 1000 7600 6900 6400 6500 6f00  A.....v.i.d.e.o.
+00001d40: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00001d50: 6f00 7200 7370 6831 5363 6f6d 7000 0000  o.r.sph1Scomp...
+00001d60: 0000 0440 0000 0000 1000 7600 6900 6400  ...@......v.i.d.
+00001d70: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
+00001d80: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
+00001d90: 6700 0000 0100 0000 0000 0000 0000 0000  g...............
+00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0016 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0042 0218 0000 000b 005f 005f 0070  ...B......._._.p
+00002030: 0000 0042 034e 0000 000b 005f 005f 0070  ...B.N....._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 be68 6b6a  moDDblob.....hkj
-00002060: 58ff c441 0000 000b 005f 005f 0070 0079  X..A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 d651 eebb  moDDblob.....Q..
+00002060: 6401 c541 0000 000b 005f 005f 0070 0079  d..A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 be68 6b6a 58ff  dDblob.....hkjX.
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 004f e000 0000 0006  comp.....O......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
@@ -724,53 +724,53 @@
 00002d30: 0110 011c 011d 011e 0127 012c 012e 012f  .........'.,.../
 00002d40: 0130 0139 013e 0140 0141 0142 014b 0151  .0.9.>.@.A.B.K.Q
 00002d50: 0153 0154 0155 015e 0166 0168 0169 016a  .S.T.U.^.f.h.i.j
 00002d60: 0173 017c 017f 0180 0181 018a 0199 019b  .s.|............
 00002d70: 019c 019d 01a6 01b0 01b1 01b2 01b3 01bc  ................
 00002d80: 01c1 01c2 0000 0000 0000 0201 0000 0000  ................
 00002d90: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-00002da0: 0000 01c4 421a 4408 10c8 0810 0808 2340  ....B.D.......#@
-00002db0: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
-00002dc0: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00002dd0: 8c00 9500 9600 a900 b200 b800 c000 cc00  ................
-00002de0: d100 de00 e300 e800 f701 0001 0801 0e01  ................
-00002df0: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
-00002e00: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
-00002e10: 4c01 4d01 4f01 5001 5201 5b01 5c01 5e01  L.M.O.P.R.[.\.^.
-00002e20: 5f01 6101 6a01 6b01 6c01 6e01 7701 7801  _.a.j.k.l.n.w.x.
-00002e30: 7a01 7b01 7d01 8601 8701 8a01 8b01 8d01  z.{.}...........
-00002e40: 9601 9701 9901 9a01 9c01 9d01 a601 ab00  ................
-00002e50: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-00002e60: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
-00002e70: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-00002e80: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00002e90: 7200 736d 6f44 4462 6c6f 6200 0000 0858  r.smoDDblob....X
-00002ea0: fa45 86d0 fec4 4100 0000 1000 7600 6900  .E....A.....v.i.
-00002eb0: 6400 6500 6f00 5f00 7000 7200 6f00 6300  d.e.o._.p.r.o.c.
-00002ec0: 6500 7300 7300 6f00 7200 736d 6f64 4462  e.s.s.o.r.smodDb
-00002ed0: 6c6f 6200 0000 0858 fa45 86d0 fec4 4100  lob....X.E....A.
-00002ee0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-00002ef0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-00002f00: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-00002f10: 0440 0000 0000 1000 7600 6900 6400 6500  .@......v.i.d.e.
-00002f20: 6f00 5f00 7000 7200 6f00 6300 6500 7300  o._.p.r.o.c.e.s.
-00002f30: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
-00002f40: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00002da0: 0000 01c4 0000 0000 0000 0000 0000 0000  ................
+00002db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003000: 0000 0000 0000 0000 0000 0022 0000 0012  ..........."....
+00003000: 0000 0000 0000 0000 0000 0023 0000 0012  ...........#....
 00003010: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 00003020: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 00003030: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
 00003040: d59a 2b59 34fe c441 0000 0012 0062 006f  ..+Y4..A.....b.o
 00003050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
 00003060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
 00003070: 6d6f 6444 626c 6f62 0000 0008 180d d46b  modDblob.......k
@@ -798,25 +798,25 @@
 000031d0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 000031e0: 0000 0000 0000 9a00 0000 0f00 6300 7500  ............c.u.
 000031f0: 6500 5f00 6c00 6900 6700 6800 7400 5f00  e._.l.i.g.h.t._.
 00003200: 7400 6f00 6f00 6c00 7364 7363 6c62 6f6f  t.o.o.l.sdsclboo
 00003210: 6c00 0000 000f 0063 0075 0065 005f 006c  l......c.u.e._.l
 00003220: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00003230: 006c 0073 6c67 3153 636f 6d70 0000 0000  .l.slg1Scomp....
-00003240: 0001 dbdd 0000 000f 0063 0075 0065 005f  .........c.u.e._
+00003240: 0001 d866 0000 000f 0063 0075 0065 005f  ...f.....c.u.e._
 00003250: 006c 0069 0067 0068 0074 005f 0074 006f  .l.i.g.h.t._.t.o
 00003260: 006f 006c 0073 6d6f 4444 626c 6f62 0000  .o.l.smoDDblob..
-00003270: 0008 99e3 9c22 d6fe c441 0000 000f 0063  ....."...A.....c
+00003270: 0008 2402 2eb2 2800 c541 0000 000f 0063  ..$...(..A.....c
 00003280: 0075 0065 005f 006c 0069 0067 0068 0074  .u.e._.l.i.g.h.t
 00003290: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
-000032a0: 626c 6f62 0000 0008 95af cbc6 2afc c441  blob........*..A
+000032a0: 626c 6f62 0000 0008 2402 2eb2 2800 c541  blob....$...(..A
 000032b0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
 000032c0: 0067 0068 0074 005f 0074 006f 006f 006c  .g.h.t._.t.o.o.l
 000032d0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
-000032e0: 5000 0000 000f 0063 0075 0065 005f 006c  P......c.u.e._.l
+000032e0: 6000 0000 000f 0063 0075 0065 005f 006c  `......c.u.e._.l
 000032f0: 0069 0067 0068 0074 005f 0074 006f 006f  .i.g.h.t._.t.o.o
 00003300: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 00003310: 0000 0008 0064 0061 0073 0068 005f 0061  .....d.a.s.h._.a
 00003320: 0070 0070 6277 7370 626c 6f62 0000 00c9  .p.pbwspblob....
 00003330: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 00003340: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 00003350: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
@@ -858,25 +858,25 @@
 00003590: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000035a0: 0000 0000 0000 009a 0000 000f 0064 0061  .............d.a
 000035b0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 000035c0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
 000035d0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
 000035e0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 000035f0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
-00003600: 0000 02be e200 0000 0f00 6400 6100 7400  ..........d.a.t.
+00003600: 0000 02c7 4300 0000 0f00 6400 6100 7400  ....C.....d.a.t.
 00003610: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00003620: 7300 6f00 7200 736d 6f44 4462 6c6f 6200  s.o.r.smoDDblob.
-00003630: 0000 08d4 7456 86d0 fec4 4100 0000 0f00  ....tV....A.....
+00003630: 0000 080d 4b59 4254 01c5 4100 0000 0f00  ....KYBT..A.....
 00003640: 6400 6100 7400 6100 5f00 7000 7200 6f00  d.a.t.a._.p.r.o.
 00003650: 6300 6500 7300 7300 6f00 7200 736d 6f64  c.e.s.s.o.r.smod
-00003660: 4462 6c6f 6200 0000 08d4 7456 86d0 fec4  Dblob.....tV....
+00003660: 4462 6c6f 6200 0000 08d8 72d8 a8f8 ffc4  Dblob.....r.....
 00003670: 4100 0000 0f00 6400 6100 7400 6100 5f00  A.....d.a.t.a._.
 00003680: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 00003690: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-000036a0: 0380 0000 0000 0f00 6400 6100 7400 6100  ........d.a.t.a.
+000036a0: 0390 0000 0000 0f00 6400 6100 7400 6100  ........d.a.t.a.
 000036b0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 000036c0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000036d0: 0100 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 000036e0: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 000036f0: 6300 7400 6f00 7200 7362 7773 7062 6c6f  c.t.o.r.sbwspblo
 00003700: 6200 0000 c862 706c 6973 7430 30d7 0102  b....bplist00...
 00003710: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
@@ -893,15 +893,15 @@
 000037c0: 0000 0000 0000 0000 0000 0000 9900 0000  ................
 000037d0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000037e0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000037f0: 6f00 7200 7364 7363 6c62 6f6f 6c00 0000  o.r.sdsclbool...
 00003800: 0012 0066 0065 0061 0074 0075 0072 0065  ...f.e.a.t.u.r.e
 00003810: 005f 0065 0078 0074 0072 0061 0063 0074  ._.e.x.t.r.a.c.t
 00003820: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00003830: 0000 0013 4e6b 0000 0012 0066 0065 0061  ....Nk.....f.e.a
+00003830: 0000 0013 573f 0000 0012 0066 0065 0061  ....W?.....f.e.a
 00003840: 0074 0075 0072 0065 005f 0065 0078 0074  .t.u.r.e._.e.x.t
 00003850: 0072 0061 0063 0074 006f 0072 0073 6c73  .r.a.c.t.o.r.sls
 00003860: 7643 626c 6f62 0000 02b8 6270 6c69 7374  vCblob....bplist
 00003870: 3030 da01 0203 0405 0607 0809 0a0b 0c0d  00..............
 00003880: 1a48 4948 4a4b 0c5f 1012 7669 6577 4f70  .HIHJK._..viewOp
 00003890: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
 000038a0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
@@ -988,1318 +988,1702 @@
 00003db0: 9901 9a01 9c01 a501 a601 a801 a901 ab01  ................
 00003dc0: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
 00003dd0: db01 e400 0000 0000 0002 0100 0000 0000  ................
 00003de0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 00003df0: 0001 e500 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
 00003e00: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00003e10: 6100 6300 7400 6f00 7200 736d 6f44 4462  a.c.t.o.r.smoDDb
-00003e20: 6c6f 6200 0000 0850 5de5 842e fec4 4100  lob....P].....A.
+00003e20: 6c6f 6200 0000 0866 04c9 1d50 01c5 4100  lob....f...P..A.
 00003e30: 0000 1200 6600 6500 6100 7400 7500 7200  ....f.e.a.t.u.r.
 00003e40: 6500 5f00 6500 7800 7400 7200 6100 6300  e._.e.x.t.r.a.c.
 00003e50: 7400 6f00 7200 736d 6f64 4462 6c6f 6200  t.o.r.smodDblob.
 00003e60: 0000 082d e1ee 5c25 fec4 4100 0000 1200  ...-..\%..A.....
 00003e70: 6600 6500 6100 7400 7500 7200 6500 5f00  f.e.a.t.u.r.e._.
 00003e80: 6500 7800 7400 7200 6100 6300 7400 6f00  e.x.t.r.a.c.t.o.
 00003e90: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
 00003ea0: 15d0 0000 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
 00003eb0: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00003ec0: 6100 6300 7400 6f00 7200 7376 5372 6e6c  a.c.t.o.r.svSrnl
 00003ed0: 6f6e 6700 0000 0100 0000 0900 6c00 6100  ong.........l.a.
 00003ee0: 6200 6500 6c00 6c00 6900 6e00 6762 7773  b.e.l.l.i.n.gbws
-00003ef0: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
+00003ef0: 7062 6c6f 6200 0000 c662 706c 6973 7430  pblob....bplist0
 00003f00: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
 00003f10: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
 00003f20: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
 00003f30: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
 00003f40: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
 00003f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
 00003f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00003f70: 6172 0808 0908 095f 1018 7b7b 3635 372c  ar....._..{{657,
-00003f80: 2032 3730 7d2c 207b 3938 392c 2034 3336   270}, {989, 436
-00003f90: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00003fa0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-00003fb0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00003fc0: 009a 0000 0000 0000 0000 0000 0000 0000  ................
-00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f70: 6172 0808 0908 095f 1015 7b7b 302c 2030  ar....._..{{0, 0
+00003f80: 7d2c 207b 3134 3430 2c20 3837 377d 7d09  }, {1440, 877}}.
+00003f90: 0817 2531 3d49 606d 797a 7b7c 7d7e 9600  ..%1=I`myz{|}~..
+00003fa0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00003fb0: 0000 0000 0000 0000 0000 0000 0000 9700  ................
+00003fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00003fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00003fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
 00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004000: 0000 0000 0000 0000 0000 001b 0000 0009  ................
+00004000: 0000 0000 0000 0000 0000 0016 0000 0009  ................
 00004010: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
-00004020: 0067 6d6f 4444 626c 6f62 0000 0008 ab68  .gmoDDblob.....h
-00004030: b87c d5fe c441 0000 0009 006c 0061 0062  .|...A.....l.a.b
-00004040: 0065 006c 006c 0069 006e 0067 6d6f 6444  .e.l.l.i.n.gmodD
-00004050: 626c 6f62 0000 0008 cb5b 96d0 97fe c441  blob.....[.....A
-00004060: 0000 0009 006c 0061 0062 0065 006c 006c  .....l.a.b.e.l.l
-00004070: 0069 006e 0067 7068 3153 636f 6d70 0000  .i.n.gph1Scomp..
-00004080: 0000 0001 c000 0000 0009 006c 0061 0062  ...........l.a.b
-00004090: 0065 006c 006c 0069 006e 0067 7653 726e  .e.l.l.i.n.gvSrn
-000040a0: 6c6f 6e67 0000 0001 0000 0006 006d 0069  long.........m.i
-000040b0: 0078 0069 006e 0073 6277 7370 626c 6f62  .x.i.n.sbwspblob
-000040c0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
-000040d0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-000040e0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-000040f0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00004100: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00004110: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00004120: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00004130: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00004140: 0809 5f10 187b 7b33 3934 2c20 3138 317d  .._..{{394, 181}
-00004150: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
-00004160: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-00004170: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00004180: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-00004190: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
-000041a0: 5363 6f6d 7000 0000 0000 0942 0900 0000  Scomp......B....
-000041b0: 0600 6d00 6900 7800 6900 6e00 736d 6f44  ..m.i.x.i.n.smoD
-000041c0: 4462 6c6f 6200 0000 0840 a297 bc97 ffc4  Dblob....@......
-000041d0: 4100 0000 0600 6d00 6900 7800 6900 6e00  A.....m.i.x.i.n.
-000041e0: 736d 6f64 4462 6c6f 6200 0000 0846 c34b  smodDblob....F.K
-000041f0: 7784 ffc4 4100 0000 0600 6d00 6900 7800  w...A.....m.i.x.
-00004200: 6900 6e00 7370 6831 5363 6f6d 7000 0000  i.n.sph1Scomp...
-00004210: 0000 0a00 0000 0000 0600 6d00 6900 7800  ..........m.i.x.
-00004220: 6900 6e00 7376 5372 6e6c 6f6e 6700 0000  i.n.svSrnlong...
-00004230: 0100 0000 0500 6d00 6f00 6400 6500 6c62  ......m.o.d.e.lb
-00004240: 7773 7062 6c6f 6200 0000 c962 706c 6973  wspblob....bplis
-00004250: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
-00004260: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00004270: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
-00004280: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00004290: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-000042a0: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-000042b0: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-000042c0: 6562 6172 0808 0908 095f 1018 7b7b 3635  ebar....._..{{65
-000042d0: 372c 2032 3730 7d2c 207b 3938 392c 2034  7, 270}, {989, 4
-000042e0: 3336 7d7d 0908 1725 313d 4960 6d79 7a7b  36}}...%1=I`myz{
-000042f0: 7c7d 7e99 0000 0000 0000 0101 0000 0000  |}~.............
-00004300: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-00004310: 0000 009a 0000 0005 006d 006f 0064 0065  .........m.o.d.e
-00004320: 006c 6c67 3153 636f 6d70 0000 0000 0001  .llg1Scomp......
-00004330: 13d4 0000 0005 006d 006f 0064 0065 006c  .......m.o.d.e.l
-00004340: 6d6f 4444 626c 6f62 0000 0008 e8d9 3f86  moDDblob......?.
-00004350: d0fe c441 0000 0005 006d 006f 0064 0065  ...A.....m.o.d.e
-00004360: 006c 6d6f 6444 626c 6f62 0000 0008 e8d9  .lmodDblob......
-00004370: 3f86 d0fe c441 0000 0005 006d 006f 0064  ?....A.....m.o.d
-00004380: 0065 006c 7068 3153 636f 6d70 0000 0000  .e.lph1Scomp....
-00004390: 0001 4000 0000 0005 006d 006f 0064 0065  ..@......m.o.d.e
-000043a0: 006c 7653 726e 6c6f 6e67 0000 0001 0000  .lvSrnlong......
-000043b0: 000d 006f 0075 0074 006c 0069 0065 0072  ...o.u.t.l.i.e.r
-000043c0: 005f 0074 006f 006f 006c 0073 6277 7370  ._.t.o.o.l.sbwsp
-000043d0: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
-000043e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-000043f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00004400: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00004410: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00004420: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00004430: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00004440: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00004450: 7208 0809 0809 5f10 187b 7b33 3934 2c20  r....._..{{394, 
-00004460: 3138 317d 2c20 7b37 3730 2c20 3433 367d  181}, {770, 436}
-00004470: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00004480: 9900 0000 0000 0001 0100 0000 0000 0000  ................
-00004490: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-000044a0: 9a00 0000 0d00 6f00 7500 7400 6c00 6900  ......o.u.t.l.i.
-000044b0: 6500 7200 5f00 7400 6f00 6f00 6c00 736c  e.r._.t.o.o.l.sl
-000044c0: 6731 5363 6f6d 7000 0000 0000 012d 2d00  g1Scomp......--.
-000044d0: 0000 0d00 6f00 7500 7400 6c00 6900 6500  ....o.u.t.l.i.e.
-000044e0: 7200 5f00 7400 6f00 6f00 6c00 736c 7376  r._.t.o.o.l.slsv
-000044f0: 4362 6c6f 6200 0002 af62 706c 6973 7430  Cblob....bplist0
-00004500: 30da 0102 0304 0506 0708 090a 0b0c 0d1a  0...............
-00004510: 4849 484a 0c4c 5869 636f 6e53 697a 655f  HIHJ.LXiconSize_
-00004520: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-00004530: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00004540: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
-00004550: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
-00004560: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
-00004570: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00004580: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00004590: 6976 6544 6174 6573 5f10 1276 6965 774f  iveDates_..viewO
-000045a0: 7074 696f 6e73 5665 7273 696f 6e23 4030  ptionsVersion#@0
-000045b0: 0000 0000 0000 09ab 0e17 1c21 252a 2f34  ...........!%*/4
-000045c0: 393e 43d4 0f10 1112 0c14 0c16 5776 6973  9>C.........Wvis
-000045d0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-000045e0: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
-000045f0: 10f0 0954 6e61 6d65 d412 1011 0f18 191a  ...Tname........
-00004600: 1a58 7562 6971 7569 7479 1023 0808 d412  .Xubiquity.#....
-00004610: 1011 0f1d 1e1a 0c5c 6461 7465 4d6f 6469  .......\dateModi
-00004620: 6669 6564 10b5 0809 d412 1011 0f22 1e1a  fied........."..
-00004630: 1a5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
-00004640: 1210 110f 2627 1a0c 5473 697a 6510 6108  ....&'..Tsize.a.
-00004650: 09d4 1210 110f 2b2c 0c0c 546b 696e 6410  ......+,..Tkind.
-00004660: 7309 09d4 1210 110f 3031 0c1a 556c 6162  s.......01..Ulab
-00004670: 656c 1064 0908 d412 1011 0f35 360c 1a57  el.d.......56..W
-00004680: 7665 7273 696f 6e10 4b09 08d4 1210 110f  version.K.......
-00004690: 3a3b 0c1a 5863 6f6d 6d65 6e74 7311 012c  :;..Xcomments..,
-000046a0: 0908 d412 1011 0f3f 401a 1a5e 6461 7465  .......?@..^date
-000046b0: 4c61 7374 4f70 656e 6564 10c8 0808 d412  LastOpened......
-000046c0: 1011 0f44 1e1a 1a59 6461 7465 4164 6465  ...D...YdateAdde
-000046d0: 6408 0808 2300 0000 0000 0000 0023 4028  d...#........#@(
-000046e0: 0000 0000 0000 546e 616d 6509 1001 0008  ......Tname.....
-000046f0: 001d 0026 0038 0040 0054 0066 006f 0081  ...&.8.@.T.f.o..
-00004700: 008c 009f 00b4 00bd 00be 00ca 00d3 00db  ................
-00004710: 00e1 00eb 00f6 00f7 00f9 00fa 00ff 0108  ................
-00004720: 0111 0113 0114 0115 011e 012b 012d 012e  ...........+.-..
-00004730: 012f 0138 0144 0145 0146 014f 0154 0156  ./.8.D.E.F.O.T.V
-00004740: 0157 0158 0161 0166 0168 0169 016a 0173  .W.X.a.f.h.i.j.s
-00004750: 0179 017b 017c 017d 0186 018e 0190 0191  .y.{.|.}........
-00004760: 0192 019b 01a4 01a7 01a8 01a9 01b2 01c1  ................
-00004770: 01c3 01c4 01c5 01ce 01d8 01d9 01da 01db  ................
-00004780: 01e4 01ed 01f2 01f3 0000 0000 0000 0201  ................
-00004790: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
-000047a0: 0000 0000 0000 01f5 0000 000d 006f 0075  .............o.u
-000047b0: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
-000047c0: 006f 006c 0073 6c73 7670 626c 6f62 0000  .o.l.slsvpblob..
-000047d0: 0294 6270 6c69 7374 3030 da01 0203 0405  ..bplist00......
-000047e0: 0607 0809 0a0b 0c0d 1c48 4948 4a0c 2958  .........HIHJ.)X
-000047f0: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
-00004800: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00004810: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00004820: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
-00004830: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
-00004840: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
-00004850: 6f6e 585a 736f 7274 436f 6c75 6d6e 5f10  onXZsortColumn_.
-00004860: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-00004870: 735f 1012 7669 6577 4f70 7469 6f6e 7356  s_..viewOptionsV
-00004880: 6572 7369 6f6e 2340 3000 0000 0000 0009  ersion#@0.......
-00004890: d90e 0f10 1112 1314 1516 1720 252a 2e33  ........... %*.3
-000048a0: 383d 4258 636f 6d6d 656e 7473 5e64 6174  8=BXcomments^dat
-000048b0: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
-000048c0: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
-000048d0: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
-000048e0: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
-000048f0: 65d4 1819 1a1b 1c1d 0c1f 5776 6973 6962  e.........Wvisib
-00004900: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
-00004910: 6e67 5569 6e64 6578 0811 012c 0910 07d4  ngUindex...,....
-00004920: 1819 1a1b 1c22 1c24 0810 c808 1008 d418  .....".$........
-00004930: 191a 1b0c 271c 2909 10b5 0810 01d4 1819  ....'.).........
-00004940: 1a1b 1c27 1c2d 0808 1002 d418 191a 1b0c  ...'.-..........
-00004950: 301c 3209 1061 0810 03d4 1819 1a1b 1c35  0.2..a.........5
-00004960: 0c37 0810 6409 1005 d418 191a 1b0c 3a0c  .7..d.........:.
-00004970: 3c09 1073 0910 04d4 1819 1a1b 1c3f 0c41  <..s.........?.A
-00004980: 0810 4b09 1006 d41b 191a 1843 440c 0c10  ..K........CD...
-00004990: 0010 f009 0908 2300 0000 0000 0000 0023  ......#........#
-000049a0: 4028 0000 0000 0000 546e 616d 6509 0008  @(......Tname...
-000049b0: 001d 0026 0038 0040 0054 0066 006f 0081  ...&.8.@.T.f.o..
-000049c0: 008c 009f 00b4 00bd 00be 00d1 00da 00e9  ................
-000049d0: 00f6 0102 0107 010d 0112 011a 011f 0128  ...............(
-000049e0: 0130 0136 0140 0146 0147 014a 014b 014d  .0.6.@.F.G.J.K.M
-000049f0: 0156 0157 0159 015a 015c 0165 0166 0168  .V.W.Y.Z.\.e.f.h
-00004a00: 0169 016b 0174 0175 0176 0178 0181 0182  .i.k.t.u.v.x....
-00004a10: 0184 0185 0187 0190 0191 0193 0194 0196  ................
-00004a20: 019f 01a0 01a2 01a3 01a5 01ae 01af 01b1  ................
-00004a30: 01b2 01b4 01bd 01bf 01c1 01c2 01c3 01c4  ................
-00004a40: 01cd 01d6 01db 0000 0000 0000 0201 0000  ................
-00004a50: 0000 0000 004c 0000 0000 0000 0000 0000  .....L..........
-00004a60: 0000 0000 01dc 0000 000d 006f 0075 0074  ...........o.u.t
-00004a70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00004a80: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
-00004a90: b7c8 5a86 d0fe c441 0000 000d 006f 0075  ..Z....A.....o.u
-00004aa0: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
-00004ab0: 006f 006c 0073 6d6f 6444 626c 6f62 0000  .o.l.smodDblob..
-00004ac0: 0008 b7c8 5a86 d0fe c441 0000 000d 006f  ....Z....A.....o
-00004ad0: 0075 0074 006c 0069 0065 0072 005f 0074  .u.t.l.i.e.r._.t
-00004ae0: 006f 006f 006c 0073 7068 3153 636f 6d70  .o.o.l.sph1Scomp
-00004af0: 0000 0000 0002 1000 0000 000d 006f 0075  .............o.u
-00004b00: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
-00004b10: 006f 006c 0073 7653 726e 6c6f 6e67 0000  .o.l.svSrnlong..
-00004b20: 0001 0000 0008 0070 006c 006f 0074 0074  .......p.l.o.t.t
-00004b30: 0069 006e 0067 6277 7370 626c 6f62 0000  .i.n.gbwspblob..
-00004b40: 00c8 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00004b50: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00004b60: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00004b70: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00004b80: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00004b90: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00004ba0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00004bb0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-00004bc0: 5f10 177b 7b32 302c 2039 307d 2c20 7b31  _..{{20, 90}, {1
-00004bd0: 3031 352c 2037 3637 7d7d 0908 1725 313d  015, 767}}...%1=
-00004be0: 4960 6d79 7a7b 7c7d 7e98 0000 0000 0000  I`myz{|}~.......
-00004bf0: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00004c00: 0000 0000 0000 0000 0099 0000 0008 0070  ...............p
-00004c10: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00004c20: 3153 636f 6d70 0000 0000 0009 13d5 0000  1Scomp..........
-00004c30: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
-00004c40: 0067 6c73 7643 626c 6f62 0000 02b0 6270  .glsvCblob....bp
-00004c50: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-00004c60: 0a0b 0c0d 1a48 4948 4a0c 4c58 6963 6f6e  .....HIHJ.LXicon
-00004c70: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-00004c80: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-00004c90: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-00004ca0: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
-00004cb0: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
-00004cc0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
-00004cd0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-00004ce0: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
-00004cf0: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00004d00: 6f6e 2340 3000 0000 0000 0009 ab0e 171c  on#@0...........
-00004d10: 2125 2a2f 3439 3e43 d40f 1011 1213 140c  !%*/49>C........
-00004d20: 0c5a 6964 656e 7469 6669 6572 5577 6964  .ZidentifierUwid
-00004d30: 7468 5961 7363 656e 6469 6e67 5776 6973  thYascendingWvis
-00004d40: 6962 6c65 546e 616d 6511 0127 0909 d40f  ibleTname..'....
-00004d50: 1011 1218 191a 1a58 7562 6971 7569 7479  .......Xubiquity
-00004d60: 1023 0808 d40f 1011 121d 1e1a 0c5c 6461  .#...........\da
-00004d70: 7465 4d6f 6469 6669 6564 10b5 0809 d40f  teModified......
-00004d80: 1011 1222 1e1a 1a5b 6461 7465 4372 6561  ..."...[dateCrea
-00004d90: 7465 6408 08d4 0f10 1112 2627 1a0c 5473  ted.......&'..Ts
-00004da0: 697a 6510 6108 09d4 0f10 1112 2b2c 0c0c  ize.a.......+,..
-00004db0: 546b 696e 6410 7309 09d4 0f10 1112 3031  Tkind.s.......01
-00004dc0: 0c1a 556c 6162 656c 1064 0908 d40f 1011  ..Ulabel.d......
-00004dd0: 1235 360c 1a57 7665 7273 696f 6e10 4b09  .56..Wversion.K.
-00004de0: 08d4 0f10 1112 3a3b 0c1a 5863 6f6d 6d65  ......:;..Xcomme
-00004df0: 6e74 7311 012c 0908 d40f 1011 123f 401a  nts..,.......?@.
-00004e00: 1a5e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00004e10: 10c8 0808 d40f 1011 1244 1e1a 1a59 6461  .........D...Yda
-00004e20: 7465 4164 6465 6408 0808 2300 0000 0000  teAdded...#.....
-00004e30: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00004e40: 6509 1001 0008 001d 0026 0038 0040 0054  e........&.8.@.T
-00004e50: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
-00004e60: 00ca 00d3 00de 00e4 00ee 00f6 00fb 00fe  ................
-00004e70: 00ff 0100 0109 0112 0114 0115 0116 011f  ................
-00004e80: 012c 012e 012f 0130 0139 0145 0146 0147  .,.../.0.9.E.F.G
-00004e90: 0150 0155 0157 0158 0159 0162 0167 0169  .P.U.W.X.Y.b.g.i
-00004ea0: 016a 016b 0174 017a 017c 017d 017e 0187  .j.k.t.z.|.}.~..
-00004eb0: 018f 0191 0192 0193 019c 01a5 01a8 01a9  ................
-00004ec0: 01aa 01b3 01c2 01c4 01c5 01c6 01cf 01d9  ................
-00004ed0: 01da 01db 01dc 01e5 01ee 01f3 01f4 0000  ................
-00004ee0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-00004ef0: 0000 0000 0000 0000 0000 0000 01f6 7430  ..............t0
-00004f00: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00004f10: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00004f20: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00004f30: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00004f40: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+00004020: 0067 6c73 7670 626c 6f62 0000 025e 6270  .glsvpblob...^bp
+00004030: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
+00004040: 0a0b 1a46 470a 2758 6963 6f6e 5369 7a65  ...FG.'XiconSize
+00004050: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00004060: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00004070: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00004080: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+00004090: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+000040a0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+000040b0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+000040c0: 0000 0009 d90c 0d0e 0f10 1112 1314 151e  ................
+000040d0: 2328 2c31 363b 4058 636f 6d6d 656e 7473  #(,16;@Xcomments
+000040e0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+000040f0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00004100: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00004110: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00004120: 546e 616d 65d4 1617 1819 1a0a 1c1d 5776  Tname.........Wv
+00004130: 6973 6962 6c65 5961 7363 656e 6469 6e67  isibleYascending
+00004140: 5577 6964 7468 5569 6e64 6578 0809 1101  UwidthUindex....
+00004150: 2c10 07d4 1617 1819 1a1a 2122 0808 10c8  ,.........!"....
+00004160: 1008 d416 1718 190a 1a26 2709 0810 b510  .........&'.....
+00004170: 01d4 1617 1819 1a1a 262b 0808 1002 d416  ........&+......
+00004180: 1718 190a 1a2f 3009 0810 6110 03d4 1617  ...../0...a.....
+00004190: 1819 1a0a 3435 0809 1064 1005 d416 1718  ....45...d......
+000041a0: 190a 0a39 3a09 0910 7310 04d4 1617 1819  ...9:...s.......
+000041b0: 1a0a 3e3f 0809 104b 1006 d416 1718 190a  ..>?...K........
+000041c0: 0a43 4409 0911 0251 1000 0823 4028 0000  .CD....Q...#@(..
+000041d0: 0000 0000 546e 616d 6509 0008 0019 0022  ....Tname......"
+000041e0: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
+000041f0: 0096 00a9 00b2 00c1 00ce 00da 00df 00e5  ................
+00004200: 00ea 00f2 00f7 0100 0108 0112 0118 011e  ................
+00004210: 011f 0120 0123 0125 012e 012f 0130 0132  ... .#.%.../.0.2
+00004220: 0134 013d 013e 013f 0141 0143 014c 014d  .4.=.>.?.A.C.L.M
+00004230: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
+00004240: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
+00004250: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
+00004260: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
+00004270: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
+00004280: 0000 0000 0000 0000 0000 01ac 0000 0009  ................
+00004290: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
+000042a0: 0067 6d6f 4444 626c 6f62 0000 0008 7246  .gmoDDblob....rF
+000042b0: 2c98 4a00 c541 0000 0009 006c 0061 0062  ,.J..A.....l.a.b
+000042c0: 0065 006c 006c 0069 006e 0067 6d6f 6444  .e.l.l.i.n.gmodD
+000042d0: 626c 6f62 0000 0008 cb5b 96d0 97fe c441  blob.....[.....A
+000042e0: 0000 0009 006c 0061 0062 0065 006c 006c  .....l.a.b.e.l.l
+000042f0: 0069 006e 0067 7068 3153 636f 6d70 0000  .i.n.gph1Scomp..
+00004300: 0000 0001 c000 0000 0009 006c 0061 0062  ...........l.a.b
+00004310: 0065 006c 006c 0069 006e 0067 7653 726e  .e.l.l.i.n.gvSrn
+00004320: 6c6f 6e67 0000 0001 0000 0006 006d 0069  long.........m.i
+00004330: 0078 0069 006e 0073 6277 7370 626c 6f62  .x.i.n.sbwspblob
+00004340: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00004350: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00004360: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00004370: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00004380: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00004390: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+000043a0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+000043b0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+000043c0: 0809 5f10 187b 7b33 3934 2c20 3138 317d  .._..{{394, 181}
+000043d0: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
+000043e0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+000043f0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00004400: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
+00004410: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
+00004420: 5363 6f6d 7000 0000 0000 0965 c500 0000  Scomp......e....
+00004430: 0600 6d00 6900 7800 6900 6e00 736d 6f44  ..m.i.x.i.n.smoD
+00004440: 4462 6c6f 6200 0000 0892 2cee 1963 01c5  Dblob.....,..c..
+00004450: 4100 0000 0600 6d00 6900 7800 6900 6e00  A.....m.i.x.i.n.
+00004460: 736d 6f64 4462 6c6f 6200 0000 0892 2cee  smodDblob.....,.
+00004470: 1963 01c5 4100 0000 0600 6d00 6900 7800  .c..A.....m.i.x.
+00004480: 6900 6e00 7370 6831 5363 6f6d 7000 0000  i.n.sph1Scomp...
+00004490: 0000 0a40 0000 0000 0600 6d00 6900 7800  ...@......m.i.x.
+000044a0: 6900 6e00 7376 5372 6e6c 6f6e 6700 0000  i.n.svSrnlong...
+000044b0: 0100 0000 0500 6d00 6f00 6400 6500 6c62  ......m.o.d.e.lb
+000044c0: 7773 7062 6c6f 6200 0000 c662 706c 6973  wspblob....bplis
+000044d0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+000044e0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+000044f0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+00004500: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00004510: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+00004520: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+00004530: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00004540: 6562 6172 0808 0908 095f 1015 7b7b 302c  ebar....._..{{0,
+00004550: 2030 7d2c 207b 3134 3430 2c20 3837 377d   0}, {1440, 877}
+00004560: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+00004570: 9600 0000 0000 0001 0100 0000 0000 0000  ................
+00004580: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+00004590: 9700 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
+000045a0: 6731 5363 6f6d 7000 0000 0000 0114 7400  g1Scomp.......t.
+000045b0: 0000 0500 6d00 6f00 6400 6500 6c6c 7376  ....m.o.d.e.llsv
+000045c0: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
+000045d0: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
+000045e0: 4b0a 5f10 1276 6965 774f 7074 696f 6e73  K._..viewOptions
+000045f0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00004600: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00004610: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00004620: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+00004630: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+00004640: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+00004650: 4461 7465 7310 0109 ab0c 151d 2226 2b30  Dates......."&+0
+00004660: 353a 3f44 d40d 0e0f 100a 0a13 1457 7669  5:?D.........Wvi
+00004670: 7369 626c 6559 6173 6365 6e64 696e 6755  sibleYascendingU
+00004680: 7769 6474 685a 6964 656e 7469 6669 6572  widthZidentifier
+00004690: 0909 1102 5154 6e61 6d65 d416 1718 1019  ....QTname......
+000046a0: 1a19 1c57 7669 7369 626c 6555 7769 6474  ...WvisibleUwidt
+000046b0: 6859 6173 6365 6e64 696e 6708 1023 0858  hYascending..#.X
+000046c0: 7562 6971 7569 7479 d40d 0e0f 100a 1920  ubiquity....... 
+000046d0: 2109 0810 b55c 6461 7465 4d6f 6469 6669  !....\dateModifi
+000046e0: 6564 d40d 0e0f 1019 1920 2508 085b 6461  ed....... %..[da
+000046f0: 7465 4372 6561 7465 64d4 0d0e 0f10 0a19  teCreated.......
+00004700: 292a 0908 1061 5473 697a 65d4 0d0e 0f10  )*...aTsize.....
+00004710: 0a0a 2e2f 0909 1073 546b 696e 64d4 0d0e  .../...sTkind...
+00004720: 0f10 190a 3334 0809 1064 556c 6162 656c  ....34...dUlabel
+00004730: d40d 0e0f 1019 0a38 3908 0910 4b57 7665  .......89...KWve
+00004740: 7273 696f 6ed4 0d0e 0f10 190a 3d3e 0809  rsion.......=>..
+00004750: 1101 2c58 636f 6d6d 656e 7473 d40d 0e0f  ..,Xcomments....
+00004760: 1019 1942 4308 0810 c85e 6461 7465 4c61  ...BC....^dateLa
+00004770: 7374 4f70 656e 6564 d416 1718 1019 2019  stOpened...... .
+00004780: 4708 0859 6461 7465 4164 6465 6408 2340  G..YdateAdded.#@
+00004790: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
+000047a0: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+000047b0: 005c 0065 0070 0079 008c 008e 008f 009b  .\.e.p.y........
+000047c0: 00a4 00ac 00b6 00bc 00c7 00c8 00c9 00cc  ................
+000047d0: 00d1 00da 00e2 00e8 00f2 00f3 00f5 00f6  ................
+000047e0: 00ff 0108 0109 010a 010c 0119 0122 0123  .............".#
+000047f0: 0124 0130 0139 013a 013b 013d 0142 014b  .$.0.9.:.;.=.B.K
+00004800: 014c 014d 014f 0154 015d 015e 015f 0161  .L.M.O.T.].^._.a
+00004810: 0167 0170 0171 0172 0174 017c 0185 0186  .g.p.q.r.t.|....
+00004820: 0187 018a 0193 019c 019d 019e 01a0 01af  ................
+00004830: 01b8 01b9 01ba 01c4 01c5 01ce 01d3 01dc  ................
+00004840: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
+00004850: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
+00004860: 0000 0005 006d 006f 0064 0065 006c 6c73  .....m.o.d.e.lls
+00004870: 7670 626c 6f62 0000 025e 6270 6c69 7374  vpblob...^bplist
+00004880: 3030 d801 0203 0405 0607 0809 0a0b 1d45  00.............E
+00004890: 4647 0a5f 1012 7669 6577 4f70 7469 6f6e  FG._..viewOption
+000048a0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+000048b0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+000048c0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+000048d0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+000048e0: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
+000048f0: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
+00004900: 6544 6174 6573 1001 09d9 0c0d 0e0f 1011  eDates..........
+00004910: 1213 1415 1e23 282d 3237 3c41 5863 6f6d  .....#(-27<AXcom
+00004920: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
+00004930: 656e 6564 5b64 6174 6543 7265 6174 6564  ened[dateCreated
+00004940: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
+00004950: 5776 6572 7369 6f6e 546e 616d 655c 6461  WversionTname\da
+00004960: 7465 4d6f 6469 6669 6564 d416 1718 191a  teModified......
+00004970: 0a1c 1d55 696e 6465 7859 6173 6365 6e64  ...UindexYascend
+00004980: 696e 6755 7769 6474 6857 7669 7369 626c  ingUwidthWvisibl
+00004990: 6510 0709 1101 2c08 d416 1718 191f 1d21  e.....,........!
+000049a0: 1d10 0808 10c8 08d4 1617 1819 241d 261d  ............$.&.
+000049b0: 1002 0810 b508 d416 1718 1929 1d2b 0a10  ...........).+..
+000049c0: 0308 1061 09d4 1617 1819 2e0a 301d 1005  ...a........0...
+000049d0: 0910 6408 d416 1718 1933 0a35 0a10 0409  ..d......3.5....
+000049e0: 1073 09d4 1617 1819 380a 3a1d 1006 0910  .s......8.:.....
+000049f0: 4b08 d416 1718 193d 0a3f 0a10 0009 1102  K......=.?......
+00004a00: 5109 d416 1718 1909 1d26 0a08 0908 2340  Q........&....#@
+00004a10: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
+00004a20: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00004a30: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
+00004a40: 00ab 00ba 00c6 00cb 00d1 00d6 00de 00e3  ................
+00004a50: 00f0 00f9 00ff 0109 010f 0117 0119 011a  ................
+00004a60: 011d 011e 0127 0129 012a 012c 012d 0136  .....'.).*.,.-.6
+00004a70: 0138 0139 013b 013c 0145 0147 0148 014a  .8.9.;.<.E.G.H.J
+00004a80: 014b 0154 0156 0157 0159 015a 0163 0165  .K.T.V.W.Y.Z.c.e
+00004a90: 0166 0168 0169 0172 0174 0175 0177 0178  .f.h.i.r.t.u.w.x
+00004aa0: 0181 0183 0184 0187 0188 0191 0192 0193  ................
+00004ab0: 0194 019d 01a2 01ab 0000 0000 0000 0201  ................
+00004ac0: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00004ad0: 0000 0000 0000 01ac 0000 0005 006d 006f  .............m.o
+00004ae0: 0064 0065 006c 6d6f 4444 626c 6f62 0000  .d.e.lmoDDblob..
+00004af0: 0008 e652 eadf 2c00 c541 0000 0005 006d  ...R..,..A.....m
+00004b00: 006f 0064 0065 006c 6d6f 6444 626c 6f62  .o.d.e.lmodDblob
+00004b10: 0000 0008 e8d9 3f86 d0fe c441 0000 0005  ......?....A....
+00004b20: 006d 006f 0064 0065 006c 7068 3153 636f  .m.o.d.e.lph1Sco
+00004b30: 6d70 0000 0000 0001 4000 0000 0005 006d  mp......@......m
+00004b40: 006f 0064 0065 006c 7653 726e 6c6f 6e67  .o.d.e.lvSrnlong
+00004b50: 0000 0001 0000 000d 006f 0075 0074 006c  .........o.u.t.l
+00004b60: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00004b70: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+00004b80: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00004b90: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00004ba0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00004bb0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00004bc0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00004bd0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00004be0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00004bf0: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+00004c00: 7b33 3934 2c20 3138 317d 2c20 7b37 3730  {394, 181}, {770
+00004c10: 2c20 3433 367d 7d09 0817 2531 3d49 606d  , 436}}...%1=I`m
+00004c20: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+00004c30: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00004c40: 0000 0000 0000 9a00 0000 0d00 6f00 7500  ............o.u.
+00004c50: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
+00004c60: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
+00004c70: 0000 012d 2d00 0000 0d00 6f00 7500 7400  ...--.....o.u.t.
+00004c80: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00004c90: 6c00 736c 7376 4362 6c6f 6200 0002 af62  l.slsvCblob....b
+00004ca0: 706c 6973 7430 30da 0102 0304 0506 0708  plist00.........
+00004cb0: 090a 0b0c 0d1a 4849 484a 0c4c 5869 636f  ......HIHJ.LXico
+00004cc0: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
+00004cd0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00004ce0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00004cf0: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
+00004d00: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
+00004d10: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
+00004d20: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+00004d30: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+00004d40: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00004d50: 696f 6e23 4030 0000 0000 0000 09ab 0e17  ion#@0..........
+00004d60: 1c21 252a 2f34 393e 43d4 0f10 1112 0c14  .!%*/49>C.......
+00004d70: 0c16 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+00004d80: 5961 7363 656e 6469 6e67 5a69 6465 6e74  YascendingZident
+00004d90: 6966 6965 7209 10f0 0954 6e61 6d65 d412  ifier....Tname..
+00004da0: 1011 0f18 191a 1a58 7562 6971 7569 7479  .......Xubiquity
+00004db0: 1023 0808 d412 1011 0f1d 1e1a 0c5c 6461  .#...........\da
+00004dc0: 7465 4d6f 6469 6669 6564 10b5 0809 d412  teModified......
+00004dd0: 1011 0f22 1e1a 1a5b 6461 7465 4372 6561  ..."...[dateCrea
+00004de0: 7465 6408 08d4 1210 110f 2627 1a0c 5473  ted.......&'..Ts
+00004df0: 697a 6510 6108 09d4 1210 110f 2b2c 0c0c  ize.a.......+,..
+00004e00: 546b 696e 6410 7309 09d4 1210 110f 3031  Tkind.s.......01
+00004e10: 0c1a 556c 6162 656c 1064 0908 d412 1011  ..Ulabel.d......
+00004e20: 0f35 360c 1a57 7665 7273 696f 6e10 4b09  .56..Wversion.K.
+00004e30: 08d4 1210 110f 3a3b 0c1a 5863 6f6d 6d65  ......:;..Xcomme
+00004e40: 6e74 7311 012c 0908 d412 1011 0f3f 401a  nts..,.......?@.
+00004e50: 1a5e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
+00004e60: 10c8 0808 d412 1011 0f44 1e1a 1a59 6461  .........D...Yda
+00004e70: 7465 4164 6465 6408 0808 2300 0000 0000  teAdded...#.....
+00004e80: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00004e90: 6509 1001 0008 001d 0026 0038 0040 0054  e........&.8.@.T
+00004ea0: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
+00004eb0: 00ca 00d3 00db 00e1 00eb 00f6 00f7 00f9  ................
+00004ec0: 00fa 00ff 0108 0111 0113 0114 0115 011e  ................
+00004ed0: 012b 012d 012e 012f 0138 0144 0145 0146  .+.-.../.8.D.E.F
+00004ee0: 014f 0154 0156 0157 0158 0161 0166 0168  .O.T.V.W.X.a.f.h
+00004ef0: 0169 016a 0173 0179 017b 017c 017d 0186  .i.j.s.y.{.|.}..
+00004f00: 018e 0190 0191 0192 019b 01a4 01a7 01a8  ................
+00004f10: 01a9 01b2 01c1 01c3 01c4 01c5 01ce 01d8  ................
+00004f20: 01d9 01da 01db 01e4 01ed 01f2 01f3 0000  ................
+00004f30: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
+00004f40: 0000 0000 0000 0000 0000 0000 01f5 5368  ..............Sh
 00004f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
 00004f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00004f70: 6172 0808 0908 095f 1018 7b7b 3635 372c  ar....._..{{657,
-00004f80: 2032 3730 7d2c 207b 3938 392c 2034 3336   270}, {989, 436
-00004f90: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00004fa0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-00004fb0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00004fc0: 009a 0000 0000 0000 0000 0000 0000 0000  ................
-00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f70: 6172 0808 0908 095f 1015 7b7b 302c 2030  ar....._..{{0, 0
+00004f80: 7d2c 207b 3134 3430 2c20 3837 377d 7d09  }, {1440, 877}}.
+00004f90: 0817 2531 3d49 606d 797a 7b7c 7d7e 9600  ..%1=I`myz{|}~..
+00004fa0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00004fb0: 0000 0000 0000 0000 0000 0000 0000 9700  ................
+00004fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00004fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00004fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005000: 0000 0000 0000 0000 0000 0014 0000 0008  ................
-00005010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00005020: 6d6f 4444 626c 6f62 0000 0008 38ff 7851  moDDblob....8.xQ
-00005030: 63ff c441 0000 0008 0070 006c 006f 0074  c..A.....p.l.o.t
-00005040: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
-00005050: 0000 0008 38ff 7851 63ff c441 0000 0008  ....8.xQc..A....
-00005060: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00005070: 7068 3153 636f 6d70 0000 0000 000b 2000  ph1Scomp...... .
-00005080: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00005090: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
-000050a0: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-000050b0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-000050c0: 0074 0069 006f 006e 0073 6277 7370 626c  .t.i.o.n.sbwspbl
-000050d0: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-000050e0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-000050f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00005100: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00005110: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00005120: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00005130: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00005140: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00005150: 0809 0809 5f10 197b 7b31 3539 2c20 3132  ...._..{{159, 12
-00005160: 337d 2c20 7b31 3037 362c 2036 3231 7d7d  3}, {1076, 621}}
-00005170: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00005180: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00005190: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-000051a0: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-000051b0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-000051c0: 0074 0069 006f 006e 0073 6473 636c 626f  .t.i.o.n.sdsclbo
-000051d0: 6f6c 0000 0000 1300 7000 6f00 7300 6500  ol......p.o.s.e.
-000051e0: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
-000051f0: 7200 6100 7400 6900 6f00 6e00 736c 6731  r.a.t.i.o.n.slg1
-00005200: 5363 6f6d 7000 0000 0000 06ae 5600 0000  Scomp.......V...
-00005210: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-00005220: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00005230: 6900 6f00 6e00 736c 7376 4362 6c6f 6200  i.o.n.slsvCblob.
-00005240: 0002 b062 706c 6973 7430 30da 0102 0304  ...bplist00.....
-00005250: 0506 0708 090a 0b0b 0d1a 4849 484a 4b4c  ..........HIHJKL
-00005260: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00005270: 7465 735f 100f 7368 6f77 4963 6f6e 5072  tes_..showIconPr
-00005280: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00005290: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-000052a0: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-000052b0: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-000052c0: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-000052d0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-000052e0: 7a65 5f10 1276 6965 774f 7074 696f 6e73  ze_..viewOptions
-000052f0: 5665 7273 696f 6e09 09ab 0e17 1c21 252a  Version......!%*
-00005300: 2f34 393e 43d4 0f10 1112 1314 0b0b 5a69  /49>C.........Zi
-00005310: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
-00005320: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00005330: 6554 6e61 6d65 1101 2709 09d4 0f10 1112  eTname..'.......
-00005340: 1819 1a1a 5875 6269 7175 6974 7910 2308  ....Xubiquity.#.
-00005350: 08d4 0f10 1112 1d1e 1a0b 5c64 6174 654d  ..........\dateM
-00005360: 6f64 6966 6965 6410 b508 09d4 0f10 1112  odified.........
-00005370: 221e 1a1a 5b64 6174 6543 7265 6174 6564  "...[dateCreated
-00005380: 0808 d40f 1011 1226 271a 0b54 7369 7a65  .......&'..Tsize
-00005390: 1061 0809 d40f 1011 122b 2c0b 0b54 6b69  .a.......+,..Tki
-000053a0: 6e64 1073 0909 d40f 1011 1230 310b 1a55  nd.s.......01..U
-000053b0: 6c61 6265 6c10 6409 08d4 0f10 1112 3536  label.d.......56
-000053c0: 0b1a 5776 6572 7369 6f6e 104b 0908 d40f  ..Wversion.K....
-000053d0: 1011 123a 3b0b 1a58 636f 6d6d 656e 7473  ...:;..Xcomments
-000053e0: 1101 2c09 08d4 0f10 1112 3f40 1a1a 5e64  ..,.......?@..^d
-000053f0: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
-00005400: 08d4 0f10 1112 441e 1a1a 5964 6174 6541  ......D...YdateA
-00005410: 6464 6564 0808 0823 0000 0000 0000 0000  dded...#........
-00005420: 2340 2800 0000 0000 0054 6e61 6d65 2340  #@(......Tname#@
-00005430: 3000 0000 0000 0010 0100 0800 1d00 3000  0.............0.
-00005440: 4200 4a00 5e00 7000 7900 8b00 9600 9f00  B.J.^.p.y.......
-00005450: b400 b500 b600 c200 cb00 d600 dc00 e600  ................
-00005460: ee00 f300 f600 f700 f801 0101 0a01 0c01  ................
-00005470: 0d01 0e01 1701 2401 2601 2701 2801 3101  ......$.&.'.(.1.
-00005480: 3d01 3e01 3f01 4801 4d01 4f01 5001 5101  =.>.?.H.M.O.P.Q.
-00005490: 5a01 5f01 6101 6201 6301 6c01 7201 7401  Z._.a.b.c.l.r.t.
-000054a0: 7501 7601 7f01 8701 8901 8a01 8b01 9401  u.v.............
-000054b0: 9d01 a001 a101 a201 ab01 ba01 bc01 bd01  ................
-000054c0: be01 c701 d101 d201 d301 d401 dd01 e601  ................
-000054d0: eb01 f400 0000 0000 0002 0100 0000 0000  ................
-000054e0: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-000054f0: 0001 f600 0000 1300 7000 6f00 7300 6500  ........p.o.s.e.
-00005500: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
-00005510: 7200 6100 7400 6900 6f00 6e00 736c 7376  r.a.t.i.o.n.slsv
-00005520: 7062 6c6f 6200 0002 9562 706c 6973 7430  pblob....bplist0
-00005530: 30da 0102 0304 0506 0708 090a 0b0b 0d1c  0...............
-00005540: 4849 484a 4b29 5f10 1075 7365 5265 6c61  HIHJK)_..useRela
-00005550: 7469 7665 4461 7465 735f 100f 7368 6f77  tiveDates_..show
-00005560: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00005570: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00005580: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00005590: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-000055a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-000055b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e58  ionXZsortColumnX
-000055c0: 6963 6f6e 5369 7a65 5f10 1276 6965 774f  iconSize_..viewO
-000055d0: 7074 696f 6e73 5665 7273 696f 6e09 09d9  ptionsVersion...
-000055e0: 0e0f 1011 1213 1415 1617 2025 2a2e 3338  .......... %*.38
-000055f0: 3d42 5863 6f6d 6d65 6e74 735e 6461 7465  =BXcomments^date
-00005600: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
-00005610: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
-00005620: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
-00005630: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
-00005640: d418 191a 1b1c 1d0b 1f57 7669 7369 626c  .........Wvisibl
-00005650: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-00005660: 6755 696e 6465 7808 1101 2c09 1007 d418  gUindex...,.....
-00005670: 191a 1b1c 221c 2408 10c8 0810 08d4 1819  ....".$.........
-00005680: 1a1b 0b27 1c29 0910 b508 1001 d418 191a  ...'.)..........
-00005690: 1b1c 271c 2d08 0810 02d4 1819 1a1b 0b30  ..'.-..........0
-000056a0: 1c32 0910 6108 1003 d418 191a 1b1c 350b  .2..a.........5.
-000056b0: 3708 1064 0910 05d4 1819 1a1b 0b3a 0b3c  7..d.........:.<
-000056c0: 0910 7309 1004 d418 191a 1b1c 3f0b 4108  ..s.........?.A.
-000056d0: 104b 0910 06d4 1819 1a1b 0b44 0b46 0911  .K.........D.F..
-000056e0: 0127 0910 0008 2300 0000 0000 0000 0023  .'....#........#
-000056f0: 4028 0000 0000 0000 546e 616d 6523 4030  @(......Tname#@0
-00005700: 0000 0000 0000 0008 001d 0030 0042 004a  ...........0.B.J
-00005710: 005e 0070 0079 008b 0096 009f 00b4 00b5  .^.p.y..........
-00005720: 00b6 00c9 00d2 00e1 00ee 00fa 00ff 0105  ................
-00005730: 010a 0112 0117 0120 0128 012e 0138 013e  ....... .(...8.>
-00005740: 013f 0142 0143 0145 014e 014f 0151 0152  .?.B.C.E.N.O.Q.R
-00005750: 0154 015d 015e 0160 0161 0163 016c 016d  .T.].^.`.a.c.l.m
-00005760: 016e 0170 0179 017a 017c 017d 017f 0188  .n.p.y.z.|.}....
-00005770: 0189 018b 018c 018e 0197 0198 019a 019b  ................
-00005780: 019d 01a6 01a7 01a9 01aa 01ac 01b5 01b6  ................
-00005790: 01b9 01ba 01bc 01bd 01c6 01cf 01d4 0000  ................
-000057a0: 0000 0000 0201 0000 0000 0000 004c 0000  .............L..
-000057b0: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
-000057c0: 0013 0070 006f 0073 0065 005f 0063 006f  ...p.o.s.e._.c.o
-000057d0: 006e 0066 0069 0067 0075 0072 0061 0074  .n.f.i.g.u.r.a.t
-000057e0: 0069 006f 006e 0073 6d6f 4444 626c 6f62  .i.o.n.smoDDblob
-000057f0: 0000 0008 d97e 4b74 e2dd c441 0000 0013  .....~Kt...A....
-00005800: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
-00005810: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
-00005820: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
-00005830: 0008 d97e 4b74 e2dd c441 0000 0013 0070  ...~Kt...A.....p
-00005840: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
-00005850: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
-00005860: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00005870: 0007 3000 0000 0013 0070 006f 0073 0065  ..0......p.o.s.e
-00005880: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
-00005890: 0072 0061 0074 0069 006f 006e 0073 7653  .r.a.t.i.o.n.svS
-000058a0: 726e 6c6f 6e67 0000 0001 0000 001b 0070  rnlong.........p
-000058b0: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
-000058c0: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
-000058d0: 006e 0073 005f 0061 0072 0063 0068 0069  .n.s._.a.r.c.h.i
-000058e0: 0076 0065 6c67 3153 636f 6d70 0000 0000  .v.elg1Scomp....
-000058f0: 0006 faed 0000 001b 0070 006f 0073 0065  .........p.o.s.e
-00005900: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
-00005910: 0072 0061 0074 0069 006f 006e 0073 005f  .r.a.t.i.o.n.s._
-00005920: 0061 0072 0063 0068 0069 0076 0065 6d6f  .a.r.c.h.i.v.emo
-00005930: 4444 626c 6f62 0000 0008 8983 1ea9 cbfe  DDblob..........
-00005940: c441 0000 001b 0070 006f 0073 0065 005f  .A.....p.o.s.e._
-00005950: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
-00005960: 0061 0074 0069 006f 006e 0073 005f 0061  .a.t.i.o.n.s._.a
-00005970: 0072 0063 0068 0069 0076 0065 6d6f 6444  .r.c.h.i.v.emodD
-00005980: 626c 6f62 0000 0008 8983 1ea9 cbfe c441  blob...........A
-00005990: 0000 001b 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-000059a0: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-000059b0: 0074 0069 006f 006e 0073 005f 0061 0072  .t.i.o.n.s._.a.r
-000059c0: 0063 0068 0069 0076 0065 7068 3153 636f  .c.h.i.v.eph1Sco
-000059d0: 6d70 0000 0000 0007 9000 0000 000e 0070  mp.............p
-000059e0: 006f 0073 0065 005f 0069 006d 0070 006f  .o.s.e._.i.m.p.o
-000059f0: 0072 0074 0065 0072 0073 6277 7370 626c  .r.t.e.r.sbwspbl
-00005a00: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-00005a10: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00005a20: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00005a30: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00005a40: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00005a50: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00005a60: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00005a70: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00005a80: 0809 0809 5f10 197b 7b36 3432 2c20 3132  ...._..{{642, 12
-00005a90: 397d 2c20 7b31 3031 352c 2037 3637 7d7d  9}, {1015, 767}}
-00005aa0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00005ab0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00005ac0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-00005ad0: 0000 000e 0070 006f 0073 0065 005f 0069  .....p.o.s.e._.i
-00005ae0: 006d 0070 006f 0072 0074 0065 0072 0073  .m.p.o.r.t.e.r.s
-00005af0: 6c67 3153 636f 6d70 0000 0000 0004 0557  lg1Scomp.......W
-00005b00: 0000 000e 0070 006f 0073 0065 005f 0069  .....p.o.s.e._.i
-00005b10: 006d 0070 006f 0072 0074 0065 0072 0073  .m.p.o.r.t.e.r.s
-00005b20: 6c73 7643 626c 6f62 0000 0278 6270 6c69  lsvCblob...xbpli
-00005b30: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00005b40: 1646 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
-00005b50: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-00005b60: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00005b70: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00005b80: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-00005b90: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
-00005ba0: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-00005bb0: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
-00005bc0: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
-00005bd0: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00005be0: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
-00005bf0: 6965 7209 10ea 0954 6e61 6d65 d40d 0e0f  ier....Tname....
-00005c00: 1016 1716 1908 1023 0858 7562 6971 7569  .......#.Xubiqui
-00005c10: 7479 d40d 0e0f 100a 1c16 1e09 10b5 085c  ty.............\
-00005c20: 6461 7465 4d6f 6469 6669 6564 d40d 0e0f  dateModified....
-00005c30: 1016 1c16 2208 085b 6461 7465 4372 6561  ...."..[dateCrea
-00005c40: 7465 64d4 0d0e 0f10 0a25 1627 0910 6108  ted......%.'..a.
-00005c50: 5473 697a 65d4 0d0e 0f10 0a2a 0a2c 0910  Tsize......*.,..
-00005c60: 7309 546b 696e 64d4 0d0e 0f10 162f 0a31  s.Tkind....../.1
-00005c70: 0810 6409 556c 6162 656c d40d 0e0f 1016  ..d.Ulabel......
-00005c80: 340a 3608 104b 0957 7665 7273 696f 6ed4  4.6..K.Wversion.
-00005c90: 0d0e 0f10 1639 0a3b 0811 012c 0958 636f  .....9.;...,.Xco
-00005ca0: 6d6d 656e 7473 d40d 0e0f 1016 3e16 4008  mments......>.@.
-00005cb0: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
-00005cc0: 6564 d40d 0e0f 1016 1c16 4408 0859 6461  ed........D..Yda
-00005cd0: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-00005ce0: 0054 6e61 6d65 2340 3000 0000 0000 0009  .Tname#@0.......
-00005cf0: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
-00005d00: 0079 008c 008e 008f 009b 00a4 00ac 00b2  .y..............
-00005d10: 00bc 00c7 00c8 00ca 00cb 00d0 00d9 00da  ................
-00005d20: 00dc 00dd 00e6 00ef 00f0 00f2 00f3 0100  ................
-00005d30: 0109 010a 010b 0117 0120 0121 0123 0124  ......... .!.#.$
-00005d40: 0129 0132 0133 0135 0136 013b 0144 0145  .).2.3.5.6.;.D.E
-00005d50: 0147 0148 014e 0157 0158 015a 015b 0163  .G.H.N.W.X.Z.[.c
-00005d60: 016c 016d 0170 0171 017a 0183 0184 0186  .l.m.p.q.z......
-00005d70: 0187 0196 019f 01a0 01a1 01ab 01ac 01b5  ................
-00005d80: 01ba 01c3 0000 0000 0000 0201 0000 0000  ................
-00005d90: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-00005da0: 0000 01c4 6108 09d4 0f10 1112 2b2c 0c0c  ....a.......+,..
-00005db0: 546b 696e 6410 7309 09d4 0f10 1112 3031  Tkind.s.......01
-00005dc0: 0c1a 556c 6162 656c 1064 0908 d40f 1011  ..Ulabel.d......
-00005dd0: 1235 360c 1a57 7665 7273 696f 6e10 4b09  .56..Wversion.K.
-00005de0: 08d4 0f10 1112 3a3b 0c1a 5863 6f6d 6d65  ......:;..Xcomme
-00005df0: 6e74 7311 012c 0908 d40f 1011 123f 401a  nts..,.......?@.
-00005e00: 1a5e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00005e10: 10c8 0808 d40f 1011 1244 1e1a 1a59 6461  .........D...Yda
-00005e20: 7465 4164 6465 6408 0808 2300 0000 0000  teAdded...#.....
-00005e30: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00005e40: 6509 1001 0008 001d 0026 0038 0040 0054  e........&.8.@.T
-00005e50: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
-00005e60: 00ca 00d3 00de 00e4 00ee 00f6 00fb 00fe  ................
-00005e70: 00ff 0100 0109 0112 0114 0115 0116 011f  ................
-00005e80: 012c 012e 012f 0130 0139 0145 0146 0147  .,.../.0.9.E.F.G
-00005e90: 0150 0155 0157 0158 0159 0162 0167 0169  .P.U.W.X.Y.b.g.i
-00005ea0: 016a 016b 0174 017a 017c 017d 017e 0187  .j.k.t.z.|.}.~..
-00005eb0: 018f 0191 0192 0193 019c 01a5 01a8 01a9  ................
-00005ec0: 01aa 01b3 01c2 01c4 01c5 01c6 01cf 01d9  ................
-00005ed0: 01da 01db 01dc 01e5 01ee 01f3 01f4 0000  ................
-00005ee0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-00005ef0: 0000 0000 0000 0000 0000 0000 01f6 7430  ..............t0
-00005f00: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00005f10: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00005f20: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00005f30: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00005f40: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00005f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00005f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00005f70: 6172 0808 0908 095f 1018 7b7b 3635 372c  ar....._..{{657,
-00005f80: 2032 3730 7d2c 207b 3938 392c 2034 3336   270}, {989, 436
-00005f90: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00005fa0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-00005fb0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00005fc0: 009a 0000 0000 0000 0000 0000 0000 0000  ................
-00005fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005000: 0000 0000 0000 0000 0000 0014 0000 000d  ................
+00005010: 006f 0075 0074 006c 0069 0065 0072 005f  .o.u.t.l.i.e.r._
+00005020: 0074 006f 006f 006c 0073 6d6f 4444 626c  .t.o.o.l.smoDDbl
+00005030: 6f62 0000 0008 b7c8 5a86 d0fe c441 0000  ob......Z....A..
+00005040: 000d 006f 0075 0074 006c 0069 0065 0072  ...o.u.t.l.i.e.r
+00005050: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
+00005060: 626c 6f62 0000 0008 b7c8 5a86 d0fe c441  blob......Z....A
+00005070: 0000 000d 006f 0075 0074 006c 0069 0065  .....o.u.t.l.i.e
+00005080: 0072 005f 0074 006f 006f 006c 0073 7068  .r._.t.o.o.l.sph
+00005090: 3153 636f 6d70 0000 0000 0002 1000 0000  1Scomp..........
+000050a0: 000d 006f 0075 0074 006c 0069 0065 0072  ...o.u.t.l.i.e.r
+000050b0: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
+000050c0: 6c6f 6e67 0000 0001 0000 0008 0070 006c  long.........p.l
+000050d0: 006f 0074 0074 0069 006e 0067 6277 7370  .o.t.t.i.n.gbwsp
+000050e0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
+000050f0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
+00005100: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+00005110: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
+00005120: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00005130: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00005140: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00005150: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00005160: 7208 0809 0809 5f10 177b 7b32 302c 2039  r....._..{{20, 9
+00005170: 307d 2c20 7b31 3031 352c 2037 3637 7d7d  0}, {1015, 767}}
+00005180: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
+00005190: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+000051a0: 0000 0000 0000 0000 0000 0000 0000 0099  ................
+000051b0: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
+000051c0: 006e 0067 6c67 3153 636f 6d70 0000 0000  .n.glg1Scomp....
+000051d0: 0009 1177 0000 0008 0070 006c 006f 0074  ...w.....p.l.o.t
+000051e0: 0074 0069 006e 0067 6c73 7643 626c 6f62  .t.i.n.glsvCblob
+000051f0: 0000 02b0 6270 6c69 7374 3030 da01 0203  ....bplist00....
+00005200: 0405 0607 0809 0a0b 0c0d 1a48 4948 4a0c  ...........HIHJ.
+00005210: 4c58 6963 6f6e 5369 7a65 5f10 0f73 686f  LXiconSize_..sho
+00005220: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00005230: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00005240: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+00005250: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+00005260: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+00005270: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00005280: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00005290: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+000052a0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+000052b0: 0009 ab0e 171c 2125 2a2f 3439 3e43 d40f  ......!%*/49>C..
+000052c0: 1011 1213 140c 0c5a 6964 656e 7469 6669  .......Zidentifi
+000052d0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+000052e0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+000052f0: 0127 0909 d40f 1011 1218 191a 1a58 7562  .'...........Xub
+00005300: 6971 7569 7479 1023 0808 d40f 1011 121d  iquity.#........
+00005310: 1e1a 0c5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00005320: 10b5 0809 d40f 1011 1222 1e1a 1a5b 6461  ........."...[da
+00005330: 7465 4372 6561 7465 6408 08d4 0f10 1112  teCreated.......
+00005340: 2627 1a0c 5473 697a 6510 6108 09d4 0f10  &'..Tsize.a.....
+00005350: 1112 2b2c 0c0c 546b 696e 6410 7309 09d4  ..+,..Tkind.s...
+00005360: 0f10 1112 3031 0c1a 556c 6162 656c 1064  ....01..Ulabel.d
+00005370: 0908 d40f 1011 1235 360c 1a57 7665 7273  .......56..Wvers
+00005380: 696f 6e10 4b09 08d4 0f10 1112 3a3b 0c1a  ion.K.......:;..
+00005390: 5863 6f6d 6d65 6e74 7311 012c 0908 d40f  Xcomments..,....
+000053a0: 1011 123f 401a 1a5e 6461 7465 4c61 7374  ...?@..^dateLast
+000053b0: 4f70 656e 6564 10c8 0808 d40f 1011 1244  Opened.........D
+000053c0: 1e1a 1a59 6461 7465 4164 6465 6408 0808  ...YdateAdded...
+000053d0: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
+000053e0: 0000 546e 616d 6509 1001 0008 001d 0026  ..Tname........&
+000053f0: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
+00005400: 00b4 00bd 00be 00ca 00d3 00de 00e4 00ee  ................
+00005410: 00f6 00fb 00fe 00ff 0100 0109 0112 0114  ................
+00005420: 0115 0116 011f 012c 012e 012f 0130 0139  .......,.../.0.9
+00005430: 0145 0146 0147 0150 0155 0157 0158 0159  .E.F.G.P.U.W.X.Y
+00005440: 0162 0167 0169 016a 016b 0174 017a 017c  .b.g.i.j.k.t.z.|
+00005450: 017d 017e 0187 018f 0191 0192 0193 019c  .}.~............
+00005460: 01a5 01a8 01a9 01aa 01b3 01c2 01c4 01c5  ................
+00005470: 01c6 01cf 01d9 01da 01db 01dc 01e5 01ee  ................
+00005480: 01f3 01f4 0000 0000 0000 0201 0000 0000  ................
+00005490: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+000054a0: 0000 01f6 0000 0008 0070 006c 006f 0074  .........p.l.o.t
+000054b0: 0074 0069 006e 0067 6c73 7670 626c 6f62  .t.i.n.glsvpblob
+000054c0: 0000 0295 6270 6c69 7374 3030 da01 0203  ....bplist00....
+000054d0: 0405 0607 0809 0a0b 0c0d 1c48 4948 4a0c  ...........HIHJ.
+000054e0: 2958 6963 6f6e 5369 7a65 5f10 0f73 686f  )XiconSize_..sho
+000054f0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00005500: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00005510: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+00005520: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+00005530: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+00005540: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00005550: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00005560: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00005570: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+00005580: 0009 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+00005590: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
+000055a0: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+000055b0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+000055c0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+000055d0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+000055e0: 616d 65d4 1819 1a1b 1c1d 0c1f 5776 6973  ame.........Wvis
+000055f0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00005600: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+00005610: 07d4 1819 1a1b 1c22 1c24 0810 c808 1008  .......".$......
+00005620: d418 191a 1b0c 271c 2909 10b5 0810 01d4  ......'.).......
+00005630: 1819 1a1b 1c27 1c2d 0808 1002 d418 191a  .....'.-........
+00005640: 1b0c 301c 3209 1061 0810 03d4 1819 1a1b  ..0.2..a........
+00005650: 1c35 0c37 0810 6409 1005 d418 191a 1b0c  .5.7..d.........
+00005660: 3a0c 3c09 1073 0910 04d4 1819 1a1b 1c3f  :.<..s.........?
+00005670: 0c41 0810 4b09 1006 d418 191a 1b0c 440c  .A..K.........D.
+00005680: 4609 1101 2709 1000 0823 0000 0000 0000  F...'....#......
+00005690: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+000056a0: 0900 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
+000056b0: 6f00 8100 8c00 9f00 b400 bd00 be00 d100  o...............
+000056c0: da00 e900 f601 0201 0701 0d01 1201 1a01  ................
+000056d0: 1f01 2801 3001 3601 4001 4601 4701 4a01  ..(.0.6.@.F.G.J.
+000056e0: 4b01 4d01 5601 5701 5901 5a01 5c01 6501  K.M.V.W.Y.Z.\.e.
+000056f0: 6601 6801 6901 6b01 7401 7501 7601 7801  f.h.i.k.t.u.v.x.
+00005700: 8101 8201 8401 8501 8701 9001 9101 9301  ................
+00005710: 9401 9601 9f01 a001 a201 a301 a501 ae01  ................
+00005720: af01 b101 b201 b401 bd01 be01 c101 c201  ................
+00005730: c401 c501 ce01 d701 dc00 0000 0000 0002  ................
+00005740: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
+00005750: 0000 0000 0000 0001 dd00 0000 0800 7000  ..............p.
+00005760: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
+00005770: 4462 6c6f 6200 0000 0858 13c8 10f2 00c5  Dblob....X......
+00005780: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
+00005790: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
+000057a0: 0838 ff78 5163 ffc4 4100 0000 0800 7000  .8.xQc..A.....p.
+000057b0: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
+000057c0: 5363 6f6d 7000 0000 0000 0b20 0000 0000  Scomp...... ....
+000057d0: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
+000057e0: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
+000057f0: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
+00005800: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
+00005810: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
+00005820: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00005830: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
+00005840: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
+00005850: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
+00005860: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00005870: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00005880: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00005890: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
+000058a0: 095f 1019 7b7b 3135 392c 2031 3233 7d2c  ._..{{159, 123},
+000058b0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
+000058c0: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
+000058d0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+000058e0: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
+000058f0: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
+00005900: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
+00005910: 6900 6f00 6e00 7364 7363 6c62 6f6f 6c00  i.o.n.sdsclbool.
+00005920: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
+00005930: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
+00005940: 0074 0069 006f 006e 0073 6c67 3153 636f  .t.i.o.n.slg1Sco
+00005950: 6d70 0000 0000 0006 ae56 0000 0013 0070  mp.......V.....p
+00005960: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
+00005970: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
+00005980: 006e 0073 6c73 7643 626c 6f62 0000 02b0  .n.slsvCblob....
+00005990: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+000059a0: 0809 0a0b 0b0d 1a48 4948 4a4b 4c5f 1010  .......HIHJKL_..
+000059b0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000059c0: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+000059d0: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+000059e0: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
+000059f0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
+00005a00: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
+00005a10: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
+00005a20: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+00005a30: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00005a40: 7369 6f6e 0909 ab0e 171c 2125 2a2f 3439  sion......!%*/49
+00005a50: 3e43 d40f 1011 1213 140b 0b5a 6964 656e  >C.........Ziden
+00005a60: 7469 6669 6572 5577 6964 7468 5961 7363  tifierUwidthYasc
+00005a70: 656e 6469 6e67 5776 6973 6962 6c65 546e  endingWvisibleTn
+00005a80: 616d 6511 0127 0909 d40f 1011 1218 191a  ame..'..........
+00005a90: 1a58 7562 6971 7569 7479 1023 0808 d40f  .Xubiquity.#....
+00005aa0: 1011 121d 1e1a 0b5c 6461 7465 4d6f 6469  .......\dateModi
+00005ab0: 6669 6564 10b5 0809 d40f 1011 1222 1e1a  fied........."..
+00005ac0: 1a5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
+00005ad0: 0f10 1112 2627 1a0b 5473 697a 6510 6108  ....&'..Tsize.a.
+00005ae0: 09d4 0f10 1112 2b2c 0b0b 546b 696e 6410  ......+,..Tkind.
+00005af0: 7309 09d4 0f10 1112 3031 0b1a 556c 6162  s.......01..Ulab
+00005b00: 656c 1064 0908 d40f 1011 1235 360b 1a57  el.d.......56..W
+00005b10: 7665 7273 696f 6e10 4b09 08d4 0f10 1112  version.K.......
+00005b20: 3a3b 0b1a 5863 6f6d 6d65 6e74 7311 012c  :;..Xcomments..,
+00005b30: 0908 d40f 1011 123f 401a 1a5e 6461 7465  .......?@..^date
+00005b40: 4c61 7374 4f70 656e 6564 10c8 0808 d40f  LastOpened......
+00005b50: 1011 1244 1e1a 1a59 6461 7465 4164 6465  ...D...YdateAdde
+00005b60: 6408 0808 2300 0000 0000 0000 0023 4028  d...#........#@(
+00005b70: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+00005b80: 0000 0000 1001 0008 001d 0030 0042 004a  ...........0.B.J
+00005b90: 005e 0070 0079 008b 0096 009f 00b4 00b5  .^.p.y..........
+00005ba0: 00b6 00c2 00cb 00d6 00dc 00e6 00ee 00f3  ................
+00005bb0: 00f6 00f7 00f8 0101 010a 010c 010d 010e  ................
+00005bc0: 0117 0124 0126 0127 0128 0131 013d 013e  ...$.&.'.(.1.=.>
+00005bd0: 013f 0148 014d 014f 0150 0151 015a 015f  .?.H.M.O.P.Q.Z._
+00005be0: 0161 0162 0163 016c 0172 0174 0175 0176  .a.b.c.l.r.t.u.v
+00005bf0: 017f 0187 0189 018a 018b 0194 019d 01a0  ................
+00005c00: 01a1 01a2 01ab 01ba 01bc 01bd 01be 01c7  ................
+00005c10: 01d1 01d2 01d3 01d4 01dd 01e6 01eb 01f4  ................
+00005c20: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
+00005c30: 0000 0000 0000 0000 0000 0000 0000 01f6  ................
+00005c40: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
+00005c50: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
+00005c60: 0074 0069 006f 006e 0073 6c73 7670 626c  .t.i.o.n.slsvpbl
+00005c70: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
+00005c80: 0203 0405 0607 0809 0a0b 0b0d 1c48 4948  .............HIH
+00005c90: 4a4b 295f 1010 7573 6552 656c 6174 6976  JK)_..useRelativ
+00005ca0: 6544 6174 6573 5f10 0f73 686f 7749 636f  eDates_..showIco
+00005cb0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00005cc0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00005cd0: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+00005ce0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+00005cf0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+00005d00: 585a 736f 7274 436f 6c75 6d6e 5869 636f  XZsortColumnXico
+00005d10: 6e53 697a 655f 1012 7669 6577 4f70 7469  nSize_..viewOpti
+00005d20: 6f6e 7356 6572 7369 6f6e 0909 d90e 0f10  onsVersion......
+00005d30: 1112 1314 1516 1720 252a 2e33 383d 4258  ....... %*.38=BX
+00005d40: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
+00005d50: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
+00005d60: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
+00005d70: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
+00005d80: 5776 6572 7369 6f6e 546e 616d 65d4 1819  WversionTname...
+00005d90: 1a1b 1c1d 0b1f 5776 6973 6962 6c65 5577  ......WvisibleUw
+00005da0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
+00005db0: 6e64 6578 0811 012c 0910 07d4 1819 1a1b  ndex...,........
+00005dc0: 1c22 1c24 0810 c808 1008 d418 191a 1b0b  .".$............
+00005dd0: 271c 2909 10b5 0810 01d4 1819 1a1b 1c27  '.)............'
+00005de0: 1c2d 0808 1002 d418 191a 1b0b 301c 3209  .-..........0.2.
+00005df0: 1061 0810 03d4 1819 1a1b 1c35 0b37 0810  .a.........5.7..
+00005e00: 6409 1005 d418 191a 1b0b 3a0b 3c09 1073  d.........:.<..s
+00005e10: 0910 04d4 1819 1a1b 1c3f 0b41 0810 4b09  .........?.A..K.
+00005e20: 1006 d418 191a 1b0b 440b 4609 1101 2709  ........D.F...'.
+00005e30: 1000 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
+00005e40: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+00005e50: 0000 0000 0800 1d00 3000 4200 4a00 5e00  ........0.B.J.^.
+00005e60: 7000 7900 8b00 9600 9f00 b400 b500 b600  p.y.............
+00005e70: c900 d200 e100 ee00 fa00 ff01 0501 0a01  ................
+00005e80: 1201 1701 2001 2801 2e01 3801 3e01 3f01  .... .(...8.>.?.
+00005e90: 4201 4301 4501 4e01 4f01 5101 5201 5401  B.C.E.N.O.Q.R.T.
+00005ea0: 5d01 5e01 6001 6101 6301 6c01 6d01 6e01  ].^.`.a.c.l.m.n.
+00005eb0: 7001 7901 7a01 7c01 7d01 7f01 8801 8901  p.y.z.|.}.......
+00005ec0: 8b01 8c01 8e01 9701 9801 9a01 9b01 9d01  ................
+00005ed0: a601 a701 a901 aa01 ac01 b501 b601 b901  ................
+00005ee0: ba01 bc01 bd01 c601 cf01 d400 0000 0000  ................
+00005ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
+00005f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
+00005f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+00005f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+00005f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
+00005f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
+00005f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00005f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00005f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
+00005f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
+00005f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
+00005fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00005fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
+00005fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00005fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00005fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
 00005ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006000: 0000 0000 0000 0000 0000 0015 0000 000e  ................
-00006010: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
-00006020: 006f 0072 0074 0065 0072 0073 6d6f 4444  .o.r.t.e.r.smoDD
-00006030: 626c 6f62 0000 0008 9022 c3eb 97ff c441  blob.....".....A
-00006040: 0000 000e 0070 006f 0073 0065 005f 0069  .....p.o.s.e._.i
-00006050: 006d 0070 006f 0072 0074 0065 0072 0073  .m.p.o.r.t.e.r.s
-00006060: 6d6f 6444 626c 6f62 0000 0008 9022 c3eb  modDblob....."..
-00006070: 97ff c441 0000 000e 0070 006f 0073 0065  ...A.....p.o.s.e
-00006080: 005f 0069 006d 0070 006f 0072 0074 0065  ._.i.m.p.o.r.t.e
-00006090: 0072 0073 7068 3153 636f 6d70 0000 0000  .r.sph1Scomp....
-000060a0: 0004 b000 0000 000e 0070 006f 0073 0065  .........p.o.s.e
-000060b0: 005f 0069 006d 0070 006f 0072 0074 0065  ._.i.m.p.o.r.t.e
-000060c0: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
-000060d0: 0000 000f 0070 006f 0073 0065 005f 0070  .....p.o.s.e._.p
-000060e0: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-000060f0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
-00006100: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00006110: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00006120: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00006130: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00006140: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00006150: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00006160: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00006170: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00006180: 7b36 3537 2c20 3237 307d 2c20 7b39 3839  {657, 270}, {989
-00006190: 2c20 3433 367d 7d09 0817 2531 3d49 606d  , 436}}...%1=I`m
-000061a0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-000061b0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000061c0: 0000 0000 0000 9a00 0000 0f00 7000 6f00  ............p.o.
-000061d0: 7300 6500 5f00 7000 7200 6f00 6300 6500  s.e._.p.r.o.c.e.
-000061e0: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-000061f0: 7000 0000 0000 0084 be00 0000 0f00 7000  p.............p.
-00006200: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
-00006210: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
-00006220: 6c6f 6200 0000 089e 5585 d097 fec4 4100  lob.....U.....A.
-00006230: 0000 0f00 7000 6f00 7300 6500 5f00 7000  ....p.o.s.e._.p.
-00006240: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-00006250: 736d 6f64 4462 6c6f 6200 0000 089e 5585  smodDblob.....U.
-00006260: d097 fec4 4100 0000 0f00 7000 6f00 7300  ....A.....p.o.s.
-00006270: 6500 5f00 7000 7200 6f00 6300 6500 7300  e._.p.r.o.c.e.s.
-00006280: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
-00006290: 0000 0000 00d0 0000 0000 0f00 7000 6f00  ............p.o.
-000062a0: 7300 6500 5f00 7000 7200 6f00 6300 6500  s.e._.p.r.o.c.e.
-000062b0: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
-000062c0: 6700 0000 0100 0000 0900 7200 6f00 6900  g.........r.o.i.
-000062d0: 5f00 7400 6f00 6f00 6c00 7362 7773 7062  _.t.o.o.l.sbwspb
-000062e0: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
-000062f0: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00006300: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00006310: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00006320: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00006330: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00006340: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00006350: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00006360: 0808 0908 095f 1018 7b7b 3635 372c 2032  ....._..{{657, 2
-00006370: 3730 7d2c 207b 3938 392c 2034 3336 7d7d  70}, {989, 436}}
-00006380: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
-00006390: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-000063a0: 0000 0000 0000 0000 0000 0000 0000 009a  ................
-000063b0: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
-000063c0: 006f 006c 0073 6c67 3153 636f 6d70 0000  .o.l.slg1Scomp..
-000063d0: 0000 0004 251a 0000 0009 0072 006f 0069  ....%......r.o.i
-000063e0: 005f 0074 006f 006f 006c 0073 6c73 7643  ._.t.o.o.l.slsvC
-000063f0: 626c 6f62 0000 0278 6270 6c69 7374 3030  blob...xbplist00
-00006400: d801 0203 0405 0607 0809 0a0b 1846 470a  .............FG.
-00006410: 4958 6963 6f6e 5369 7a65 5f10 0f73 686f  IXiconSize_..sho
-00006420: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00006430: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00006440: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-00006450: 655a 736f 7274 436f 6c75 6d6e 5f10 1075  eZsortColumn_..u
-00006460: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
-00006470: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-00006480: 7369 6f6e 2340 3000 0000 0000 0009 ab0c  sion#@0.........
-00006490: 151a 1f23 282d 3237 3c41 d40d 0e0f 1011  ...#(-27<A......
-000064a0: 120a 0a5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
-000064b0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
-000064c0: 6973 6962 6c65 546e 616d 6510 d009 09d4  isibleTname.....
-000064d0: 0d0e 0f10 1617 1818 5875 6269 7175 6974  ........Xubiquit
-000064e0: 7910 2308 08d4 0d0e 0f10 1b1c 180a 5c64  y.#...........\d
-000064f0: 6174 654d 6f64 6966 6965 6410 b508 09d4  ateModified.....
-00006500: 0d0e 0f10 201c 1818 5b64 6174 6543 7265  .... ...[dateCre
-00006510: 6174 6564 0808 d40d 0e0f 1024 2518 0a54  ated.......$%..T
-00006520: 7369 7a65 1061 0809 d40d 0e0f 1029 2a0a  size.a.......)*.
-00006530: 0a54 6b69 6e64 1073 0909 d40d 0e0f 102e  .Tkind.s........
-00006540: 2f0a 1855 6c61 6265 6c10 6409 08d4 0d0e  /..Ulabel.d.....
-00006550: 0f10 3334 0a18 5776 6572 7369 6f6e 104b  ..34..Wversion.K
-00006560: 0908 d40d 0e0f 1038 390a 1858 636f 6d6d  .......89..Xcomm
-00006570: 656e 7473 1101 2c09 08d4 0d0e 0f10 3d3e  ents..,.......=>
-00006580: 1818 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00006590: 6410 c808 08d4 0d0e 0f10 421c 1818 5964  d.........B...Yd
-000065a0: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
-000065b0: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
-000065c0: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-000065d0: 0095 0096 00a2 00ab 00b6 00bc 00c6 00ce  ................
-000065e0: 00d3 00d5 00d6 00d7 00e0 00e9 00eb 00ec  ................
-000065f0: 00ed 00f6 0103 0105 0106 0107 0110 011c  ................
-00006600: 011d 011e 0127 012c 012e 012f 0130 0139  .....'.,.../.0.9
-00006610: 013e 0140 0141 0142 014b 0151 0153 0154  .>.@.A.B.K.Q.S.T
-00006620: 0155 015e 0166 0168 0169 016a 0173 017c  .U.^.f.h.i.j.s.|
-00006630: 017f 0180 0181 018a 0199 019b 019c 019d  ................
-00006640: 01a6 01b0 01b1 01b2 01b3 01bc 01c1 01c2  ................
-00006650: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
-00006660: 0000 0000 0000 0000 0000 0000 0000 01c4  ................
-00006670: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
-00006680: 006f 006c 0073 6c73 7670 626c 6f62 0000  .o.l.slsvpblob..
-00006690: 025d 6270 6c69 7374 3030 d801 0203 0405  .]bplist00......
-000066a0: 0607 0809 0a0b 1a46 470a 2758 6963 6f6e  .......FG.'Xicon
-000066b0: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-000066c0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-000066d0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-000066e0: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-000066f0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
-00006700: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
-00006710: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
-00006720: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
-00006730: 1314 151e 2328 2c31 363b 4058 636f 6d6d  ....#(,16;@Xcomm
-00006740: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-00006750: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-00006760: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-00006770: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00006780: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
-00006790: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-000067a0: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
-000067b0: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
-000067c0: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
-000067d0: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
-000067e0: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
-000067f0: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
-00006800: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
-00006810: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
-00006820: 1718 190a 420a 4409 10d0 0910 0008 2340  ....B.D.......#@
-00006830: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
-00006840: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
-00006850: 8c00 9500 9600 a900 b200 c100 ce00 da00  ................
-00006860: df00 e500 ea00 f200 f701 0001 0801 0e01  ................
-00006870: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
-00006880: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
-00006890: 4c01 4d01 4e01 5001 5901 5a01 5c01 5d01  L.M.N.P.Y.Z.\.].
-000068a0: 5f01 6801 6901 6b01 6c01 6e01 7701 7801  _.h.i.k.l.n.w.x.
-000068b0: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
-000068c0: 9501 9601 9801 9901 9b01 9c01 a501 aa00  ................
-000068d0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
-000068e0: 0000 0000 0000 0000 0000 0000 0001 ab00  ................
-000068f0: 0000 0900 7200 6f00 6900 5f00 7400 6f00  ....r.o.i._.t.o.
-00006900: 6f00 6c00 736d 6f44 4462 6c6f 6200 0000  o.l.smoDDblob...
-00006910: 080a af5f 86d0 fec4 4100 0000 0900 7200  ..._....A.....r.
-00006920: 6f00 6900 5f00 7400 6f00 6f00 6c00 736d  o.i._.t.o.o.l.sm
-00006930: 6f64 4462 6c6f 6200 0000 08b5 b22b b8e5  odDblob......+..
-00006940: fcc4 4100 0000 0900 7200 6f00 6900 5f00  ..A.....r.o.i._.
-00006950: 7400 6f00 6f00 6c00 7370 6831 5363 6f6d  t.o.o.l.sph1Scom
-00006960: 7000 0000 0000 0510 0000 0000 0900 7200  p.............r.
-00006970: 6f00 6900 5f00 7400 6f00 6f00 6c00 7376  o.i._.t.o.o.l.sv
-00006980: 5372 6e6c 6f6e 6700 0000 0100 0000 1b00  Srnlong.........
-00006990: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
-000069a0: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
-000069b0: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
-000069c0: 6500 7200 7362 7773 7062 6c6f 6200 0000  e.r.sbwspblob...
-000069d0: c962 706c 6973 7430 30d7 0102 0304 0506  .bplist00.......
-000069e0: 0708 080a 080a 0d0a 5d53 686f 7753 7461  ........]ShowSta
-000069f0: 7475 7342 6172 5b53 686f 7750 6174 6862  tusBar[ShowPathb
-00006a00: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
-00006a10: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
-00006a20: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
-00006a30: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
-00006a40: 686f 7753 6964 6562 6172 0808 0908 095f  howSidebar....._
-00006a50: 1018 7b7b 3332 2c20 3132 337d 2c20 7b31  ..{{32, 123}, {1
-00006a60: 3230 332c 2037 3534 7d7d 0908 1725 313d  203, 754}}...%1=
-00006a70: 4960 6d79 7a7b 7c7d 7e99 0000 0000 0000  I`myz{|}~.......
-00006a80: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00006a90: 0000 0000 0000 0000 009a 0000 001b 0074  ...............t
-00006aa0: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
-00006ab0: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
-00006ac0: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
-00006ad0: 0072 0073 6c67 3153 636f 6d70 0000 0000  .r.slg1Scomp....
-00006ae0: 0002 1ab6 0000 001b 0074 0068 0069 0072  .........t.h.i.r
-00006af0: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
-00006b00: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
-00006b10: 0070 0065 006e 0064 0065 0072 0073 6c73  .p.e.n.d.e.r.sls
-00006b20: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
-00006b30: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
-00006b40: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-00006b50: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00006b60: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00006b70: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00006b80: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00006b90: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-00006ba0: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-00006bb0: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-00006bc0: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
-00006bd0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00006be0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-00006bf0: 7209 1101 a609 546e 616d 65d4 0d0e 0f10  r.....Tname.....
-00006c00: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00006c10: 79d4 0d0e 0f10 0a1c 161e 0910 b508 5c64  y.............\d
-00006c20: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
-00006c30: 161c 1622 0808 5b64 6174 6543 7265 6174  ..."..[dateCreat
-00006c40: 6564 d40d 0e0f 100a 2516 2709 1061 0854  ed......%.'..a.T
-00006c50: 7369 7a65 d40d 0e0f 100a 2a0a 2c09 1073  size......*.,..s
-00006c60: 0954 6b69 6e64 d40d 0e0f 1016 2f0a 3108  .Tkind....../.1.
-00006c70: 1064 0955 6c61 6265 6cd4 0d0e 0f10 1634  .d.Ulabel......4
-00006c80: 0a36 0810 4b09 5776 6572 7369 6f6e d40d  .6..K.Wversion..
-00006c90: 0e0f 1016 390a 3b08 1101 2c09 5863 6f6d  ....9.;...,.Xcom
-00006ca0: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
-00006cb0: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00006cc0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
-00006cd0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-00006ce0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-00006cf0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-00006d00: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
-00006d10: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
-00006d20: dd00 de00 e700 f000 f100 f300 f401 0101  ................
-00006d30: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
-00006d40: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
-00006d50: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
-00006d60: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
-00006d70: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
-00006d80: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-00006d90: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00006da0: 0001 c5c4 6108 09d4 0f10 1112 2b2c 0c0c  ....a.......+,..
-00006db0: 546b 696e 6410 7309 09d4 0f10 1112 3031  Tkind.s.......01
-00006dc0: 0c1a 556c 6162 656c 1064 0908 d40f 1011  ..Ulabel.d......
-00006dd0: 1235 360c 1a57 7665 7273 696f 6e10 4b09  .56..Wversion.K.
-00006de0: 08d4 0f10 1112 3a3b 0c1a 5863 6f6d 6d65  ......:;..Xcomme
-00006df0: 6e74 7311 012c 0908 d40f 1011 123f 401a  nts..,.......?@.
-00006e00: 1a5e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00006e10: 10c8 0808 d40f 1011 1244 1e1a 1a59 6461  .........D...Yda
-00006e20: 7465 4164 6465 6408 0808 2300 0000 0000  teAdded...#.....
-00006e30: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00006e40: 6509 1001 0008 001d 0026 0038 0040 0054  e........&.8.@.T
-00006e50: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
-00006e60: 00ca 00d3 00de 00e4 00ee 00f6 00fb 00fe  ................
-00006e70: 00ff 0100 0109 0112 0114 0115 0116 011f  ................
-00006e80: 012c 012e 012f 0130 0139 0145 0146 0147  .,.../.0.9.E.F.G
-00006e90: 0150 0155 0157 0158 0159 0162 0167 0169  .P.U.W.X.Y.b.g.i
-00006ea0: 016a 016b 0174 017a 017c 017d 017e 0187  .j.k.t.z.|.}.~..
-00006eb0: 018f 0191 0192 0193 019c 01a5 01a8 01a9  ................
-00006ec0: 01aa 01b3 01c2 01c4 01c5 01c6 01cf 01d9  ................
-00006ed0: 01da 01db 01dc 01e5 01ee 01f3 01f4 0000  ................
-00006ee0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-00006ef0: 0000 0000 0000 0000 0000 0000 01f6 7430  ..............t0
-00006f00: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00006f10: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00006f20: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00006f30: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00006f40: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00006f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00006f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00006f70: 6172 0808 0908 095f 1018 7b7b 3635 372c  ar....._..{{657,
-00006f80: 2032 3730 7d2c 207b 3938 392c 2034 3336   270}, {989, 436
-00006f90: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00006fa0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-00006fb0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00006fc0: 009a 0000 0000 0000 0000 0000 0000 0000  ................
-00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006000: 0000 0000 0000 0000 0000 0015 0000 001b  ................
+00006010: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
+00006020: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
+00006030: 006f 006e 0073 005f 0061 0072 0063 0068  .o.n.s._.a.r.c.h
+00006040: 0069 0076 0065 6c67 3153 636f 6d70 0000  .i.v.elg1Scomp..
+00006050: 0000 0006 faed 0000 001b 0070 006f 0073  ...........p.o.s
+00006060: 0065 005f 0063 006f 006e 0066 0069 0067  .e._.c.o.n.f.i.g
+00006070: 0075 0072 0061 0074 0069 006f 006e 0073  .u.r.a.t.i.o.n.s
+00006080: 005f 0061 0072 0063 0068 0069 0076 0065  ._.a.r.c.h.i.v.e
+00006090: 6d6f 4444 626c 6f62 0000 0008 8983 1ea9  moDDblob........
+000060a0: cbfe c441 0000 001b 0070 006f 0073 0065  ...A.....p.o.s.e
+000060b0: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
+000060c0: 0072 0061 0074 0069 006f 006e 0073 005f  .r.a.t.i.o.n.s._
+000060d0: 0061 0072 0063 0068 0069 0076 0065 6d6f  .a.r.c.h.i.v.emo
+000060e0: 6444 626c 6f62 0000 0008 8983 1ea9 cbfe  dDblob..........
+000060f0: c441 0000 001b 0070 006f 0073 0065 005f  .A.....p.o.s.e._
+00006100: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
+00006110: 0061 0074 0069 006f 006e 0073 005f 0061  .a.t.i.o.n.s._.a
+00006120: 0072 0063 0068 0069 0076 0065 7068 3153  .r.c.h.i.v.eph1S
+00006130: 636f 6d70 0000 0000 0007 9000 0000 000e  comp............
+00006140: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
+00006150: 006f 0072 0074 0065 0072 0073 6277 7370  .o.r.t.e.r.sbwsp
+00006160: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
+00006170: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
+00006180: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+00006190: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
+000061a0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+000061b0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+000061c0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+000061d0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+000061e0: 7208 0809 0809 5f10 197b 7b36 3432 2c20  r....._..{{642, 
+000061f0: 3132 397d 2c20 7b31 3031 352c 2037 3637  129}, {1015, 767
+00006200: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+00006210: 7e9a 0000 0000 0000 0101 0000 0000 0000  ~...............
+00006220: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+00006230: 009b 0000 000e 0070 006f 0073 0065 005f  .......p.o.s.e._
+00006240: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
+00006250: 0073 6c67 3153 636f 6d70 0000 0000 0003  .slg1Scomp......
+00006260: fb81 0000 000e 0070 006f 0073 0065 005f  .......p.o.s.e._
+00006270: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
+00006280: 0073 6c73 7643 626c 6f62 0000 0278 6270  .slsvCblob...xbp
+00006290: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
+000062a0: 0a0b 1646 4748 0a5f 1012 7669 6577 4f70  ...FGH._..viewOp
+000062b0: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
+000062c0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+000062d0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+000062e0: 7465 416c 6c53 697a 6573 5874 6578 7453  teAllSizesXtextS
+000062f0: 697a 655a 736f 7274 436f 6c75 6d6e 5869  izeZsortColumnXi
+00006300: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
+00006310: 6174 6976 6544 6174 6573 1001 09ab 0c15  ativeDates......
+00006320: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 0a12  ..#(-27<A.......
+00006330: 0a14 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+00006340: 5961 7363 656e 6469 6e67 5a69 6465 6e74  YascendingZident
+00006350: 6966 6965 7209 10ea 0954 6e61 6d65 d40d  ifier....Tname..
+00006360: 0e0f 1016 1716 1908 1023 0858 7562 6971  .........#.Xubiq
+00006370: 7569 7479 d40d 0e0f 100a 1c16 1e09 10b5  uity............
+00006380: 085c 6461 7465 4d6f 6469 6669 6564 d40d  .\dateModified..
+00006390: 0e0f 1016 1c16 2208 085b 6461 7465 4372  ......"..[dateCr
+000063a0: 6561 7465 64d4 0d0e 0f10 0a25 1627 0910  eated......%.'..
+000063b0: 6108 5473 697a 65d4 0d0e 0f10 0a2a 0a2c  a.Tsize......*.,
+000063c0: 0910 7309 546b 696e 64d4 0d0e 0f10 162f  ..s.Tkind....../
+000063d0: 0a31 0810 6409 556c 6162 656c d40d 0e0f  .1..d.Ulabel....
+000063e0: 1016 340a 3608 104b 0957 7665 7273 696f  ..4.6..K.Wversio
+000063f0: 6ed4 0d0e 0f10 1639 0a3b 0811 012c 0958  n......9.;...,.X
+00006400: 636f 6d6d 656e 7473 d40d 0e0f 1016 3e16  comments......>.
+00006410: 4008 10c8 085e 6461 7465 4c61 7374 4f70  @....^dateLastOp
+00006420: 656e 6564 d40d 0e0f 1016 1c16 4408 0859  ened........D..Y
+00006430: 6461 7465 4164 6465 6408 2340 2800 0000  dateAdded.#@(...
+00006440: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
+00006450: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+00006460: 0070 0079 008c 008e 008f 009b 00a4 00ac  .p.y............
+00006470: 00b2 00bc 00c7 00c8 00ca 00cb 00d0 00d9  ................
+00006480: 00da 00dc 00dd 00e6 00ef 00f0 00f2 00f3  ................
+00006490: 0100 0109 010a 010b 0117 0120 0121 0123  ........... .!.#
+000064a0: 0124 0129 0132 0133 0135 0136 013b 0144  .$.).2.3.5.6.;.D
+000064b0: 0145 0147 0148 014e 0157 0158 015a 015b  .E.G.H.N.W.X.Z.[
+000064c0: 0163 016c 016d 0170 0171 017a 0183 0184  .c.l.m.p.q.z....
+000064d0: 0186 0187 0196 019f 01a0 01a1 01ab 01ac  ................
+000064e0: 01b5 01ba 01c3 0000 0000 0000 0201 0000  ................
+000064f0: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
+00006500: 0000 0000 01c4 0000 000e 0070 006f 0073  ...........p.o.s
+00006510: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
+00006520: 0065 0072 0073 6c73 7670 626c 6f62 0000  .e.r.slsvpblob..
+00006530: 025d 6270 6c69 7374 3030 d801 0203 0405  .]bplist00......
+00006540: 0607 0809 0a0b 1d45 4647 0a5f 1012 7669  .......EFG._..vi
+00006550: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00006560: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00006570: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00006580: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00006590: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+000065a0: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+000065b0: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
+000065c0: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
+000065d0: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
+000065e0: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+000065f0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+00006600: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00006610: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00006620: 6d65 d416 1718 191a 1b0a 1d55 696e 6465  me.........Uinde
+00006630: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
+00006640: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
+00006650: d416 1718 191f 201d 1d10 0810 c808 08d4  ...... .........
+00006660: 1617 1819 0924 1d0a 10b5 0809 d416 1718  .....$..........
+00006670: 1928 241d 1d10 0208 08d4 1617 1819 2c2d  .($...........,-
+00006680: 1d0a 1003 1061 0809 d416 1718 1931 320a  .....a.......12.
+00006690: 1d10 0510 6409 08d4 1617 1819 3637 0a0a  ....d.......67..
+000066a0: 1004 1073 0909 d416 1718 193b 3c0a 1d10  ...s.......;<...
+000066b0: 0610 4b09 08d4 1617 1819 4041 0a0a 1000  ..K.......@A....
+000066c0: 10ea 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+000066d0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
+000066e0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
+000066f0: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
+00006700: d800 de00 e300 eb00 f000 f900 ff01 0501  ................
+00006710: 0f01 1701 1901 1c01 1d01 1e01 2701 2901  ............'.).
+00006720: 2b01 2c01 2d01 3601 3801 3901 3a01 4301  +.,.-.6.8.9.:.C.
+00006730: 4501 4601 4701 5001 5201 5401 5501 5601  E.F.G.P.R.T.U.V.
+00006740: 5f01 6101 6301 6401 6501 6e01 7001 7201  _.a.c.d.e.n.p.r.
+00006750: 7301 7401 7d01 7f01 8101 8201 8301 8c01  s.t.}...........
+00006760: 8e01 9001 9101 9201 9301 9c01 a101 aa00  ................
+00006770: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
+00006780: 0000 0000 0000 0000 0000 0000 0001 ab00  ................
+00006790: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
+000067a0: 6d00 7000 6f00 7200 7400 6500 7200 736d  m.p.o.r.t.e.r.sm
+000067b0: 6f44 4462 6c6f 6200 0000 0890 22c3 eb97  oDDblob....."...
+000067c0: ffc4 4100 0000 0e00 7000 6f00 7300 6500  ..A.....p.o.s.e.
+000067d0: 5f00 6900 6d00 7000 6f00 7200 7400 6500  _.i.m.p.o.r.t.e.
+000067e0: 7200 736d 6f64 4462 6c6f 6200 0000 0890  r.smodDblob.....
+000067f0: 22c3 eb97 ffc4 4100 0000 0e00 7000 6f00  ".....A.....p.o.
+00006800: 7300 6500 5f00 6900 6d00 7000 6f00 7200  s.e._.i.m.p.o.r.
+00006810: 7400 6500 7200 7370 6831 5363 6f6d 7000  t.e.r.sph1Scomp.
+00006820: 0000 0000 04a0 0000 0000 0e00 7000 6f00  ............p.o.
+00006830: 7300 6500 5f00 6900 6d00 7000 6f00 7200  s.e._.i.m.p.o.r.
+00006840: 7400 6500 7200 7376 5372 6e6c 6f6e 6700  t.e.r.svSrnlong.
+00006850: 0000 0100 0000 0f00 7000 6f00 7300 6500  ........p.o.s.e.
+00006860: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00006870: 6f00 7200 7362 7773 7062 6c6f 6200 0000  o.r.sbwspblob...
+00006880: c962 706c 6973 7430 30d7 0102 0304 0506  .bplist00.......
+00006890: 0708 080a 080a 0d0a 5d53 686f 7753 7461  ........]ShowSta
+000068a0: 7475 7342 6172 5b53 686f 7750 6174 6862  tusBar[ShowPathb
+000068b0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+000068c0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+000068d0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+000068e0: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+000068f0: 686f 7753 6964 6562 6172 0808 0908 095f  howSidebar....._
+00006900: 1018 7b7b 3635 372c 2032 3730 7d2c 207b  ..{{657, 270}, {
+00006910: 3938 392c 2034 3336 7d7d 0908 1725 313d  989, 436}}...%1=
+00006920: 4960 6d79 7a7b 7c7d 7e99 0000 0000 0000  I`myz{|}~.......
+00006930: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00006940: 0000 0000 0000 0000 009a 0000 000f 0070  ...............p
+00006950: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
+00006960: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
+00006970: 636f 6d70 0000 0000 0000 84be 0000 000f  comp............
+00006980: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
+00006990: 0063 0065 0073 0073 006f 0072 0073 6d6f  .c.e.s.s.o.r.smo
+000069a0: 4444 626c 6f62 0000 0008 9e55 85d0 97fe  DDblob.....U....
+000069b0: c441 0000 000f 0070 006f 0073 0065 005f  .A.....p.o.s.e._
+000069c0: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
+000069d0: 0072 0073 6d6f 6444 626c 6f62 0000 0008  .r.smodDblob....
+000069e0: 9e55 85d0 97fe c441 0000 000f 0070 006f  .U.....A.....p.o
+000069f0: 0073 0065 005f 0070 0072 006f 0063 0065  .s.e._.p.r.o.c.e
+00006a00: 0073 0073 006f 0072 0073 7068 3153 636f  .s.s.o.r.sph1Sco
+00006a10: 6d70 0000 0000 0000 d000 0000 000f 0070  mp.............p
+00006a20: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
+00006a30: 0065 0073 0073 006f 0072 0073 7653 726e  .e.s.s.o.r.svSrn
+00006a40: 6c6f 6e67 0000 0001 0000 0009 0072 006f  long.........r.o
+00006a50: 0069 005f 0074 006f 006f 006c 0073 6277  .i._.t.o.o.l.sbw
+00006a60: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
+00006a70: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
+00006a80: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00006a90: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
+00006aa0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00006ab0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00006ac0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00006ad0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00006ae0: 6261 7208 0809 0809 5f10 187b 7b36 3537  bar....._..{{657
+00006af0: 2c20 3237 307d 2c20 7b39 3839 2c20 3433  , 270}, {989, 43
+00006b00: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
+00006b10: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
+00006b20: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+00006b30: 0000 9a00 0000 0900 7200 6f00 6900 5f00  ........r.o.i._.
+00006b40: 7400 6f00 6f00 6c00 736c 6731 5363 6f6d  t.o.o.l.slg1Scom
+00006b50: 7000 0000 0000 0425 3e00 0000 0900 7200  p......%>.....r.
+00006b60: 6f00 6900 5f00 7400 6f00 6f00 6c00 736c  o.i._.t.o.o.l.sl
+00006b70: 7376 4362 6c6f 6200 0002 7862 706c 6973  svCblob...xbplis
+00006b80: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+00006b90: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
+00006ba0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00006bb0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00006bc0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+00006bd0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+00006be0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00006bf0: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+00006c00: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+00006c10: 09ab 0c15 1a1f 2328 2d32 373c 41d4 0d0e  ......#(-27<A...
+00006c20: 0f10 1112 0a0a 5a69 6465 6e74 6966 6965  ......Zidentifie
+00006c30: 7255 7769 6474 6859 6173 6365 6e64 696e  rUwidthYascendin
+00006c40: 6757 7669 7369 626c 6554 6e61 6d65 10d0  gWvisibleTname..
+00006c50: 0909 d40d 0e0f 1016 1718 1858 7562 6971  ...........Xubiq
+00006c60: 7569 7479 1023 0808 d40d 0e0f 101b 1c18  uity.#..........
+00006c70: 0a5c 6461 7465 4d6f 6469 6669 6564 10b5  .\dateModified..
+00006c80: 0809 d40d 0e0f 1020 1c18 185b 6461 7465  ....... ...[date
+00006c90: 4372 6561 7465 6408 08d4 0d0e 0f10 2425  Created.......$%
+00006ca0: 180a 5473 697a 6510 6108 09d4 0d0e 0f10  ..Tsize.a.......
+00006cb0: 292a 0a0a 546b 696e 6410 7309 09d4 0d0e  )*..Tkind.s.....
+00006cc0: 0f10 2e2f 0a18 556c 6162 656c 1064 0908  .../..Ulabel.d..
+00006cd0: d40d 0e0f 1033 340a 1857 7665 7273 696f  .....34..Wversio
+00006ce0: 6e10 4b09 08d4 0d0e 0f10 3839 0a18 5863  n.K.......89..Xc
+00006cf0: 6f6d 6d65 6e74 7311 012c 0908 d40d 0e0f  omments..,......
+00006d00: 103d 3e18 185e 6461 7465 4c61 7374 4f70  .=>..^dateLastOp
+00006d10: 656e 6564 10c8 0808 d40d 0e0f 1042 1c18  ened.........B..
+00006d20: 1859 6461 7465 4164 6465 6408 0808 2340  .YdateAdded...#@
+00006d30: 2800 0000 0000 0054 6e61 6d65 0910 0100  (......Tname....
+00006d40: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
+00006d50: 7700 8c00 9500 9600 a200 ab00 b600 bc00  w...............
+00006d60: c600 ce00 d300 d500 d600 d700 e000 e900  ................
+00006d70: eb00 ec00 ed00 f601 0301 0501 0601 0701  ................
+00006d80: 1001 1c01 1d01 1e01 2701 2c01 2e01 2f01  ........'.,.../.
+00006d90: 3001 3901 3e01 4001 4101 4201 4b01 5101  0.9.>.@.A.B.K.Q.
+00006da0: 5301 5401 5501 5e01 6601 6801 6901 6a01  S.T.U.^.f.h.i.j.
+00006db0: 7301 7c01 7f01 8001 8101 8a01 9901 9b01  s.|.............
+00006dc0: 9c01 9d01 a601 b001 b101 b201 b301 bc01  ................
+00006dd0: c101 c200 0000 0000 0002 0100 0000 0000  ................
+00006de0: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00006df0: 0001 c410 03d4 1819 1a1b 1c35 0b37 0810  ...........5.7..
+00006e00: 6409 1005 d418 191a 1b0b 3a0b 3c09 1073  d.........:.<..s
+00006e10: 0910 04d4 1819 1a1b 1c3f 0b41 0810 4b09  .........?.A..K.
+00006e20: 1006 d418 191a 1b0b 440b 4609 1101 2709  ........D.F...'.
+00006e30: 1000 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
+00006e40: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+00006e50: 0000 0000 0800 1d00 3000 4200 4a00 5e00  ........0.B.J.^.
+00006e60: 7000 7900 8b00 9600 9f00 b400 b500 b600  p.y.............
+00006e70: c900 d200 e100 ee00 fa00 ff01 0501 0a01  ................
+00006e80: 1201 1701 2001 2801 2e01 3801 3e01 3f01  .... .(...8.>.?.
+00006e90: 4201 4301 4501 4e01 4f01 5101 5201 5401  B.C.E.N.O.Q.R.T.
+00006ea0: 5d01 5e01 6001 6101 6301 6c01 6d01 6e01  ].^.`.a.c.l.m.n.
+00006eb0: 7001 7901 7a01 7c01 7d01 7f01 8801 8901  p.y.z.|.}.......
+00006ec0: 8b01 8c01 8e01 9701 9801 9a01 9b01 9d01  ................
+00006ed0: a601 a701 a901 aa01 ac01 b501 b601 b901  ................
+00006ee0: ba01 bc01 bd01 c601 cf01 d400 0000 0000  ................
+00006ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
+00006f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
+00006f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+00006f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+00006f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
+00006f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
+00006f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00006f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00006f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
+00006f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
+00006f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
+00006fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00006fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
+00006fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00006fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00006fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007000: 0000 0000 0000 0000 0000 000f 0000 001b  ................
-00007010: 0074 0068 0069 0072 0064 005f 0070 0061  .t.h.i.r.d._.p.a
-00007020: 0072 0074 0079 005f 006c 0061 0062 0065  .r.t.y._.l.a.b.e
-00007030: 006c 005f 0061 0070 0070 0065 006e 0064  .l._.a.p.p.e.n.d
-00007040: 0065 0072 0073 6d6f 4444 626c 6f62 0000  .e.r.smoDDblob..
-00007050: 0008 801f e384 2efe c441 0000 001b 0074  .........A.....t
-00007060: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
-00007070: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
-00007080: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
-00007090: 0072 0073 6d6f 6444 626c 6f62 0000 0008  .r.smodDblob....
-000070a0: 4c89 caff 10fc c441 0000 001b 0074 0068  L......A.....t.h
+00007000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
+00007010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
+00007020: 0073 6d6f 4444 626c 6f62 0000 0008 2506  .smoDDblob....%.
+00007030: b721 6f01 c541 0000 0009 0072 006f 0069  .!o..A.....r.o.i
+00007040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
+00007050: 626c 6f62 0000 0008 b5b2 2bb8 e5fc c441  blob......+....A
+00007060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
+00007070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
+00007080: 0000 0005 1000 0000 0009 0072 006f 0069  ...........r.o.i
+00007090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
+000070a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
 000070b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
 000070c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
 000070d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
-000070e0: 0073 7068 3153 636f 6d70 0000 0000 0002  .sph1Scomp......
-000070f0: b000 0000 001b 0074 0068 0069 0072 0064  .......t.h.i.r.d
-00007100: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
-00007110: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
-00007120: 0065 006e 0064 0065 0072 0073 7653 726e  .e.n.d.e.r.svSrn
-00007130: 6c6f 6e67 0000 0001 0000 0002 0075 0069  long.........u.i
-00007140: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
-00007150: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
-00007160: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00007170: 725b 5368 6f77 5061 7468 6261 725b 5368  r[ShowPathbar[Sh
-00007180: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00007190: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-000071a0: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-000071b0: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-000071c0: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
-000071d0: 3532 2c20 3234 377d 2c20 7b39 3839 2c20  52, 247}, {989, 
-000071e0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
-000071f0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
-00007200: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
-00007210: 0000 0000 9a00 0000 0200 7500 6964 7363  ..........u.idsc
-00007220: 6c62 6f6f 6c00 0000 0002 0075 0069 6c67  lbool......u.ilg
-00007230: 3153 636f 6d70 0000 0000 000b 8aaf 0000  1Scomp..........
-00007240: 0002 0075 0069 6d6f 4444 626c 6f62 0000  ...u.imoDDblob..
-00007250: 0008 6f49 0e2b 55ff c441 0000 0002 0075  ..oI.+U..A.....u
-00007260: 0069 6d6f 6444 626c 6f62 0000 0008 6f49  .imodDblob....oI
-00007270: 0e2b 55ff c441 0000 0002 0075 0069 7068  .+U..A.....u.iph
-00007280: 3153 636f 6d70 0000 0000 000e 9000 0000  1Scomp..........
-00007290: 0002 0075 0069 7653 726e 6c6f 6e67 0000  ...u.ivSrnlong..
-000072a0: 0001 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
-000072b0: 0065 0072 0076 0069 0073 0065 0064 6277  .e.r.v.i.s.e.dbw
-000072c0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
-000072d0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
-000072e0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-000072f0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
-00007300: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00007310: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00007320: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00007330: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00007340: 6261 7208 0809 0809 5f10 197b 7b32 3630  bar....._..{{260
-00007350: 2c20 3136 327d 2c20 7b31 3138 302c 2035  , 162}, {1180, 5
-00007360: 3538 7d7d 0908 1725 313d 4960 6d79 7a7b  58}}...%1=I`myz{
-00007370: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
-00007380: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-00007390: 0000 009b 0000 000c 0075 006e 0073 0075  .........u.n.s.u
-000073a0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-000073b0: 6473 636c 626f 6f6c 0000 0000 0c00 7500  dsclbool......u.
-000073c0: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
-000073d0: 7300 6500 646c 6731 5363 6f6d 7000 0000  s.e.dlg1Scomp...
-000073e0: 0000 05d0 3500 0000 0c00 7500 6e00 7300  ....5.....u.n.s.
-000073f0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00007400: 646c 7376 4362 6c6f 6200 0002 9762 706c  dlsvCblob....bpl
-00007410: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
-00007420: 0b19 494a 0a4c 5f10 1276 6965 774f 7074  ..IJ.L_..viewOpt
-00007430: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
-00007440: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00007450: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00007460: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00007470: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00007480: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00007490: 5869 636f 6e53 697a 6510 0109 ab0c 151d  XiconSize.......
-000074a0: 2226 2b30 353a 3f44 d40d 0e0f 100a 0a13  "&+05:?D........
-000074b0: 1457 7669 7369 626c 6559 6173 6365 6e64  .WvisibleYascend
-000074c0: 696e 6755 7769 6474 685a 6964 656e 7469  ingUwidthZidenti
-000074d0: 6669 6572 0909 1101 8f54 6e61 6d65 d416  fier.....Tname..
-000074e0: 1718 1019 1a19 1c57 7669 7369 626c 6555  .......WvisibleU
-000074f0: 7769 6474 6859 6173 6365 6e64 696e 6708  widthYascending.
-00007500: 1023 0858 7562 6971 7569 7479 d40d 0e0f  .#.Xubiquity....
-00007510: 100a 1920 2109 0810 b55c 6461 7465 4d6f  ... !....\dateMo
-00007520: 6469 6669 6564 d40d 0e0f 1019 1920 2508  dified....... %.
-00007530: 085b 6461 7465 4372 6561 7465 64d4 0d0e  .[dateCreated...
-00007540: 0f10 0a19 292a 0908 1061 5473 697a 65d4  ....)*...aTsize.
-00007550: 0d0e 0f10 0a0a 2e2f 0909 1073 546b 696e  ......./...sTkin
-00007560: 64d4 0d0e 0f10 190a 3334 0809 1064 556c  d.......34...dUl
-00007570: 6162 656c d40d 0e0f 1019 0a38 3908 0910  abel.......89...
-00007580: 4b57 7665 7273 696f 6ed4 0d0e 0f10 190a  KWversion.......
-00007590: 3d3e 0809 1101 2c58 636f 6d6d 656e 7473  =>....,Xcomments
-000075a0: d40d 0e0f 1019 1942 4308 0810 c85e 6461  .......BC....^da
-000075b0: 7465 4c61 7374 4f70 656e 6564 d416 1718  teLastOpened....
-000075c0: 1019 2019 4708 0859 6461 7465 4164 6465  .. .G..YdateAdde
-000075d0: 6408 2340 2800 0000 0000 0054 6e61 6d65  d.#@(......Tname
-000075e0: 0923 4030 0000 0000 0000 0008 0019 002e  .#@0............
-000075f0: 0040 0048 005c 0065 0070 0083 008c 008e  .@.H.\.e.p......
-00007600: 008f 009b 00a4 00ac 00b6 00bc 00c7 00c8  ................
-00007610: 00c9 00cc 00d1 00da 00e2 00e8 00f2 00f3  ................
-00007620: 00f5 00f6 00ff 0108 0109 010a 010c 0119  ................
-00007630: 0122 0123 0124 0130 0139 013a 013b 013d  .".#.$.0.9.:.;.=
-00007640: 0142 014b 014c 014d 014f 0154 015d 015e  .B.K.L.M.O.T.].^
-00007650: 015f 0161 0167 0170 0171 0172 0174 017c  ._.a.g.p.q.r.t.|
-00007660: 0185 0186 0187 018a 0193 019c 019d 019e  ................
-00007670: 01a0 01af 01b8 01b9 01ba 01c4 01c5 01ce  ................
-00007680: 01d3 01d4 0000 0000 0000 0201 0000 0000  ................
-00007690: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
-000076a0: 0000 01dd 0a0b 1a46 470a 2758 6963 6f6e  .......FG.'Xicon
-000076b0: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
-000076c0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-000076d0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-000076e0: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-000076f0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
-00007700: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
-00007710: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
-00007720: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
-00007730: 1314 151e 2328 2c31 363b 4058 636f 6d6d  ....#(,16;@Xcomm
-00007740: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-00007750: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-00007760: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-00007770: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00007780: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
-00007790: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-000077a0: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
-000077b0: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
-000077c0: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
-000077d0: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
-000077e0: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
-000077f0: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
-00007800: d416 1718 0000 000a 0000 0000 0000 780b  ..............x.
-00007810: 0000 0045 0000 100c 0000 800c 0000 200c  ...E.......... .
-00007820: 0000 300c 0000 400c 0000 500c 0000 600c  ..0...@...P...`.
-00007830: 0000 700b 0000 0000 0000 0000 0000 0000  ..p.............
-00007840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000078a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000078b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000078c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000078d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000078e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000078f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000079a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000079b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000079c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000079d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000079e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000079f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00007c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
-00007c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00007c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00007c50: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-00007c60: 0100 0008 0000 0000 0100 0090 0000 0000  ................
-00007c70: 0100 00a0 0000 0000 0100 00c0 0000 0000  ................
-00007c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
-00007c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
-00007ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
-00007cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
-00007cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
-00007cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
-00007ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00007cf0: 0000 0000 0140 0000 0000 0000 0028 0130  .....@.......(.0
-00007d00: 0136 0140 0146 0147 014a 014b 014d 0156  .6.@.F.G.J.K.M.V
-00007d10: 0157 0159 015a 015c 0165 0166 0168 0169  .W.Y.Z.\.e.f.h.i
-00007d20: 016b 0174 0175 0176 0178 0181 0182 0184  .k.t.u.v.x......
-00007d30: 0185 0187 0190 0191 0193 0194 0196 019f  ................
-00007d40: 01a0 01a2 01a3 01a5 01ae 01af 01b1 01b2  ................
-00007d50: 01b4 01bd 01be 01c1 01c2 01c4 01c5 01ce  ................
-00007d60: 01d7 01dc 0000 0000 0000 0201 0000 0000  ................
-00007d70: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
-00007d80: 0000 01dd 0000 0007 0000 000e 0070 006f  .............p.o
-00007d90: 0073 0065 005f 0069 006d 0070 006f 0072  .s.e._.i.m.p.o.r
-00007da0: 0074 0065 0072 0073 6c73 7670 626c 6f62  .t.e.r.slsvpblob
-00007db0: 0000 025d 6270 6c69 7374 3030 d801 0203  ...]bplist00....
-00007dc0: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
-00007dd0: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00007de0: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00007df0: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00007e00: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00007e10: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-00007e20: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-00007e30: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00007e40: 1001 09d9 0c0d 0e0f 1011 1213 1415 1e23  ...............#
-00007e50: 272b 3035 3a3f 5863 6f6d 6d65 6e74 735e  '+05:?Xcomments^
-00007e60: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
-00007e70: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
-00007e80: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
-00007e90: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
-00007ea0: 6e61 6d65 d416 1718 191a 1b0a 1d55 696e  name.........Uin
-00007eb0: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
-00007ec0: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
-00007ed0: 0908 d416 1718 191f 201d 1d10 0810 c808  ........ .......
-00007ee0: 08d4 1617 1819 0924 1d0a 10b5 0809 d416  .......$........
-00007ef0: 1718 1928 241d 1d10 0208 08d4 1617 1819  ...($...........
-00007f00: 2c2d 1d0a 1003 1061 0809 d416 1718 1931  ,-.....a.......1
-00007f10: 320a 1d10 0510 6409 08d4 1617 1819 3637  2.....d.......67
-00007f20: 0a0a 1004 1073 0909 d416 1718 193b 3c0a  .....s.......;<.
-00007f30: 1d10 0610 4b09 08d4 1617 1819 4041 0a0a  ....K.......@A..
-00007f40: 1000 10ea 0909 0823 4028 0000 0000 0000  .......#@(......
-00007f50: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-00007f60: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-00007f70: 7900 8c00 8e00 8f00 a200 ab00 ba00 c700  y...............
-00007f80: d300 d800 de00 e300 eb00 f000 f900 ff01  ................
-00007f90: 0501 0f01 1701 1901 1c01 1d01 1e01 2701  ..............'.
-00007fa0: 2901 2b01 2c01 2d01 3601 3801 3901 3a01  ).+.,.-.6.8.9.:.
-00007fb0: 4301 4501 4601 4701 5001 5201 5401 5501  C.E.F.G.P.R.T.U.
-00007fc0: 5601 5f01 6101 6301 6401 6501 6e01 7001  V._.a.c.d.e.n.p.
-00007fd0: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
-00007fe0: 8c01 8e01 9001 9101 9201 9301 9c01 a101  ................
-00007ff0: aa00 0000 0000 0002 0100 0000 0000 0000  ................
-00008000: 4900 0000 0000 0002 0000 0006 0000 0004  I...............
-00008010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
-00008020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
-00008030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
-00008040: 0000 025d 6270 6c69 7374 3030 d801 0203  ...]bplist00....
-00008050: 0405 0607 0809 0a0b 1a46 470a 2758 6963  .........FG.'Xic
-00008060: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00008070: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00008080: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00008090: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-000080a0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-000080b0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-000080c0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-000080d0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
-000080e0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
-000080f0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
-00008100: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
-00008110: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00008120: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00008130: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
-00008140: 1a1b 0a1d 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
-00008150: 7468 5961 7363 656e 6469 6e67 5569 6e64  thYascendingUind
-00008160: 6578 0811 012c 0910 07d4 1617 1819 1a20  ex...,......... 
-00008170: 1a22 0810 c808 1008 d416 1718 190a 251a  ."............%.
-00008180: 2709 10b5 0810 01d4 1617 1819 1a25 1a2b  '............%.+
-00008190: 0808 1002 d416 1718 190a 2e1a 3009 1061  ............0..a
-000081a0: 0810 03d4 1617 1819 1a33 0a35 0810 6409  .........3.5..d.
-000081b0: 1005 d416 1718 190a 380a 3a09 1073 0910  ........8.:..s..
-000081c0: 04d4 1617 1819 1a3d 0a3f 0810 4b09 1006  .......=.?..K...
-000081d0: d416 1718 190a 420a 4409 10f0 0910 0008  ......B.D.......
-000081e0: 2340 2800 0000 0000 0054 6e61 6d65 0900  #@(......Tname..
-000081f0: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
-00008200: 7700 8c00 9500 9600 a900 b200 c100 ce00  w...............
-00008210: da00 df00 e500 ea00 f200 f701 0001 0801  ................
-00008220: 0e01 1801 1e01 1f01 2201 2301 2501 2e01  ........".#.%...
-00008230: 2f01 3101 3201 3401 3d01 3e01 4001 4101  /.1.2.4.=.>.@.A.
-00008240: 4301 4c01 4d01 4e01 5001 5901 5a01 5c01  C.L.M.N.P.Y.Z.\.
-00008250: 5d01 5f01 6801 6901 6b01 6c01 6e01 7701  ]._.h.i.k.l.n.w.
-00008260: 7801 7a01 7b01 7d01 8601 8701 8901 8a01  x.z.{.}.........
-00008270: 8c01 9501 9601 9801 9901 9b01 9c01 a501  ................
-00008280: aa00 0000 0000 0002 0100 0000 0000 0000  ................
-00008290: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-000082a0: ab00 0000 0500 0000 0900 6c00 6100 6200  ..........l.a.b.
-000082b0: 6500 6c00 6c00 6900 6e00 676c 6731 5363  e.l.l.i.n.glg1Sc
-000082c0: 6f6d 7000 0000 0000 018c 6a00 0000 0600  omp.......j.....
-000082d0: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-000082e0: 6e00 676c 7376 7062 6c6f 6200 0002 9562  n.glsvpblob....b
-000082f0: 706c 6973 7430 30da 0102 0304 0506 0708  plist00.........
-00008300: 090a 0b0c 0d1c 4849 484a 0c29 5869 636f  ......HIHJ.)Xico
-00008310: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
-00008320: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00008330: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00008340: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
-00008350: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
-00008360: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
-00008370: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00008380: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00008390: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-000083a0: 696f 6e23 4030 0000 0000 0000 09d9 0e0f  ion#@0..........
-000083b0: 1011 1213 1415 1617 2025 2a2e 3338 3d42  ........ %*.38=B
-000083c0: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
-000083d0: 7374 4f70 656e 6564 5c64 6174 654d 6f64  stOpened\dateMod
-000083e0: 6966 6965 645b 6461 7465 4372 6561 7465  ified[dateCreate
-000083f0: 6454 7369 7a65 556c 6162 656c 546b 696e  dTsizeUlabelTkin
-00008400: 6457 7665 7273 696f 6e54 6e61 6d65 d418  dWversionTname..
-00008410: 191a 1b1c 1d0c 1f57 7669 7369 626c 6555  .......WvisibleU
-00008420: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
-00008430: 696e 6465 7808 1101 2c09 1007 d418 191a  index...,.......
-00008440: 1b1c 221c 2408 10c8 0810 08d4 1819 1a1b  ..".$...........
-00008450: 0c27 1c29 0910 b508 1001 d418 191a 1b1c  .'.)............
-00008460: 271c 2d08 0810 02d4 1819 1a1b 0c30 1c32  '.-..........0.2
-00008470: 0910 6108 1003 d418 191a 1b1c 350c 3708  ..a.........5.7.
-00008480: 1064 0910 05d4 1819 1a1b 0c3a 0c3c 0910  .d.........:.<..
-00008490: 7309 1004 d418 191a 1b1c 3f0c 4108 104b  s.........?.A..K
-000084a0: 0910 06d4 1819 1a1b 0c44 0c46 0911 0127  .........D.F...'
-000084b0: 0910 0008 2300 0000 0000 0000 0023 4028  ....#........#@(
-000084c0: 0000 0000 0000 546e 616d 6509 0008 001d  ......Tname.....
-000084d0: 0026 0038 0040 0054 0066 006f 0081 008c  .&.8.@.T.f.o....
-000084e0: 009f 00b4 00bd 00be 00d1 00da 00e9 00f6  ................
-000084f0: 0102 0107 010d 0112 011a 011f 0128 0130  .............(.0
-00008500: 0136 0140 0146 0147 014a 014b 014d 0156  .6.@.F.G.J.K.M.V
-00008510: 0157 0159 015a 015c 0165 0166 0168 0169  .W.Y.Z.\.e.f.h.i
-00008520: 016b 0174 0175 0176 0178 0181 0182 0184  .k.t.u.v.x......
-00008530: 0185 0187 0190 0191 0193 0194 0196 019f  ................
-00008540: 01a0 01a2 01a3 01a5 01ae 01af 01b1 01b2  ................
-00008550: 01b4 01bd 01be 01c1 01c2 01c4 01c5 01ce  ................
-00008560: 01d7 01dc 0000 0000 0000 0201 0000 0000  ................
-00008570: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
-00008580: 0000 01dd 0000 0007 0000 000e 0070 006f  .............p.o
-00008590: 0073 0065 005f 0069 006d 0070 006f 0072  .s.e._.i.m.p.o.r
-000085a0: 0074 0065 0072 0073 6c73 7670 626c 6f62  .t.e.r.slsvpblob
-000085b0: 0000 025d 6270 6c69 7374 3030 d801 0203  ...]bplist00....
-000085c0: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
-000085d0: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-000085e0: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-000085f0: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00008600: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00008610: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-00008620: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-00008630: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00008640: 1001 09d9 0c0d 0e0f 1011 1213 1415 1e23  ...............#
-00008650: 272b 3035 3a3f 5863 6f6d 6d65 6e74 735e  '+05:?Xcomments^
-00008660: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
-00008670: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
-00008680: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
-00008690: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
-000086a0: 6e61 6d65 d416 1718 191a 1b0a 1d55 696e  name.........Uin
-000086b0: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
-000086c0: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
-000086d0: 0908 d416 1718 191f 201d 1d10 0810 c808  ........ .......
-000086e0: 08d4 1617 1819 0924 1d0a 10b5 0809 d416  .......$........
-000086f0: 1718 1928 241d 1d10 0208 08d4 1617 1819  ...($...........
-00008700: 2c2d 1d0a 1003 1061 0809 d416 1718 1931  ,-.....a.......1
-00008710: 320a 1d10 0510 6409 08d4 1617 1819 3637  2.....d.......67
-00008720: 0a0a 1004 1073 0909 d416 1718 193b 3c0a  .....s.......;<.
-00008730: 1d10 0610 4b09 08d4 1617 1819 4041 0a0a  ....K.......@A..
-00008740: 1000 10ea 0909 0823 4028 0000 0000 0000  .......#@(......
-00008750: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-00008760: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-00008770: 7900 8c00 8e00 8f00 a200 ab00 ba00 c700  y...............
-00008780: d300 d800 de00 e300 eb00 f000 f900 ff01  ................
-00008790: 0501 0f01 1701 1901 1c01 1d01 1e01 2701  ..............'.
-000087a0: 2901 2b01 2c01 2d01 3601 3801 3901 3a01  ).+.,.-.6.8.9.:.
-000087b0: 4301 4501 4601 4701 5001 5201 5401 5501  C.E.F.G.P.R.T.U.
-000087c0: 5601 5f01 6101 6301 6401 6501 6e01 7001  V._.a.c.d.e.n.p.
-000087d0: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
-000087e0: 8c01 8e01 9001 9101 9201 9301 9c01 a101  ................
-000087f0: aa00 0000 0000 0002 0100 0000 0000 0000  ................
-00008800: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-00008810: ab00 0000 0800 0000 1b00 7400 6800 6900  ..........t.h.i.
-00008820: 7200 6400 5f00 7000 6100 7200 7400 7900  r.d._.p.a.r.t.y.
-00008830: 5f00 6c00 6100 6200 6500 6c00 5f00 6100  _.l.a.b.e.l._.a.
-00008840: 7000 7000 6500 6e00 6400 6500 7200 736c  p.p.e.n.d.e.r.sl
-00008850: 7376 7062 6c6f 6200 0002 5e62 706c 6973  svpblob...^bplis
-00008860: 7430 30d8 0102 0304 0506 0708 090a 0b1d  t00.............
-00008870: 4546 470a 5f10 1276 6965 774f 7074 696f  EFG._..viewOptio
-00008880: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00008890: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-000088a0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-000088b0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-000088c0: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
-000088d0: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
-000088e0: 7665 4461 7465 7310 0109 d90c 0d0e 0f10  veDates.........
-000088f0: 1112 1314 151e 2327 2b30 353a 3f58 636f  ......#'+05:?Xco
-00008900: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
-00008910: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
-00008920: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
-00008930: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
-00008940: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
-00008950: 1a1b 0a1d 5569 6e64 6578 5577 6964 7468  ....UindexUwidth
-00008960: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00008970: 6c65 1007 1101 2c09 08d4 1617 1819 1f20  le....,........ 
-00008980: 1d1d 1008 10c8 0808 d416 1718 1909 241d  ..............$.
-00008990: 0a10 b508 09d4 1617 1819 2824 1d1d 1002  ..........($....
-000089a0: 0808 d416 1718 192c 2d1d 0a10 0310 6108  .......,-.....a.
-000089b0: 09d4 1617 1819 3132 0a1d 1005 1064 0908  ......12.....d..
-000089c0: d416 1718 1936 370a 0a10 0410 7309 09d4  .....67.....s...
-000089d0: 1617 1819 3b3c 0a1d 1006 104b 0908 d416  ....;<.....K....
-000089e0: 1718 1940 410a 0a10 0011 01a6 0909 0823  ...@A..........#
-000089f0: 4028 0000 0000 0000 546e 616d 6523 4030  @(......Tname#@0
-00008a00: 0000 0000 0000 0900 0800 1900 2e00 4000  ..............@.
-00008a10: 4800 5c00 6500 7000 7900 8c00 8e00 8f00  H.\.e.p.y.......
-00008a20: a200 ab00 ba00 c700 d300 d800 de00 e300  ................
-00008a30: eb00 f000 f900 ff01 0501 0f01 1701 1901  ................
-00008a40: 1c01 1d01 1e01 2701 2901 2b01 2c01 2d01  ......'.).+.,.-.
-00008a50: 3601 3801 3901 3a01 4301 4501 4601 4701  6.8.9.:.C.E.F.G.
-00008a60: 5001 5201 5401 5501 5601 5f01 6101 6301  P.R.T.U.V._.a.c.
-00008a70: 6401 6501 6e01 7001 7201 7301 7401 7d01  d.e.n.p.r.s.t.}.
-00008a80: 7f01 8101 8201 8301 8c01 8e01 9101 9201  ................
-00008a90: 9301 9401 9d01 a201 ab00 0000 0000 0002  ................
-00008aa0: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
-00008ab0: 0000 0000 0000 0001 ac00 0000 0900 0000  ................
-00008ac0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
-00008ad0: 7600 6900 7300 6500 646c 7376 7062 6c6f  v.i.s.e.dlsvpblo
-00008ae0: 6200 0002 5e62 706c 6973 7430 30d8 0102  b...^bplist00...
-00008af0: 0304 0506 0708 090a 0b1d 4546 0a48 5f10  ..........EF.H_.
-00008b00: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00008b10: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00008b20: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00008b30: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00008b40: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00008b50: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00008b60: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
-00008b70: 6510 0109 d90c 0d0e 0f10 1112 1314 151e  e...............
-00008b80: 2328 2d32 373c 4158 636f 6d6d 656e 7473  #(-27<AXcomments
-00008b90: 5e64 6174 654c 6173 744f 7065 6e65 645b  ^dateLastOpened[
-00008ba0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-00008bb0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-00008bc0: 696f 6e54 6e61 6d65 5c64 6174 654d 6f64  ionTname\dateMod
-00008bd0: 6966 6965 64d4 1617 1819 1a0a 1c1d 5569  ified.........Ui
-00008be0: 6e64 6578 5961 7363 656e 6469 6e67 5577  ndexYascendingUw
-00008bf0: 6964 7468 5776 6973 6962 6c65 1007 0911  idthWvisible....
-00008c00: 012c 08d4 1617 1819 1f1d 211d 1008 0810  .,........!.....
-00008c10: c808 d416 1718 1924 1d26 1d10 0208 10b5  .......$.&......
-00008c20: 08d4 1617 1819 291d 2b0a 1003 0810 6109  ......).+.....a.
-00008c30: d416 1718 192e 0a30 1d10 0509 1064 08d4  .......0.....d..
-00008c40: 1617 1819 330a 350a 1004 0910 7309 d416  ....3.5.....s...
-00008c50: 1718 1938 0a3a 1d10 0609 104b 08d4 1617  ...8.:.....K....
-00008c60: 1819 3d0a 3f0a 1000 0911 018f 09d4 1617  ..=.?...........
-00008c70: 1819 091d 260a 0809 0823 4028 0000 0000  ....&....#@(....
-00008c80: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
-00008c90: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-00008ca0: 7000 8300 8c00 8e00 8f00 a200 ab00 ba00  p...............
-00008cb0: c600 cb00 d100 d600 de00 e300 f000 f900  ................
-00008cc0: ff01 0901 0f01 1701 1901 1a01 1d01 1e01  ................
-00008cd0: 2701 2901 2a01 2c01 2d01 3601 3801 3901  '.).*.,.-.6.8.9.
-00008ce0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
-00008cf0: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
-00008d00: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
-00008d10: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
-00008d20: a201 a300 0000 0000 0002 0100 0000 0000  ................
-00008d30: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
-00008d40: 0001 ac01 3401 3601 3701 3c01 4501 4601  ....4.6.7.<.E.F.
-00008d50: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
-00008d60: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
-00008d70: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
-00008d80: bb01 c400 0000 0000 0002 0100 0000 0000  ................
-00008d90: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
-00008da0: 0001 c5c4 6108 09d4 0f10 1112 2b2c 0c0c  ....a.......+,..
-00008db0: 546b 696e 6410 7309 09d4 0f10 1112 3031  Tkind.s.......01
-00008dc0: 0c1a 556c 6162 656c 1064 0908 d40f 1011  ..Ulabel.d......
-00008dd0: 1235 360c 1a57 7665 7273 696f 6e10 4b09  .56..Wversion.K.
-00008de0: 08d4 0f10 1112 3a3b 0c1a 5863 6f6d 6d65  ......:;..Xcomme
-00008df0: 6e74 7311 012c 0908 d40f 1011 123f 401a  nts..,.......?@.
-00008e00: 1a5e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00008e10: 10c8 0808 d40f 1011 1244 1e1a 1a59 6461  .........D...Yda
-00008e20: 7465 4164 6465 6408 0808 2300 0000 0000  teAdded...#.....
-00008e30: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00008e40: 6509 1001 0008 001d 0026 0038 0040 0054  e........&.8.@.T
-00008e50: 0066 006f 0081 008c 009f 00b4 00bd 00be  .f.o............
-00008e60: 00ca 00d3 00de 00e4 00ee 00f6 00fb 00fe  ................
-00008e70: 00ff 0100 0109 0112 0114 0115 0116 011f  ................
-00008e80: 012c 012e 012f 0130 0139 0145 0146 0147  .,.../.0.9.E.F.G
-00008e90: 0150 0155 0157 0158 0159 0162 0167 0169  .P.U.W.X.Y.b.g.i
-00008ea0: 016a 016b 0174 017a 017c 017d 017e 0187  .j.k.t.z.|.}.~..
-00008eb0: 018f 0191 0192 0193 019c 01a5 01a8 01a9  ................
-00008ec0: 01aa 01b3 01c2 01c4 01c5 01c6 01cf 01d9  ................
-00008ed0: 01da 01db 01dc 01e5 01ee 01f3 01f4 0000  ................
-00008ee0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
-00008ef0: 0000 0000 0000 0000 0000 0000 01f6 7430  ..............t0
-00008f00: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00008f10: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00008f20: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00008f30: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00008f40: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00008f50: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00008f60: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00008f70: 6172 0808 0908 095f 1018 7b7b 3635 372c  ar....._..{{657,
-00008f80: 2032 3730 7d2c 207b 3938 392c 2034 3336   270}, {989, 436
-00008f90: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00008fa0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-00008fb0: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00008fc0: 009a 0000 0000 0000 0000 0000 0000 0000  ................
-00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000070e0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+000070f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00007100: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00007110: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00007120: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00007130: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00007140: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00007150: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00007160: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+00007170: 7b33 322c 2031 3233 7d2c 207b 3132 3033  {32, 123}, {1203
+00007180: 2c20 3735 347d 7d09 0817 2531 3d49 606d  , 754}}...%1=I`m
+00007190: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+000071a0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+000071b0: 0000 0000 0000 9a00 0000 1b00 7400 6800  ............t.h.
+000071c0: 6900 7200 6400 5f00 7000 6100 7200 7400  i.r.d._.p.a.r.t.
+000071d0: 7900 5f00 6c00 6100 6200 6500 6c00 5f00  y._.l.a.b.e.l._.
+000071e0: 6100 7000 7000 6500 6e00 6400 6500 7200  a.p.p.e.n.d.e.r.
+000071f0: 736c 6731 5363 6f6d 7000 0000 0000 021a  slg1Scomp.......
+00007200: b600 0000 1b00 7400 6800 6900 7200 6400  ......t.h.i.r.d.
+00007210: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
+00007220: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
+00007230: 6500 6e00 6400 6500 7200 736c 7376 4362  e.n.d.e.r.slsvCb
+00007240: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
+00007250: 0102 0304 0506 0708 090a 0b16 4647 480a  ............FGH.
+00007260: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00007270: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+00007280: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00007290: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+000072a0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+000072b0: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+000072c0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+000072d0: 7465 7310 0109 ab0c 151a 1f23 282d 3237  tes........#(-27
+000072e0: 3c41 d40d 0e0f 100a 120a 1457 7669 7369  <A.........Wvisi
+000072f0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+00007300: 696e 675a 6964 656e 7469 6669 6572 0911  ingZidentifier..
+00007310: 01a6 0954 6e61 6d65 d40d 0e0f 1016 1716  ...Tname........
+00007320: 1908 1023 0858 7562 6971 7569 7479 d40d  ...#.Xubiquity..
+00007330: 0e0f 100a 1c16 1e09 10b5 085c 6461 7465  ...........\date
+00007340: 4d6f 6469 6669 6564 d40d 0e0f 1016 1c16  Modified........
+00007350: 2208 085b 6461 7465 4372 6561 7465 64d4  "..[dateCreated.
+00007360: 0d0e 0f10 0a25 1627 0910 6108 5473 697a  .....%.'..a.Tsiz
+00007370: 65d4 0d0e 0f10 0a2a 0a2c 0910 7309 546b  e......*.,..s.Tk
+00007380: 696e 64d4 0d0e 0f10 162f 0a31 0810 6409  ind....../.1..d.
+00007390: 556c 6162 656c d40d 0e0f 1016 340a 3608  Ulabel......4.6.
+000073a0: 104b 0957 7665 7273 696f 6ed4 0d0e 0f10  .K.Wversion.....
+000073b0: 1639 0a3b 0811 012c 0958 636f 6d6d 656e  .9.;...,.Xcommen
+000073c0: 7473 d40d 0e0f 1016 3e16 4008 10c8 085e  ts......>.@....^
+000073d0: 6461 7465 4c61 7374 4f70 656e 6564 d40d  dateLastOpened..
+000073e0: 0e0f 1016 1c16 4408 0859 6461 7465 4164  ......D..YdateAd
+000073f0: 6465 6408 2340 2800 0000 0000 0054 6e61  ded.#@(......Tna
+00007400: 6d65 2340 3000 0000 0000 0009 0008 0019  me#@0...........
+00007410: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
+00007420: 008e 008f 009b 00a4 00ac 00b2 00bc 00c7  ................
+00007430: 00c8 00cb 00cc 00d1 00da 00db 00dd 00de  ................
+00007440: 00e7 00f0 00f1 00f3 00f4 0101 010a 010b  ................
+00007450: 010c 0118 0121 0122 0124 0125 012a 0133  .....!.".$.%.*.3
+00007460: 0134 0136 0137 013c 0145 0146 0148 0149  .4.6.7.<.E.F.H.I
+00007470: 014f 0158 0159 015b 015c 0164 016d 016e  .O.X.Y.[.\.d.m.n
+00007480: 0171 0172 017b 0184 0185 0187 0188 0197  .q.r.{..........
+00007490: 01a0 01a1 01a2 01ac 01ad 01b6 01bb 01c4  ................
+000074a0: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+000074b0: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+000074c0: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+000074d0: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+000074e0: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+000074f0: 006e 0064 0065 0072 0073 6c73 7670 626c  .n.d.e.r.slsvpbl
+00007500: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
+00007510: 0203 0405 0607 0809 0a0b 1d45 4647 0a5f  ...........EFG._
+00007520: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00007530: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+00007540: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00007550: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00007560: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+00007570: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+00007580: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00007590: 6573 1001 09d9 0c0d 0e0f 1011 1213 1415  es..............
+000075a0: 1e23 272b 3035 3a3f 5863 6f6d 6d65 6e74  .#'+05:?Xcomment
+000075b0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+000075c0: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
+000075d0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+000075e0: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+000075f0: 6e54 6e61 6d65 d416 1718 191a 1b0a 1d55  nTname.........U
+00007600: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
+00007610: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
+00007620: 012c 0908 d416 1718 191f 201d 1d10 0810  .,........ .....
+00007630: c808 08d4 1617 1819 0924 1d0a 10b5 0809  .........$......
+00007640: d416 1718 1928 241d 1d10 0208 08d4 1617  .....($.........
+00007650: 1819 2c2d 1d0a 1003 1061 0809 d416 1718  ..,-.....a......
+00007660: 1931 320a 1d10 0510 6409 08d4 1617 1819  .12.....d.......
+00007670: 3637 0a0a 1004 1073 0909 d416 1718 193b  67.....s.......;
+00007680: 3c0a 1d10 0610 4b09 08d4 1617 1819 4041  <.....K.......@A
+00007690: 0a0a 1000 1101 a609 0908 2340 2800 0000  ..........#@(...
+000076a0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
+000076b0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+000076c0: 0070 0079 008c 008e 008f 00a2 00ab 00ba  .p.y............
+000076d0: 00c7 00d3 00d8 00de 00e3 00eb 00f0 00f9  ................
+000076e0: 00ff 0105 010f 0117 0119 011c 011d 011e  ................
+000076f0: 0127 0129 012b 012c 012d 0136 0138 0139  .'.).+.,.-.6.8.9
+00007700: 013a 0143 0145 0146 0147 0150 0152 0154  .:.C.E.F.G.P.R.T
+00007710: 0155 0156 015f 0161 0163 0164 0165 016e  .U.V._.a.c.d.e.n
+00007720: 0170 0172 0173 0174 017d 017f 0181 0182  .p.r.s.t.}......
+00007730: 0183 018c 018e 0191 0192 0193 0194 019d  ................
+00007740: 01a2 01ab 0000 0000 0000 0201 0000 0000  ................
+00007750: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
+00007760: 0000 01ac 0000 001b 0074 0068 0069 0072  .........t.h.i.r
+00007770: 0064 005f 0070 0061 0072 0074 0079 005f  .d._.p.a.r.t.y._
+00007780: 006c 0061 0062 0065 006c 005f 0061 0070  .l.a.b.e.l._.a.p
+00007790: 0070 0065 006e 0064 0065 0072 0073 6d6f  .p.e.n.d.e.r.smo
+000077a0: 4444 626c 6f62 0000 0008 801f e384 2efe  DDblob..........
+000077b0: c441 0000 001b 0074 0068 0069 0072 0064  .A.....t.h.i.r.d
+000077c0: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
+000077d0: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
+000077e0: 0065 006e 0064 0065 0072 0073 6d6f 6444  .e.n.d.e.r.smodD
+000077f0: 626c 6f62 0000 0008 4c89 caff 10fc c441  blob....L......A
+00007800: 0000 001b 0074 0068 0069 0072 0064 005f  .....t.h.i.r.d._
+00007810: 0070 0061 0072 0074 0079 005f 006c 0061  .p.a.r.t.y._.l.a
+00007820: 0062 0065 006c 005f 0061 0070 0070 0065  .b.e.l._.a.p.p.e
+00007830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
+00007840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
+00007850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
+00007860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
+00007870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
+00007880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
+00007890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
+000078a0: 0000 00c6 6270 6c69 7374 3030 d701 0203  ....bplist00....
+000078b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+000078c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+000078d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+000078e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+000078f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00007900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00007910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00007920: 0809 5f10 157b 7b30 2c20 307d 2c20 7b31  .._..{{0, 0}, {1
+00007930: 3434 302c 2038 3737 7d7d 0908 1725 313d  440, 877}}...%1=
+00007940: 4960 6d79 7a7b 7c7d 7e96 0000 0000 0000  I`myz{|}~.......
+00007950: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00007960: 0000 0000 0000 0000 0097 0000 0002 0075  ...............u
+00007970: 0069 6473 636c 626f 6f6c 0100 0000 0200  .idsclbool......
+00007980: 7500 696c 6731 5363 6f6d 7000 0000 0000  u.ilg1Scomp.....
+00007990: 0bf8 5c00 0000 0200 7500 696c 7376 4362  ..\.....u.ilsvCb
+000079a0: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
+000079b0: 0102 0304 0506 0708 090a 0b16 4647 0a49  ............FG.I
+000079c0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+000079d0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+000079e0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+000079f0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00007a00: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+00007a10: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+00007a20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00007a30: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
+00007a40: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 110a  ..#(-27<A.......
+00007a50: 130a 5a69 6465 6e74 6966 6965 7259 6173  ..ZidentifierYas
+00007a60: 6365 6e64 696e 6755 7769 6474 6857 7669  cendingUwidthWvi
+00007a70: 7369 626c 6554 6e61 6d65 0911 0251 09d4  sibleTname...Q..
+00007a80: 100f 0e0d 1617 1619 0810 2308 5875 6269  ..........#.Xubi
+00007a90: 7175 6974 79d4 100e 0f0d 0a16 1d1e 0908  quity...........
+00007aa0: 10b5 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
+00007ab0: 100e 0f0d 1616 1d22 0808 5b64 6174 6543  ......."..[dateC
+00007ac0: 7265 6174 6564 d410 0e0f 0d0a 1626 2709  reated.......&'.
+00007ad0: 0810 6154 7369 7a65 d410 0e0f 0d0a 0a2b  ..aTsize.......+
+00007ae0: 2c09 0910 7354 6b69 6e64 d410 0e0f 0d16  ,...sTkind......
+00007af0: 0a30 3108 0910 6455 6c61 6265 6cd4 100e  .01...dUlabel...
+00007b00: 0f0d 160a 3536 0809 104b 5776 6572 7369  ....56...KWversi
+00007b10: 6f6e d410 0e0f 0d16 0a3a 3b08 0911 012c  on.......:;....,
+00007b20: 5863 6f6d 6d65 6e74 73d4 100e 0f0d 1616  Xcomments.......
+00007b30: 3f40 0808 10c8 5e64 6174 654c 6173 744f  ?@....^dateLastO
+00007b40: 7065 6e65 64d4 100f 0e0d 161d 1644 0808  pened........D..
+00007b50: 5964 6174 6541 6464 6564 0823 4028 0000  YdateAdded.#@(..
+00007b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
+00007b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00007b80: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
+00007b90: 00d3 00d4 00d7 00d8 00e1 00e2 00e4 00e5  ................
+00007ba0: 00ee 00f7 00f8 00f9 00fb 0108 0111 0112  ................
+00007bb0: 0113 011f 0128 0129 012a 012c 0131 013a  .....(.).*.,.1.:
+00007bc0: 013b 013c 013e 0143 014c 014d 014e 0150  .;.<.>.C.L.M.N.P
+00007bd0: 0156 015f 0160 0161 0163 016b 0174 0175  .V._.`.a.c.k.t.u
+00007be0: 0176 0179 0182 018b 018c 018d 018f 019e  .v.y............
+00007bf0: 01a7 01a8 01a9 01b3 01b4 01bd 01c2 01c3  ................
+00007c00: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+00007c10: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+00007c20: 0000 0002 0075 0069 6c73 7670 626c 6f62  .....u.ilsvpblob
+00007c30: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
+00007c40: 0405 0607 0809 0a0b 1d46 470a 2458 6963  .........FG.$Xic
+00007c50: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00007c60: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00007c70: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00007c80: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+00007c90: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+00007ca0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+00007cb0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00007cc0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
+00007cd0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
+00007ce0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+00007cf0: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+00007d00: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00007d10: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00007d20: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
+00007d30: 1a0a 1c1d 5569 6e64 6578 5961 7363 656e  ....UindexYascen
+00007d40: 6469 6e67 5577 6964 7468 5776 6973 6962  dingUwidthWvisib
+00007d50: 6c65 1007 0911 012c 08d4 1617 1819 1f1d  le.....,........
+00007d60: 211d 1008 0810 c808 d416 1718 1924 1d26  !............$.&
+00007d70: 0a10 0108 10b5 09d4 1617 1819 291d 261d  ............).&.
+00007d80: 1002 0808 d416 1718 192d 1d2f 0a10 0308  .........-./....
+00007d90: 1061 09d4 1617 1819 320a 341d 1005 0910  .a......2.4.....
+00007da0: 6408 d416 1718 1937 0a39 0a10 0409 1073  d......7.9.....s
+00007db0: 09d4 1617 1819 3c0a 3e1d 1006 0910 4b08  ......<.>.....K.
+00007dc0: d419 1718 160a 0a43 4409 0911 0251 1000  .......CD....Q..
+00007dd0: 0823 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
+00007de0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+00007df0: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
+00007e00: 00da 00df 00e5 00ea 00f2 00f7 0100 0106  ................
+00007e10: 0110 0116 011e 0120 0121 0124 0125 012e  ....... .!.$.%..
+00007e20: 0130 0131 0133 0134 013d 013f 0140 0142  .0.1.3.4.=.?.@.B
+00007e30: 0143 014c 014e 014f 0150 0159 015b 015c  .C.L.N.O.P.Y.[.\
+00007e40: 015e 015f 0168 016a 016b 016d 016e 0177  .^._.h.j.k.m.n.w
+00007e50: 0179 017a 017c 017d 0186 0188 0189 018b  .y.z.|.}........
+00007e60: 018c 0195 0196 0197 019a 019c 019d 01a6  ................
+00007e70: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
+00007e80: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+00007e90: 01ac 0000 0002 0075 0069 6d6f 4444 626c  .......u.imoDDbl
+00007ea0: 6f62 0000 0008 6da9 747c 5e01 c541 0000  ob....m.t|^..A..
+00007eb0: 0002 0075 0069 6d6f 6444 626c 6f62 0000  ...u.imodDblob..
+00007ec0: 0008 6da9 747c 5e01 c541 0000 0002 0075  ..m.t|^..A.....u
+00007ed0: 0069 7068 3153 636f 6d70 0000 0000 000f  .iph1Scomp......
+00007ee0: 1000 bc01 bd01 c601 cf01 d400 0000 0000  ................
+00007ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
+00007f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
+00007f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+00007f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+00007f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
+00007f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
+00007f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00007f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00007f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
+00007f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
+00007f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
+00007fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00007fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
+00007fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00007fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00007fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
+00008010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+00008020: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
+00008030: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00008040: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00008050: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00008060: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00008070: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00008080: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00008090: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+000080a0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+000080b0: 0809 5f10 197b 7b32 3630 2c20 3136 327d  .._..{{260, 162}
+000080c0: 2c20 7b31 3138 302c 2035 3538 7d7d 0908  , {1180, 558}}..
+000080d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+000080e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+000080f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
+00008100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+00008110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
+00008120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
+00008130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
+00008140: 6731 5363 6f6d 7000 0000 0000 05cf 0200  g1Scomp.........
+00008150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
+00008160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
+00008170: 6c6f 6200 0002 9762 706c 6973 7430 30d8  lob....bplist00.
+00008180: 0102 0304 0506 0708 090a 0b19 494a 0a4c  ............IJ.L
+00008190: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000081a0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+000081b0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+000081c0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+000081d0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+000081e0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+000081f0: 6174 6976 6544 6174 6573 5869 636f 6e53  ativeDatesXiconS
+00008200: 697a 6510 0109 ab0c 151d 2226 2b30 353a  ize......."&+05:
+00008210: 3f44 d40d 0e0f 100a 0a13 1457 7669 7369  ?D.........Wvisi
+00008220: 626c 6559 6173 6365 6e64 696e 6755 7769  bleYascendingUwi
+00008230: 6474 685a 6964 656e 7469 6669 6572 0909  dthZidentifier..
+00008240: 1101 8f54 6e61 6d65 d416 1718 1019 1a19  ...Tname........
+00008250: 1c57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+00008260: 6173 6365 6e64 696e 6708 1023 0858 7562  ascending..#.Xub
+00008270: 6971 7569 7479 d40d 0e0f 100a 1920 2109  iquity....... !.
+00008280: 0810 b55c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00008290: d40d 0e0f 1019 1920 2508 085b 6461 7465  ....... %..[date
+000082a0: 4372 6561 7465 64d4 0d0e 0f10 0a19 292a  Created.......)*
+000082b0: 0908 1061 5473 697a 65d4 0d0e 0f10 0a0a  ...aTsize.......
+000082c0: 2e2f 0909 1073 546b 696e 64d4 0d0e 0f10  ./...sTkind.....
+000082d0: 190a 3334 0809 1064 556c 6162 656c d40d  ..34...dUlabel..
+000082e0: 0e0f 1019 0a38 3908 0910 4b57 7665 7273  .....89...KWvers
+000082f0: 696f 6ed4 0d0e 0f10 190a 3d3e 0809 1101  ion.......=>....
+00008300: 2c58 636f 6d6d 656e 7473 d40d 0e0f 1019  ,Xcomments......
+00008310: 1942 4308 0810 c85e 6461 7465 4c61 7374  .BC....^dateLast
+00008320: 4f70 656e 6564 d416 1718 1019 2019 4708  Opened...... .G.
+00008330: 0859 6461 7465 4164 6465 6408 2340 2800  .YdateAdded.#@(.
+00008340: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
+00008350: 0000 0000 0008 0019 002e 0040 0048 005c  ...........@.H.\
+00008360: 0065 0070 0083 008c 008e 008f 009b 00a4  .e.p............
+00008370: 00ac 00b6 00bc 00c7 00c8 00c9 00cc 00d1  ................
+00008380: 00da 00e2 00e8 00f2 00f3 00f5 00f6 00ff  ................
+00008390: 0108 0109 010a 010c 0119 0122 0123 0124  ...........".#.$
+000083a0: 0130 0139 013a 013b 013d 0142 014b 014c  .0.9.:.;.=.B.K.L
+000083b0: 014d 014f 0154 015d 015e 015f 0161 0167  .M.O.T.].^._.a.g
+000083c0: 0170 0171 0172 0174 017c 0185 0186 0187  .p.q.r.t.|......
+000083d0: 018a 0193 019c 019d 019e 01a0 01af 01b8  ................
+000083e0: 01b9 01ba 01c4 01c5 01ce 01d3 01d4 0000  ................
+000083f0: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
+00008400: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
+00008410: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+00008420: 0076 0069 0073 0065 0064 6c73 7670 626c  .v.i.s.e.dlsvpbl
+00008430: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
+00008440: 0203 0405 0607 0809 0a0b 1d45 460a 485f  ...........EF.H_
+00008450: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00008460: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
+00008470: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+00008480: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+00008490: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+000084a0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
+000084b0: 7469 7665 4461 7465 7358 6963 6f6e 5369  tiveDatesXiconSi
+000084c0: 7a65 1001 09d9 0c0d 0e0f 1011 1213 1415  ze..............
+000084d0: 1e23 282d 3237 3c41 5863 6f6d 6d65 6e74  .#(-27<AXcomment
+000084e0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+000084f0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+00008500: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+00008510: 7369 6f6e 546e 616d 655c 6461 7465 4d6f  sionTname\dateMo
+00008520: 6469 6669 6564 d416 1718 191a 0a1c 1d55  dified.........U
+00008530: 696e 6465 7859 6173 6365 6e64 696e 6755  indexYascendingU
+00008540: 7769 6474 6857 7669 7369 626c 6510 0709  widthWvisible...
+00008550: 1101 2c08 d416 1718 191f 1d21 1d10 0808  ..,........!....
+00008560: 10c8 08d4 1617 1819 241d 261d 1002 0810  ........$.&.....
+00008570: b508 d416 1718 1929 1d2b 0a10 0308 1061  .......).+.....a
+00008580: 09d4 1617 1819 2e0a 301d 1005 0910 6408  ........0.....d.
+00008590: d416 1718 1933 0a35 0a10 0409 1073 09d4  .....3.5.....s..
+000085a0: 1617 1819 380a 3a1d 1006 0910 4b08 d416  ....8.:.....K...
+000085b0: 1718 193d 0a3f 0a10 0009 1101 8f09 d416  ...=.?..........
+000085c0: 1718 1909 1d26 0a08 0908 2340 2800 0000  .....&....#@(...
+000085d0: 0000 0054 6e61 6d65 0923 4030 0000 0000  ...Tname.#@0....
+000085e0: 0000 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+000085f0: 0070 0083 008c 008e 008f 00a2 00ab 00ba  .p..............
+00008600: 00c6 00cb 00d1 00d6 00de 00e3 00f0 00f9  ................
+00008610: 00ff 0109 010f 0117 0119 011a 011d 011e  ................
+00008620: 0127 0129 012a 012c 012d 0136 0138 0139  .'.).*.,.-.6.8.9
+00008630: 013b 013c 0145 0147 0148 014a 014b 0154  .;.<.E.G.H.J.K.T
+00008640: 0156 0157 0159 015a 0163 0165 0166 0168  .V.W.Y.Z.c.e.f.h
+00008650: 0169 0172 0174 0175 0177 0178 0181 0183  .i.r.t.u.w.x....
+00008660: 0184 0187 0188 0191 0192 0193 0194 019d  ................
+00008670: 01a2 01a3 0000 0000 0000 0201 0000 0000  ................
+00008680: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
+00008690: 0000 01ac 0000 000c 0075 006e 0073 0075  .........u.n.s.u
+000086a0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
+000086b0: 6d6f 4444 626c 6f62 0000 0008 0e97 7a42  moDDblob......zB
+000086c0: c500 c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
+000086d0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
+000086e0: 6d6f 6444 626c 6f62 0000 0008 785b 2585  modDblob....x[%.
+000086f0: fefd c441 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
+00008700: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
+00008710: 7068 3153 636f 6d70 0000 0000 0007 4000  ph1Scomp......@.
+00008720: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
+00008730: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
+00008740: 6c6f 6e67 0000 0001 0000 0005 0075 0074  long.........u.t
+00008750: 0069 006c 0073 6277 7370 626c 6f62 0000  .i.l.sbwspblob..
+00008760: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00008770: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+00008780: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00008790: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+000087a0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+000087b0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+000087c0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+000087d0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+000087e0: 5f10 187b 7b33 3532 2c20 3234 377d 2c20  _..{{352, 247}, 
+000087f0: 7b39 3839 2c20 3433 367d 7d09 0817 2531  {989, 436}}...%1
+00008800: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
+00008810: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
+00008820: 0000 0000 0000 0000 0000 9a70 0070 0065  ...........p.p.e
+00008830: 006e 0064 0065 0072 0073 7068 3153 636f  .n.d.e.r.sph1Sco
+00008840: 6d70 0000 0000 0002 b000 0000 001b 0074  mp.............t
+00008850: 0068 0069 0072 0064 005f 0070 0061 0072  .h.i.r.d._.p.a.r
+00008860: 0074 0079 005f 006c 0061 0062 0065 006c  .t.y._.l.a.b.e.l
+00008870: 005f 0061 0070 0070 0065 006e 0064 0065  ._.a.p.p.e.n.d.e
+00008880: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
+00008890: 0000 0002 0075 0069 6277 7370 626c 6f62  .....u.ibwspblob
+000088a0: 0000 00c6 6270 6c69 7374 3030 d701 0203  ....bplist00....
+000088b0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+000088c0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+000088d0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+000088e0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+000088f0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00008900: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00008910: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00008920: 0809 5f10 157b 7b30 2c20 307d 2c20 7b31  .._..{{0, 0}, {1
+00008930: 3434 302c 2038 3737 7d7d 0908 1725 313d  440, 877}}...%1=
+00008940: 4960 6d79 7a7b 7c7d 7e96 0000 0000 0000  I`myz{|}~.......
+00008950: 0101 0000 0000 0000 000f 0000 0000 0000  ................
+00008960: 0000 0000 0000 0000 0097 0000 0002 0075  ...............u
+00008970: 0069 6473 636c 626f 6f6c 0100 0000 0200  .idsclbool......
+00008980: 7500 696c 6731 5363 6f6d 7000 0000 0000  u.ilg1Scomp.....
+00008990: 0bf8 5c00 0000 0200 7500 696c 7376 4362  ..\.....u.ilsvCb
+000089a0: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
+000089b0: 0102 0304 0506 0708 090a 0b16 4647 0a49  ............FG.I
+000089c0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+000089d0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+000089e0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+000089f0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00008a00: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+00008a10: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+00008a20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00008a30: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
+00008a40: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 110a  ..#(-27<A.......
+00008a50: 130a 5a69 6465 6e74 6966 6965 7259 6173  ..ZidentifierYas
+00008a60: 6365 6e64 696e 6755 7769 6474 6857 7669  cendingUwidthWvi
+00008a70: 7369 626c 6554 6e61 6d65 0911 0251 09d4  sibleTname...Q..
+00008a80: 100f 0e0d 1617 1619 0810 2308 5875 6269  ..........#.Xubi
+00008a90: 7175 6974 79d4 100e 0f0d 0a16 1d1e 0908  quity...........
+00008aa0: 10b5 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
+00008ab0: 100e 0f0d 1616 1d22 0808 5b64 6174 6543  ......."..[dateC
+00008ac0: 7265 6174 6564 d410 0e0f 0d0a 1626 2709  reated.......&'.
+00008ad0: 0810 6154 7369 7a65 d410 0e0f 0d0a 0a2b  ..aTsize.......+
+00008ae0: 2c09 0910 7354 6b69 6e64 d410 0e0f 0d16  ,...sTkind......
+00008af0: 0a30 3108 0910 6455 6c61 6265 6cd4 100e  .01...dUlabel...
+00008b00: 0f0d 160a 3536 0809 104b 5776 6572 7369  ....56...KWversi
+00008b10: 6f6e d410 0e0f 0d16 0a3a 3b08 0911 012c  on.......:;....,
+00008b20: 5863 6f6d 6d65 6e74 73d4 100e 0f0d 1616  Xcomments.......
+00008b30: 3f40 0808 10c8 5e64 6174 654c 6173 744f  ?@....^dateLastO
+00008b40: 7065 6e65 64d4 100f 0e0d 161d 1644 0808  pened........D..
+00008b50: 5964 6174 6541 6464 6564 0823 4028 0000  YdateAdded.#@(..
+00008b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
+00008b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00008b80: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
+00008b90: 00d3 00d4 00d7 00d8 00e1 00e2 00e4 00e5  ................
+00008ba0: 00ee 00f7 00f8 00f9 00fb 0108 0111 0112  ................
+00008bb0: 0113 011f 0128 0129 012a 012c 0131 013a  .....(.).*.,.1.:
+00008bc0: 013b 013c 013e 0143 014c 014d 014e 0150  .;.<.>.C.L.M.N.P
+00008bd0: 0156 015f 0160 0161 0163 016b 0174 0175  .V._.`.a.c.k.t.u
+00008be0: 0176 0179 0182 018b 018c 018d 018f 019e  .v.y............
+00008bf0: 01a7 01a8 01a9 01b3 01b4 01bd 01c2 01c3  ................
+00008c00: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+00008c10: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+00008c20: 0000 0002 0075 0069 6c73 7670 626c 6f62  .....u.ilsvpblob
+00008c30: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
+00008c40: 0405 0607 0809 0a0b 1d46 470a 2458 6963  .........FG.$Xic
+00008c50: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00008c60: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00008c70: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00008c80: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+00008c90: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+00008ca0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+00008cb0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00008cc0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
+00008cd0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
+00008ce0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+00008cf0: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+00008d00: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00008d10: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00008d20: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
+00008d30: 1a0a 1c1d 5569 6e64 6578 5961 7363 656e  ....UindexYascen
+00008d40: 6469 6e67 5577 6964 7468 5776 6973 6962  dingUwidthWvisib
+00008d50: 6c65 1007 0911 012c 08d4 1617 1819 1f1d  le.....,........
+00008d60: 211d 1008 0810 c808 d416 1718 1924 1d26  !............$.&
+00008d70: 0a10 0108 10b5 09d4 1617 1819 291d 261d  ............).&.
+00008d80: 1002 0808 d416 1718 192d 1d2f 0a10 0308  .........-./....
+00008d90: 1061 09d4 1617 1819 320a 341d 1005 0910  .a......2.4.....
+00008da0: 6408 d416 1718 1937 0a39 0a10 0409 1073  d......7.9.....s
+00008db0: 09d4 1617 1819 3c0a 3e1d 1006 0910 4b08  ......<.>.....K.
+00008dc0: d419 1718 160a 0a43 4409 0911 0251 1000  .......CD....Q..
+00008dd0: 0823 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
+00008de0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+00008df0: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
+00008e00: 00da 00df 00e5 00ea 00f2 00f7 0100 0106  ................
+00008e10: 0110 0116 011e 0120 0121 0124 0125 012e  ....... .!.$.%..
+00008e20: 0130 0131 0133 0134 013d 013f 0140 0142  .0.1.3.4.=.?.@.B
+00008e30: 0143 014c 014e 014f 0150 0159 015b 015c  .C.L.N.O.P.Y.[.\
+00008e40: 015e 015f 0168 016a 016b 016d 016e 0177  .^._.h.j.k.m.n.w
+00008e50: 0179 017a 017c 017d 0186 0188 0189 018b  .y.z.|.}........
+00008e60: 018c 0195 0196 0197 019a 019c 019d 01a6  ................
+00008e70: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
+00008e80: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+00008e90: 01ac 0000 0002 0075 0069 6d6f 4444 626c  .......u.imoDDbl
+00008ea0: 6f62 0000 0008 6da9 747c 5e01 c541 0000  ob....m.t|^..A..
+00008eb0: 0002 0075 0069 6d6f 6444 626c 6f62 0000  ...u.imodDblob..
+00008ec0: 0008 6da9 747c 5e01 c541 0000 0002 0075  ..m.t|^..A.....u
+00008ed0: 0069 7068 3153 636f 6d70 0000 0000 000f  .iph1Scomp......
+00008ee0: 1000 bc01 bd01 c601 cf01 d400 0000 0000  ................
+00008ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
+00008f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
+00008f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+00008f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+00008f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
+00008f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
+00008f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00008f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00008f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
+00008f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
+00008f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
+00008fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00008fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
+00008fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00008fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00008fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00009000: 0000 0000                                ....
+00009000: 0000 0000 0000 0002 0000 0007 0000 0004  ................
+00009010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
+00009020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
+00009030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
+00009040: 0000 025d 6270 6c69 7374 3030 d801 0203  ...]bplist00....
+00009050: 0405 0607 0809 0a0b 1a46 470a 2758 6963  .........FG.'Xic
+00009060: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00009070: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00009080: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00009090: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+000090a0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000090b0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+000090c0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000090d0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
+000090e0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
+000090f0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+00009100: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+00009110: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00009120: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00009130: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
+00009140: 1a1b 0a1d 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
+00009150: 7468 5961 7363 656e 6469 6e67 5569 6e64  thYascendingUind
+00009160: 6578 0811 012c 0910 07d4 1617 1819 1a20  ex...,......... 
+00009170: 1a22 0810 c808 1008 d416 1718 190a 251a  ."............%.
+00009180: 2709 10b5 0810 01d4 1617 1819 1a25 1a2b  '............%.+
+00009190: 0808 1002 d416 1718 190a 2e1a 3009 1061  ............0..a
+000091a0: 0810 03d4 1617 1819 1a33 0a35 0810 6409  .........3.5..d.
+000091b0: 1005 d416 1718 190a 380a 3a09 1073 0910  ........8.:..s..
+000091c0: 04d4 1617 1819 1a3d 0a3f 0810 4b09 1006  .......=.?..K...
+000091d0: d416 1718 190a 420a 4409 10f0 0910 0008  ......B.D.......
+000091e0: 2340 2800 0000 0000 0054 6e61 6d65 0900  #@(......Tname..
+000091f0: 0800 1900 2200 3400 3c00 5000 5900 6400  ....".4.<.P.Y.d.
+00009200: 7700 8c00 9500 9600 a900 b200 c100 ce00  w...............
+00009210: da00 df00 e500 ea00 f200 f701 0001 0801  ................
+00009220: 0e01 1801 1e01 1f01 2201 2301 2501 2e01  ........".#.%...
+00009230: 2f01 3101 3201 3401 3d01 3e01 4001 4101  /.1.2.4.=.>.@.A.
+00009240: 4301 4c01 4d01 4e01 5001 5901 5a01 5c01  C.L.M.N.P.Y.Z.\.
+00009250: 5d01 5f01 6801 6901 6b01 6c01 6e01 7701  ]._.h.i.k.l.n.w.
+00009260: 7801 7a01 7b01 7d01 8601 8701 8901 8a01  x.z.{.}.........
+00009270: 8c01 9501 9601 9801 9901 9b01 9c01 a501  ................
+00009280: aa00 0000 0000 0002 0100 0000 0000 0000  ................
+00009290: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
+000092a0: ab00 0000 0500 0000 0900 6c00 6100 6200  ..........l.a.b.
+000092b0: 6500 6c00 6c00 6900 6e00 676c 7376 4362  e.l.l.i.n.glsvCb
+000092c0: 6c6f 6200 0002 7962 706c 6973 7430 30d8  lob...ybplist00.
+000092d0: 0102 0304 0506 0708 090a 0b18 4647 0a49  ............FG.I
+000092e0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+000092f0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00009300: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00009310: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00009320: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+00009330: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+00009340: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00009350: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
+00009360: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 110a  ..#(-27<A.......
+00009370: 130a 5a69 6465 6e74 6966 6965 7259 6173  ..ZidentifierYas
+00009380: 6365 6e64 696e 6755 7769 6474 6857 7669  cendingUwidthWvi
+00009390: 7369 626c 6554 6e61 6d65 0911 0251 09d4  sibleTname...Q..
+000093a0: 0d0f 0e10 1617 1818 5875 6269 7175 6974  ........Xubiquit
+000093b0: 7910 2308 08d4 0d0e 0f10 1b18 1d0a 5c64  y.#...........\d
+000093c0: 6174 654d 6f64 6966 6965 6408 10b5 09d4  ateModified.....
+000093d0: 0d0e 0f10 2018 1d18 5b64 6174 6543 7265  .... ...[dateCre
+000093e0: 6174 6564 0808 d40d 0e0f 1024 1826 0a54  ated.......$.&.T
+000093f0: 7369 7a65 0810 6109 d40d 0e0f 1029 0a2b  size..a......).+
+00009400: 0a54 6b69 6e64 0910 7309 d40d 0e0f 102e  .Tkind..s.......
+00009410: 0a30 1855 6c61 6265 6c09 1064 08d4 0d0e  .0.Ulabel..d....
+00009420: 0f10 330a 3518 5776 6572 7369 6f6e 0910  ..3.5.Wversion..
+00009430: 4b08 d40d 0e0f 1038 0a3a 1858 636f 6d6d  K......8.:.Xcomm
+00009440: 656e 7473 0911 012c 08d4 0d0e 0f10 3d18  ents...,......=.
+00009450: 3f18 5e64 6174 654c 6173 744f 7065 6e65  ?.^dateLastOpene
+00009460: 6408 10c8 08d4 0d0f 0e10 421d 1818 5964  d.........B...Yd
+00009470: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
+00009480: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
+00009490: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+000094a0: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
+000094b0: 00d3 00d4 00d7 00d8 00e1 00ea 00ec 00ed  ................
+000094c0: 00ee 00f7 0104 0105 0107 0108 0111 011d  ................
+000094d0: 011e 011f 0128 012d 012e 0130 0131 013a  .....(.-...0.1.:
+000094e0: 013f 0140 0142 0143 014c 0152 0153 0155  .?.@.B.C.L.R.S.U
+000094f0: 0156 015f 0167 0168 016a 016b 0174 017d  .V._.g.h.j.k.t.}
+00009500: 017e 0181 0182 018b 019a 019b 019d 019e  .~..............
+00009510: 01a7 01b1 01b2 01b3 01b4 01bd 01c2 01c3  ................
+00009520: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+00009530: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+00009540: 0000 0006 0000 000d 006f 0075 0074 006c  .........o.u.t.l
+00009550: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00009560: 0073 6c73 7670 626c 6f62 0000 0294 6270  .slsvpblob....bp
+00009570: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
+00009580: 0a0b 0c0d 1c48 4948 4a0c 2958 6963 6f6e  .....HIHJ.)Xicon
+00009590: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
+000095a0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+000095b0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+000095c0: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
+000095d0: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
+000095e0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
+000095f0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+00009600: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
+00009610: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00009620: 6f6e 2340 3000 0000 0000 0009 d90e 0f10  on#@0...........
+00009630: 1112 1314 1516 1720 252a 2e33 383d 4258  ....... %*.38=BX
+00009640: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
+00009650: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
+00009660: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
+00009670: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
+00009680: 5776 6572 7369 6f6e 546e 616d 65d4 1819  WversionTname...
+00009690: 1a1b 1c1d 0c1f 5776 6973 6962 6c65 5577  ......WvisibleUw
+000096a0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
+000096b0: 6e64 6578 0811 012c 0910 07d4 1819 1a1b  ndex...,........
+000096c0: 1c22 1c24 0810 c808 1008 d418 191a 1b0c  .".$............
+000096d0: 271c 2909 10b5 0810 01d4 1819 1a1b 1c27  '.)............'
+000096e0: 1c2d 0808 1002 d418 191a 1b0c 301c 3209  .-..........0.2.
+000096f0: 1061 0810 03d4 1819 1a1b 1c35 0c37 0810  .a.........5.7..
+00009700: 6409 1005 d418 191a 1b0c 3a0c 3c09 1073  d.........:.<..s
+00009710: 0910 04d4 1819 1a1b 1c3f 0c41 0810 4b09  .........?.A..K.
+00009720: 1006 d41b 191a 1843 440c 0c10 0010 f009  .......CD.......
+00009730: 0908 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
+00009740: 0000 0000 546e 616d 6509 0008 001d 0026  ....Tname......&
+00009750: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
+00009760: 00b4 00bd 00be 00d1 00da 00e9 00f6 0102  ................
+00009770: 0107 010d 0112 011a 011f 0128 0130 0136  ...........(.0.6
+00009780: 0140 0146 0147 014a 014b 014d 0156 0157  .@.F.G.J.K.M.V.W
+00009790: 0159 015a 015c 0165 0166 0168 0169 016b  .Y.Z.\.e.f.h.i.k
+000097a0: 0174 0175 0176 0178 0181 0182 0184 0185  .t.u.v.x........
+000097b0: 0187 0190 0191 0193 0194 0196 019f 01a0  ................
+000097c0: 01a2 01a3 01a5 01ae 01af 01b1 01b2 01b4  ................
+000097d0: 01bd 01bf 01c1 01c2 01c3 01c4 01cd 01d6  ................
+000097e0: 01db 0000 0000 0000 0201 0000 0000 0000  ................
+000097f0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
+00009800: 01dc 0000 0007 0000 0013 0070 006f 0073  ...........p.o.s
+00009810: 0065 005f 0063 006f 006e 0066 0069 0067  .e._.c.o.n.f.i.g
+00009820: 0075 0072 0061 0074 0069 006f 006e 0073  .u.r.a.t.i.o.n.s
+00009830: 7653 726e 6c6f 6e67 0000 0001 0000 0008  vSrnlong........
+00009840: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
+00009850: 006f 006c 0073 6c73 7670 626c 6f62 0000  .o.l.slsvpblob..
+00009860: 025d 6270 6c69 7374 3030 d801 0203 0405  .]bplist00......
+00009870: 0607 0809 0a0b 1a46 470a 2758 6963 6f6e  .......FG.'Xicon
+00009880: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
+00009890: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+000098a0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+000098b0: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
+000098c0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
+000098d0: 7469 7665 4461 7465 735f 1012 7669 6577  tiveDates_..view
+000098e0: 4f70 7469 6f6e 7356 6572 7369 6f6e 2340  OptionsVersion#@
+000098f0: 3000 0000 0000 0009 d90c 0d0e 0f10 1112  0...............
+00009900: 1314 151e 2328 2c31 363b 4058 636f 6d6d  ....#(,16;@Xcomm
+00009910: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+00009920: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
+00009930: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+00009940: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+00009950: 7369 6f6e 546e 616d 65d4 1617 1819 1a1b  sionTname.......
+00009960: 0a1d 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+00009970: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
+00009980: 0811 012c 0910 07d4 1617 1819 1a20 1a22  ...,......... ."
+00009990: 0810 c808 1008 d416 1718 190a 251a 2709  ............%.'.
+000099a0: 10b5 0810 01d4 1617 1819 1a25 1a2b 0808  ...........%.+..
+000099b0: 1002 d416 1718 190a 2e1a 3009 1061 0810  ..........0..a..
+000099c0: 03d4 1617 1819 1a33 0a35 0810 6409 1005  .......3.5..d...
+000099d0: d416 1718 190a 380a 3a09 1073 0910 04d4  ......8.:..s....
+000099e0: 1617 1819 1a3d 0a3f 0810 4b09 1006 d416  .....=.?..K.....
+000099f0: 1718 190a 420a 4409 10d0 0910 0008 2340  ....B.D.......#@
+00009a00: 2800 0000 0000 0054 6e61 6d65 0900 0800  (......Tname....
+00009a10: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
+00009a20: 8c00 9500 9600 a900 b200 c100 ce00 da00  ................
+00009a30: df00 e500 ea00 f200 f701 0001 0801 0e01  ................
+00009a40: 1801 1e01 1f01 2201 2301 2501 2e01 2f01  ......".#.%.../.
+00009a50: 3101 3201 3401 3d01 3e01 4001 4101 4301  1.2.4.=.>.@.A.C.
+00009a60: 4c01 4d01 4e01 5001 5901 5a01 5c01 5d01  L.M.N.P.Y.Z.\.].
+00009a70: 5f01 6801 6901 6b01 6c01 6e01 7701 7801  _.h.i.k.l.n.w.x.
+00009a80: 7a01 7b01 7d01 8601 8701 8901 8a01 8c01  z.{.}...........
+00009a90: 9501 9601 9801 9901 9b01 9c01 a501 aa00  ................
+00009aa0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
+00009ab0: 0000 0000 0000 0000 0000 0000 0001 ab00  ................
+00009ac0: 0000 0900 0000 0200 7500 6976 5372 6e6c  ........u.ivSrnl
+00009ad0: 6f6e 6700 0000 0100 0000 0a00 0000 0500  ong.............
+00009ae0: 7500 7400 6900 6c00 7364 7363 6c62 6f6f  u.t.i.l.sdsclboo
+00009af0: 6c00 3108 0910 6455 6c61 6265 6cd4 100e  l.1...dUlabel...
+00009b00: 0f0d 160a 3536 0809 104b 5776 6572 7369  ....56...KWversi
+00009b10: 6f6e d410 0e0f 0d16 0a3a 3b08 0911 012c  on.......:;....,
+00009b20: 5863 6f6d 6d65 6e74 73d4 100e 0f0d 1616  Xcomments.......
+00009b30: 3f40 0808 10c8 5e64 6174 654c 6173 744f  ?@....^dateLastO
+00009b40: 7065 6e65 64d4 100f 0e0d 161d 1644 0808  pened........D..
+00009b50: 5964 6174 6541 6464 6564 0823 4028 0000  YdateAdded.#@(..
+00009b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
+00009b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00009b80: 0095 0096 00a2 00ab 00b6 00c0 00c6 00ce  ................
+00009b90: 00d3 00d4 00d7 00d8 00e1 00e2 00e4 00e5  ................
+00009ba0: 00ee 00f7 00f8 00f9 00fb 0108 0111 0112  ................
+00009bb0: 0113 011f 0128 0129 012a 012c 0131 013a  .....(.).*.,.1.:
+00009bc0: 013b 013c 013e 0143 014c 014d 014e 0150  .;.<.>.C.L.M.N.P
+00009bd0: 0156 015f 0160 0161 0163 016b 0174 0175  .V._.`.a.c.k.t.u
+00009be0: 0176 0179 0182 018b 018c 018d 018f 019e  .v.y............
+00009bf0: 01a7 01a8 01a9 01b3 01b4 01bd 01c2 01c3  ................
+00009c00: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+00009c10: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+00009c20: 0000 0002 0075 0069 6c73 7670 626c 6f62  .....u.ilsvpblob
+00009c30: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
+00009c40: 0405 0607 0809 0a0b 1d46 470a 2458 6963  .........FG.$Xic
+00009c50: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+00009c60: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+00009c70: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+00009c80: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+00009c90: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+00009ca0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+00009cb0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00009cc0: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
+00009cd0: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
+00009ce0: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+00009cf0: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+00009d00: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00009d10: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00009d20: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
+00009d30: 1a0a 1c1d 5569 6e64 6578 5961 7363 656e  ....UindexYascen
+00009d40: 6469 6e67 5577 6964 7468 5776 6973 6962  dingUwidthWvisib
+00009d50: 6c65 1007 0911 012c 08d4 1617 1819 1f1d  le.....,........
+00009d60: 211d 1008 0810 c808 d416 1718 1924 1d26  !............$.&
+00009d70: 0a10 0108 10b5 09d4 1617 1819 291d 261d  ............).&.
+00009d80: 1002 0808 d416 1718 192d 1d2f 0a10 0308  .........-./....
+00009d90: 1061 09d4 1617 1819 320a 341d 1005 0910  .a......2.4.....
+00009da0: 6408 d416 1718 1937 0a39 0a10 0409 1073  d......7.9.....s
+00009db0: 09d4 1617 1819 3c0a 3e1d 1006 0910 4b08  ......<.>.....K.
+00009dc0: d419 1718 160a 0a43 4409 0911 0251 1000  .......CD....Q..
+00009dd0: 0823 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
+00009de0: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+00009df0: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
+00009e00: 00da 00df 00e5 00ea 00f2 00f7 0100 0106  ................
+00009e10: 0110 0116 011e 0120 0121 0124 0125 012e  ....... .!.$.%..
+00009e20: 0130 0131 0133 0134 013d 013f 0140 0142  .0.1.3.4.=.?.@.B
+00009e30: 0143 014c 014e 014f 0150 0159 015b 015c  .C.L.N.O.P.Y.[.\
+00009e40: 015e 015f 0168 016a 016b 016d 016e 0177  .^._.h.j.k.m.n.w
+00009e50: 0179 017a 017c 017d 0186 0188 0189 018b  .y.z.|.}........
+00009e60: 018c 0195 0196 0197 019a 019c 019d 01a6  ................
+00009e70: 01ab 0000 0000 0000 0201 0000 0000 0000  ................
+00009e80: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+00009e90: 01ac 0000 0002 0075 0069 6d6f 4444 626c  .......u.imoDDbl
+00009ea0: 6f62 0000 0008 6da9 747c 5e01 c541 0000  ob....m.t|^..A..
+00009eb0: 0002 0075 0069 6d6f 6444 626c 6f62 0000  ...u.imodDblob..
+00009ec0: 0008 6da9 747c 5e01 c541 0000 0002 0075  ..m.t|^..A.....u
+00009ed0: 0069 7068 3153 636f 6d70 0000 0000 000f  .iph1Scomp......
+00009ee0: 1000 bc01 bd01 c601 cf01 d400 0000 0000  ................
+00009ef0: 0002 0100 0000 0000 0000 4c00 0000 0000  ..........L.....
+00009f00: 0000 0000 0000 0000 0001 dd00 0000 1300  ................
+00009f10: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+00009f20: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+00009f30: 6f00 6e00 736d 6f44 4462 6c6f 6200 0000  o.n.smoDDblob...
+00009f40: 08d9 7e4b 74e2 ddc4 4100 0000 1300 7000  ..~Kt...A.....p.
+00009f50: 6f00 7300 6500 5f00 6300 6f00 6e00 6600  o.s.e._.c.o.n.f.
+00009f60: 6900 6700 7500 7200 6100 7400 6900 6f00  i.g.u.r.a.t.i.o.
+00009f70: 6e00 736d 6f64 4462 6c6f 6200 0000 08d9  n.smodDblob.....
+00009f80: 7e4b 74e2 ddc4 4100 0000 1300 7000 6f00  ~Kt...A.....p.o.
+00009f90: 7300 6500 5f00 6300 6f00 6e00 6600 6900  s.e._.c.o.n.f.i.
+00009fa0: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00009fb0: 7370 6831 5363 6f6d 7000 0000 0000 0730  sph1Scomp......0
+00009fc0: 0000 0900 6c00 6100 6200 6500 6c00 6c00  ....l.a.b.e.l.l.
+00009fd0: 6900 6e00 676c 6731 5363 6f6d 7000 0000  i.n.glg1Scomp...
+00009fe0: 0000 018c 6000 0000 0000 0000 0000 0000  ....`...........
+00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a000: 0000 0000 0000 000b 0000 0000 0000 a00b  ................
+0000a010: 0000 0045 0000 100c 0000 900c 0000 200c  ...E.......... .
+0000a020: 0000 300c 0000 400c 0000 500c 0000 600c  ..0...@...P...`.
+0000a030: 0000 700c 0000 800c 0000 0000 0000 0000  ..p.............
+0000a040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a0a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a0b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a0c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a0d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a0e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a0f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a1a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a1b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a1c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a1d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a1e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a1f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a2a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a2b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a2c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a2d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a2e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a2f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a3a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a3b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a3c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a3d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a3e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a3f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+0000a410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+0000a420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000a430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+0000a440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+0000a450: 0100 0002 0000 0000 0100 0004 0000 0000  ................
+0000a460: 0200 0008 0000 00a8 0000 0000 0100 00b0  ................
+0000a470: 0000 0000 0000 0000 0100 00c0 0000 0000  ................
+0000a480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
+0000a490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
+0000a4a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
+0000a4b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
+0000a4c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
+0000a4d0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
+0000a4e0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
+0000a4f0: 0000 0000 0140 0000 0000 0000 0074 017d  .....@.......t.}
+0000a500: 017e 0181 0182 018b 019a 019b 019d 019e  .~..............
+0000a510: 01a7 01b1 01b2 01b3 01b4 01bd 01c2 01c3  ................
+0000a520: 0000 0000 0000 0201 0000 0000 0000 004a  ...............J
+0000a530: 0000 0000 0000 0000 0000 0000 0000 01c5  ................
+0000a540: 0000 0006 0000 000d 006f 0075 0074 006c  .........o.u.t.l
+0000a550: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+0000a560: 0073 6c73 7670 626c 6f62 0000 0294 6270  .slsvpblob....bp
+0000a570: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
+0000a580: 0a0b 0c0d 1c48 4948 4a0c 2958 6963 6f6e  .....HIHJ.)Xicon
+0000a590: 5369 7a65 5f10 0f73 686f 7749 636f 6e50  Size_..showIconP
+0000a5a0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
+0000a5b0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
+0000a5c0: 6573 5f10 0f73 6372 6f6c 6c50 6f73 6974  es_..scrollPosit
+0000a5d0: 696f 6e59 5874 6578 7453 697a 655f 100f  ionYXtextSize_..
+0000a5e0: 7363 726f 6c6c 506f 7369 7469 6f6e 585a  scrollPositionXZ
+0000a5f0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
+0000a600: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
+0000a610: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+0000a620: 6f6e 2340 3000 0000 0000 0009 d90e 0f10  on#@0...........
+0000a630: 1112 1314 1516 1720 252a 2e33 383d 4258  ....... %*.38=BX
+0000a640: 636f 6d6d 656e 7473 5e64 6174 654c 6173  comments^dateLas
+0000a650: 744f 7065 6e65 645c 6461 7465 4d6f 6469  tOpened\dateModi
+0000a660: 6669 6564 5b64 6174 6543 7265 6174 6564  fied[dateCreated
+0000a670: 5473 697a 6555 6c61 6265 6c54 6b69 6e64  TsizeUlabelTkind
+0000a680: 5776 6572 7369 6f6e 546e 616d 65d4 1819  WversionTname...
+0000a690: 1a1b 1c1d 0c1f 5776 6973 6962 6c65 5577  ......WvisibleUw
+0000a6a0: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
+0000a6b0: 6e64 6578 0811 012c 0910 07d4 1819 1a1b  ndex...,........
+0000a6c0: 1c22 1c24 0810 c808 1008 d418 191a 1b0c  .".$............
+0000a6d0: 271c 2909 10b5 0810 01d4 1819 1a1b 1c27  '.)............'
+0000a6e0: 1c2d 0808 1002 d418 191a 1b0c 301c 3209  .-..........0.2.
+0000a6f0: 1061 0810 03d4 1819 1a1b 1c35 0c37 0810  .a.........5.7..
+0000a700: 6409 1005 d418 191a 1b0c 3a0c 3c09 1073  d.........:.<..s
+0000a710: 0910 04d4 1819 1a1b 1c3f 0c41 0810 4b09  .........?.A..K.
+0000a720: 1006 d41b 191a 1843 440c 0c10 0010 f009  .......CD.......
+0000a730: 0908 2300 0000 0000 0000 0023 4028 0000  ..#........#@(..
+0000a740: 0000 0000 546e 616d 6509 0008 001d 0026  ....Tname......&
+0000a750: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
+0000a760: 00b4 00bd 00be 00d1 00da 00e9 00f6 0102  ................
+0000a770: 0107 010d 0112 011a 011f 0128 0130 0136  ...........(.0.6
+0000a780: 0140 0146 0147 014a 014b 014d 0156 0157  .@.F.G.J.K.M.V.W
+0000a790: 0159 015a 015c 0165 0166 0168 0169 016b  .Y.Z.\.e.f.h.i.k
+0000a7a0: 0174 0175 0176 0178 0181 0182 0184 0185  .t.u.v.x........
+0000a7b0: 0187 0190 0191 0193 0194 0196 019f 01a0  ................
+0000a7c0: 01a2 01a3 01a5 01ae 01af 01b1 01b2 01b4  ................
+0000a7d0: 01bd 01bf 01c1 01c2 01c3 01c4 01cd 01d6  ................
+0000a7e0: 01db 0000 0000 0000 0201 0000 0000 0000  ................
+0000a7f0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
+0000a800: 01dc 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/perimeter_jit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Simon Nilsson"
 ### modified from https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179
 
 import numpy as np
-from numba import njit, prange
+from numba import njit, jit, prange
 from numba.np.extensions import cross2d
 
 @njit('(float32[:,:], int64[:], int64, int64)')
 def process(S, P, a, b):
     signed_dist = cross2d(S[P] - S[a], S[b] - S[a])
     K = np.array([i for s, i in zip(signed_dist, P) if s > 0 and i != a and i != b], dtype=np.int64)
     if len(K) == 0:
@@ -23,40 +23,70 @@
     :return: 1d np.array
 
     :EXAMPLE:
     >>> points = np.random.randint(1, 50, size=(50, 5, 2)).astype(float)
     >>> results = jitted_hull(points, target='area')
     """
 
-    results = np.full((points.shape[0]), np.nan)
-
     def perimeter(xy):
         perimeter = np.linalg.norm(xy[0] - xy[-1])
         for i in prange(xy.shape[0]-1):
             p = np.linalg.norm(xy[i] - xy[i+1])
             perimeter+=p
         return perimeter
 
     def area(x, y):
         return 0.5 * np.abs(np.dot(x, np.roll(y, 1)) - np.dot(y, np.roll(x, 1)))
 
+    results = np.full((points.shape[0]), np.nan)
     for i in range(points.shape[0]):
         S = points[i, :, :]
         a, b = np.argmin(S[:,0]), np.argmax(S[:,0])
         max_index = np.argmax(S[:,0])
         idx = process(S, np.arange(S.shape[0]), a, max_index)[:-1] + process(S, np.arange(S.shape[0]), max_index, a)[:-1]
         x, y = np.full((len(idx)), np.nan), np.full((len(idx)), np.nan)
         for j in prange(len(idx)):
             x[j], y[j] = S[idx[j], 0], S[idx[j], 1]
-
         x0, y0 = np.mean(x), np.mean(y)
         r = np.sqrt((x - x0) ** 2 + (y - y0) ** 2)
         angles = np.where((y - y0) > 0, np.arccos((x - x0) / r), 2 * np.pi - np.arccos((x - x0) / r))
         mask = np.argsort(angles)
         x_sorted, y_sorted = x[mask], y[mask]
         if target == 'perimeter':
             xy = np.vstack((x_sorted, y_sorted)).T
             results[i] = perimeter(xy)
         if target == 'area':
             results[i] = area(x_sorted, y_sorted)
 
-    return results
+    return results
+
+
+@jit(nopython=True)
+def jitted_centroid(points: np.ndarray) -> np.ndarray:
+
+    """
+    :param array points: 3d array FRAMESxBODY-PARTxCOORDINATE
+    :param str target: Options [perimeter, area]
+    :return: 1d np.array
+
+    :EXAMPLE:
+    >>> points = np.random.randint(1, 50, size=(50, 5, 2)).astype(float)
+    >>> results = jitted_centroid(points)
+    """
+    results = np.full((points.shape[0], 2), np.nan)
+    for i in range(points.shape[0]):
+        S = points[i, :, :]
+        a, b = np.argmin(S[:,0]), np.argmax(S[:,0])
+        max_index = np.argmax(S[:,0])
+        idx = process(S, np.arange(S.shape[0]), a, max_index)[:-1] + process(S, np.arange(S.shape[0]), max_index, a)[:-1]
+        perimeter_points = np.full((len(idx), 2), np.nan)
+        for j in prange(len(idx)):
+            perimeter_points[j] = points[i][j]
+        results[i][0] = np.int(np.mean(perimeter_points[:, 0].flatten()))
+        results[i][1] = np.int(np.mean(perimeter_points[:, 1].flatten()))
+    return results
+
+points = np.random.randint(1, 10, size=(50, 5, 2)).astype(np.float32)
+results = jitted_centroid(points)
+#
+#
+# results = np.full((points.shape[0]), np.nan)
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.6/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/requirements.txt` & `Simba-UW-tf-dev-1.58.6/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/pop_up_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,14 @@
         self.animal_cnt_confirm_btn = Button(self.animal_cnt_frm, text="Confirm", command=lambda: self.update_body_parts())
         self.animal_cnt_frm.grid(row=self.children_cnt_main(), sticky=NW)
         self.animal_cnt_dropdown.grid(row=self.children_cnt_main(), column=1, sticky=NW)
         self.animal_cnt_confirm_btn.grid(row=self.children_cnt_main(), column=2, sticky=NW)
         self.create_choose_body_parts_frm()
         self.update_body_parts()
 
-
     def create_choose_body_parts_frm(self):
         if hasattr(self, 'body_part_frm'):
             self.body_part_frm.destroy()
         self.body_parts_dropdown_dict = {}
         self.body_part_frm = LabelFrame(self.main_frm, text="CHOOSE ANIMAL BODY-PARTS", font=Formats.LABELFRAME_HEADER_FORMAT.value, name='choose animal body-parts')
         self.body_part_frm.grid(row=self.children_cnt_main(), sticky=NW)
 
@@ -173,16 +172,14 @@
                                         list_boxes: list,
                                         values: list):
         if len(list_boxes) != len(values):
             raise CountError(msg='Value count and listboxes count are not equal')
         for i in range(len(list_boxes)):
             list_boxes[i].insert(0, values[i])
 
-
-
     def remove_from_listbox(self,
                             list_box: Listbox):
         selection = list_box.curselection()
         if selection:
             list_box.delete(selection[0])
 
 
@@ -194,14 +191,25 @@
         self.body_part_frm.grid(row=self.children_cnt_main(), sticky=NW)
         for bp_cnt in range(int(self.bp_cnt_dropdown.getChoices())):
             self.body_parts_dropdowns[bp_cnt] = DropDownMenu(self.body_part_frm, f'Body-part {str(bp_cnt+1)}:', project_body_parts, '25')
             self.body_parts_dropdowns[bp_cnt].grid(row=bp_cnt, column=0, sticky=NW)
             self.body_parts_dropdowns[bp_cnt].setChoices(project_body_parts[bp_cnt])
         self.create_run_frm(run_function=run_function)
 
+    def choose_bp_frm(self, parent: LabelFrame, bp_options: list):
+        self.body_parts_dropdowns = {}
+        self.body_part_frm = LabelFrame(parent, text="CHOOSE ANIMAL BODY-PARTS",
+                                        font=Formats.LABELFRAME_HEADER_FORMAT.value, name='choose animal body-parts')
+        self.body_part_frm.grid(row=self.frame_children(frame=parent), sticky=NW)
+        for bp_cnt in range(int(self.animal_cnt_dropdown.getChoices())):
+            self.body_parts_dropdowns[bp_cnt] = DropDownMenu(self.body_part_frm, f'Body-part {str(bp_cnt + 1)}:', bp_options, '20')
+            self.body_parts_dropdowns[bp_cnt].grid(row=bp_cnt, column=0, sticky=NW)
+            self.body_parts_dropdowns[bp_cnt].setChoices(bp_options[bp_cnt])
+
+
 
     def children_cnt_main(self):
         return int(len(list(self.main_frm.children.keys())))
 
     def frame_children(self, frame: Frame):
         return int(len(list(frame.children.keys())))
 
@@ -211,14 +219,21 @@
 
     def show_smoothing_entry_box_from_dropdown(self, choice):
         if choice == 'None':
             self.smoothing_time_eb.grid_forget()
         if (choice == 'Gaussian') or (choice == 'Savitzky Golay'):
             self.smoothing_time_eb.grid(row=0, column=1, sticky=E)
 
+    def choose_bp_threshold_frm(self, parent: LabelFrame):
+        self.probability_frm = LabelFrame(parent, text="PROBABILITY THRESHOLD", font=Formats.LABELFRAME_HEADER_FORMAT.value)
+        self.probability_frm.grid(row=self.frame_children(frame=parent), column=0, sticky=NW)
+        self.probability_entry = Entry_Box(self.probability_frm, "Probability threshold: ", labelwidth=20)
+        self.probability_entry.entry_set('0.00')
+        self.probability_entry.grid(row=0, column=0, sticky=NW)
+
 
     def enable_dropdown_from_checkbox(self,
                                       check_box_var: BooleanVar,
                                       dropdown_menus: [DropDownMenu]):
         if check_box_var.get():
             for menu in dropdown_menus:
                 menu.enable()
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.58.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/feature_extraction_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import warnings
 warnings.filterwarnings("ignore")
 import numpy as np
 from numba import jit, prange
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
+from scipy.signal import savgol_filter
 import math
 import os, glob
 from scipy import stats
 import pandas as pd
 from scipy.signal import find_peaks
 from simba.utils.enums import Paths, Options
 from simba.utils.checks import check_if_filepath_list_is_empty, check_file_exist_and_readable, check_minimum_roll_windows
@@ -384,14 +385,35 @@
         results = np.full((location_1.shape[0]), np.nan)
         for i in prange(location_1.shape[0]):
             results[i] = np.linalg.norm(location_1[i] - location_2[i]) / px_per_mm
         if centimeter:
             results = results / 10
         return results
 
+    def dataframe_gaussian_smoother(self,
+                                    df: pd.DataFrame,
+                                    fps: int,
+                                    time_window: int=100):
+
+        frames_in_time_window = int(time_window / (1000 / fps))
+        for c in df.columns:
+            df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
+        return df
+
+
+    def dataframe_savgol_smoother(self,
+                                  df: pd.DataFrame,
+                                  fps: int,
+                                  time_window: int = 150):
+        frames_in_time_window = int(time_window / (1000 / fps))
+        if (frames_in_time_window % 2) == 0: frames_in_time_window = frames_in_time_window - 1
+        if (frames_in_time_window % 2) <= 3: frames_in_time_window = 5
+        for c in df.columns:
+            df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
+        return df
 
     def get_bp_headers(self):
         """
         Helper to create ordered list of all column header fields for SimBA project dataframes.
         """
         self.col_headers = []
         for bp in self.body_parts_lst:
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/plotting_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,14 @@
         color_dict = get_color_dict()
 
         img = np.zeros((int(video_info['Resolution_height'].values[0]), int(video_info['Resolution_width'].values[0]), 3))
         img[:] = style_attr['bg color']
 
         for animal_name, animal_data in deque_dict.items():
             cv2.circle(img, (deque_dict[animal_name]['deque'][0]), 0, deque_dict[animal_name]['clr'], style_attr['circle size'])
-            print(animal_name, style_attr['font size'])
             cv2.putText(img, animal_name, (deque_dict[animal_name]['deque'][0]), font, style_attr['font size'], deque_dict[animal_name]['clr'], style_attr['font thickness'])
 
         for animal_name, animal_data in deque_dict.items():
             for i in range(len(deque_dict[animal_name]['deque']) - 1):
                 line_clr = deque_dict[animal_name]['clr']
                 position_1 = deque_dict[animal_name]['deque'][i]
                 position_2 = deque_dict[animal_name]['deque'][i + 1]
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/unsupervised_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 __author__ = "Simon Nilsson"
 
 import os, glob
 import pickle
 import simba
 from simba.utils.enums import Paths
 from sklearn.feature_selection import VarianceThreshold
-from simba.unsupervised.enums import Unsupervised
+
 import pandas as pd
 from datetime import datetime
 import numpy as np
+
 from sklearn.preprocessing import (MinMaxScaler,
                                    StandardScaler,
                                    QuantileTransformer)
 from simba.utils.errors import (InvalidInputError,
                                 NoDataError,
                                 NoFilesFoundError,
                                 InvalidFileTypeError,
                                 MissingColumnsError,
                                 IntegerError,
                                 DirectoryNotEmptyError)
 from simba.utils.checks import check_float
 from simba.utils.printing import SimbaTimer
+from simba.unsupervised.enums import Unsupervised, UMLOptions
 
 
 class UnsupervisedMixin(object):
     def __init__(self):
 
         """
         Methods for unsupervised ML.
@@ -64,32 +66,32 @@
                                    hyper_parameters):
         for key in Unsupervised.HYPERPARAMETERS.value:
             if key not in hyper_parameters.keys():
                 raise InvalidInputError(msg=f'Hyperparameter dictionary is missing {key} entry.')
         for key in [Unsupervised.N_NEIGHBORS.value, Unsupervised.MIN_DISTANCE.value, Unsupervised.SPREAD.value]:
             if len(hyper_parameters[key]) == 0:
                 raise InvalidInputError(msg=f'Hyperparameter dictionary key {key} has 0 entries.')
-        if hyper_parameters[Unsupervised.SCALER.value] not in Unsupervised.SCALER_NAMES.value:
-            raise InvalidInputError(msg=f'Scaler {Unsupervised.SCALER.value} not supported. Opitions: {Unsupervised.SCALER_NAMES.value}')
+        if hyper_parameters[Unsupervised.SCALER.value] not in UMLOptions.SCALER_OPTIONS.value:
+            raise InvalidInputError(msg=f'Scaler {Unsupervised.SCALER.value} not supported. Opitions: {UMLOptions.SCALER_OPTIONS.value}')
         check_float('VARIANCE THRESHOLD', value=hyper_parameters[Unsupervised.VARIANCE.value])
 
     def find_low_variance_fields(self, data: pd.DataFrame, variance: float):
         feature_selector = VarianceThreshold(threshold=round((variance / 100), 2))
         feature_selector.fit(data)
         low_variance_fields = [c for c in data.columns if c not in data.columns[feature_selector.get_support()]]
         if len(low_variance_fields) == len(data.columns):
             raise NoDataError(msg=f'All feature columns show a variance below the {str(variance)} threshold. Thus, no data remain for analysis.')
         return low_variance_fields
 
     def drop_fields(self, data: pd.DataFrame, fields: list):
         return data.drop(columns=fields)
 
     def define_scaler(self, scaler_name: str):
-        if scaler_name not in Unsupervised.SCALER_NAMES.value:
-            raise InvalidInputError(msg=f'Scaler {scaler_name} not supported. Options: {Unsupervised.SCALER_NAMES.value}')
+        if scaler_name not in UMLOptions.SCALER_OPTIONS.value:
+            raise InvalidInputError(msg=f'Scaler {scaler_name} not supported. Options: {UMLOptions.SCALER_OPTIONS.value}')
         if scaler_name == Unsupervised.MIN_MAX.value:
             return MinMaxScaler()
         elif scaler_name == Unsupervised.STANDARD.value:
             return StandardScaler()
         elif scaler_name == Unsupervised.QUANTILE.value:
             return QuantileTransformer()
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.58.6/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.58.6/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/enums.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,17 @@
     ROI_DATA_PLOT = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-4-visualizing-roi-data'
     DIRECTING_ANIMALS_PLOTS = 'https://github.com/sgoldenlab/simba/blob/master/docs/directionality_between_animals.md'
     CLF_VALIDATION = 'https://github.com/sgoldenlab/simba/blob/master/docs/classifier_validation.md'
     BATCH_PREPROCESS = 'https://github.com/sgoldenlab/simba/blob/master/docs/tutorial_process_videos.md'
     THIRD_PARTY_ANNOTATION_NEW = 'https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot_new.md'
     OUT_OF_SAMPLE_VALIDATION = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#step-8-evaluating-the-model-on-new-out-of-sample-data'
     ROI = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial_new.md'
+    ROI_FEATURES = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-3-generating-features-from-roi-data'
+    ROI_DATA_ANALYSIS = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-2-analyzing-roi-data'
+    DATA_ANALYSIS = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results'
     ANALYZE_ROI = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-2-analyzing-roi-data'
     EXTRACT_FEATURES = 'https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#step-5-extract-features'
     APPEND_ROI_FEATURES = 'https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial.md#part-3-generating-features-from-roi-data'
     LABEL_BEHAVIOR = 'https://github.com/sgoldenlab/simba/blob/master/docs/label_behavior.md'
     THIRD_PARTY_ANNOTATION = 'https://github.com/sgoldenlab/simba/blob/master/docs/third_party_annot.md'
     PSEUDO_LBL = 'https://github.com/sgoldenlab/simba/blob/master/docs/pseudoLabel.md'
     ADVANCED_LBL = 'https://github.com/sgoldenlab/simba/blob/master/docs/advanced_labelling.md'
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/checks.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/errors.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/data.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/utils/printing.py` & `Simba-UW-tf-dev-1.58.6/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/plot_clf_results_mp.py`

 * *Files 14% similar despite different names*

```diff
@@ -244,53 +244,30 @@
 
         self.timer.stop_timer()
         if self.video_setting:
             stdout_success(msg=f'{len(self.files_found)} videos saved in project_folder/frames/output/sklearn_results directory', elapsed_time=self.timer.elapsed_time_str)
         if self.frame_setting:
             stdout_success(f'Frames for {len(self.files_found)} videos saved in sub-folders within project_folder/frames/output/sklearn_results directory', elapsed_time=self.timer.elapsed_time_str)
 
-# test = PlotSklearnResultsMultiProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
-#                                       video_setting=True,
-#                                       frame_setting=False,
-#                                       video_file_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/videos/SF2.mp4',
-#                                       print_timers=True,
-#                                       text_settings=False,
-#                                       cores=6,
-#                                       rotate=False)
-# test.initialize_visualizations()
 
-
-
-
-
-
-# test = PlotSklearnResultsMultiProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
-#                                       video_setting=True,
-#                                       frame_setting=False,
-#                                       video_file_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/videos/Together_1.avi',
-#                                       print_timers=True,
-#                                       text_settings=False,
-# cores=6,
-#                                       rotate=False)
-# test.initialize_visualizations()
-
-
-# test = PlotSklearnResultsMultiProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                       video_setting=True,
-#                                       frame_setting=False,
-#                                       video_file_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Together_1.avi',
-#                                       print_timers=True,
-#                                       text_settings=False,
-#                                       cores=6,
-#                                       rotate=False)
-# test.initialize_visualizations()
-
-
-# test = PlotSklearnResultsMultiProcess(config_path='/Users/simon/Desktop/envs/troubleshooting/Rat_NOR_BAD/project_folder/project_config.ini',
-#                                       video_setting=True,
-#                                       frame_setting=False,
-#                                       cores=6,
-#                                       video_file_path='/Users/simon/Desktop/envs/troubleshooting/Rat_NOR_BAD/project_folder/videos/03142021_NOB_DOT_5_upsidedown.mp4',
-#                                       print_timers=True,
-#                                       text_settings=False,
-#                                       rotate=False)
-# test.initialize_visualizations()
+# style_attr = {'width': 'As input',
+#               'height': 'As input',
+#               'line width': 5,
+#               'font size': 5,
+#               'font thickness': 2,
+#               'circle size': 5,
+#               'bg color': 'White',
+#               'max lines': 10000}
+#
+# animal_attr = {0: ['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Green']}
+# clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Black', 'Size: 30']}
+#
+# test = PathPlotterSingleCore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                             frame_setting=False,
+#                             video_setting=True,
+#                              last_frame=True,
+#                             input_style_attr=style_attr,
+#                    animal_attr=animal_attr,
+#                              input_clf_attr=clf_attr,
+#                     files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv',
+#                                  '/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'])
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/path_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,22 +236,22 @@
             self.deque_dict[animal]['deque'] = deque(maxlen=self.style_attr['max lines'])
             self.deque_dict[animal]['bp'] = self.animal_attr[animal_cnt][0]
             self.deque_dict[animal]['clr'] = self.color_dict[self.animal_attr[animal_cnt][1]]
 
 
 # style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 10000}
 # animal_attr = {0: ['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Green']}
-# clf_attr = {0: ['Attack', 'Black', 'Size: 30']}
+# clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Black', 'Size: 30']}
 # #
 # # clf_attr = None
 # # style_attr = None
 #
 # path_plotter = PathPlotterMulticore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                     frame_setting=False,
-#                                     video_setting=False,
+#                                     video_setting=True,
 #                                     last_frame=True,
 #                                     input_clf_attr=clf_attr,
 #                                     input_style_attr=style_attr,
 #                                     animal_attr=animal_attr,
 #                                     files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'],
 #                                     cores=5)
 # path_plotter.create_path_plots()
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/data_plotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,29 +46,28 @@
         super().__init__(config_path=config_path)
         if (not video_setting) and (not frame_setting):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choose to create video and/or frames data plots. SimBA found that you ticked neither video and/or frames')
         self.video_setting, self.frame_setting = video_setting, frame_setting
         self.files_found, self.style_attr, self.body_part_attr = data_paths, style_attr, body_part_attr
         if not os.path.exists(self.data_table_path):
             os.makedirs(self.data_table_path)
-        self.__compute_spacings()
         self.process_movement()
-        print('Processing {} video(s)...'.format(str(len(self.files_found))))
+        print(f'Processing {len(self.files_found)} video(s)...')
 
     def __compute_spacings(self):
         """
         Private helper to compute appropriate spacing between printed text.
         """
         self.loc_dict = {}
         self.loc_dict['Animal'] = (50, 20)
         self.loc_dict['total_movement_header'] = (250, 20)
         self.loc_dict['current_velocity_header'] = (475, 20)
         self.loc_dict['animals'] = {}
         y_cord, x_cord = 75, 15
-        for animal_cnt, animal_name in enumerate(self.multi_animal_id_list):
+        for animal_cnt, animal_name in enumerate(self.video_data.columns):
             self.loc_dict['animals'][animal_name] = {}
             self.loc_dict['animals'][animal_name]['index_loc'] = (50, y_cord)
             self.loc_dict['animals'][animal_name]['total_movement_loc'] = (250, y_cord)
             self.loc_dict['animals'][animal_name]['current_velocity_loc'] = (475, y_cord)
             y_cord += 50
 
     def process_movement(self):
@@ -76,25 +75,19 @@
         Method to create movement data for visualization
 
         Returns
         -------
         Attribute: pd.Dataframe
             movement
         """
-        self.config.set('process movements', 'no_of_animals', str(len(self.body_part_attr)))
-        self.config.set('process movements', 'probability_threshold', str(0.00))
-        for animal_cnt, animal in enumerate(self.body_part_attr):
-            self.config.set('process movements', 'animal_{}_bp'.format(animal_cnt + 1), animal[0])
-        with open(self.config_path, 'w') as file:
-            self.config.write(file)
-        movement_processor = MovementCalculator(config_path=self.config_path, visualization=True, files=self.files_found)
+        movement_processor = MovementCalculator(config_path=self.config_path, file_paths=self.files_found, threshold=0.00, body_parts=[x[0] for x in self.body_part_attr])
         movement_processor.run()
-        self.movement = movement_processor.movement_dict
+        self.movement = movement_processor.movement_dfs
 
-    def create_data_plots(self):
+    def run(self):
         """
         Method to create and save visualizations on disk from data created in
         :meth:`~simba.DataPlotter.process_movement`. Results are stored in the `project_folder/frames/output/live_data_table`.
 
         Returns
         -------
         None
@@ -119,38 +112,38 @@
                 current_velocity = str(round(video_data_slice[animal_name].sum() / 10, style_attr['data_accuracy']))
                 cv2.putText(img, animal_name, location_dict['animals'][animal_name]['index_loc'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, clr, 1)
                 cv2.putText(img, total_movement, location_dict['animals'][animal_name]['total_movement_loc'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, clr, 1)
                 cv2.putText(img, current_velocity, location_dict['animals'][animal_name]['current_velocity_loc'], cv2.FONT_HERSHEY_TRIPLEX, 0.5, clr, 1)
             return img
 
         for file_cnt, file_path in enumerate(self.files_found):
-            video_timer = SimbaTimer()
-            video_timer.start_timer()
+            video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(file_path)
-            video_data = pd.DataFrame(self.movement[video_name])
+            self.video_data = pd.DataFrame(self.movement[video_name])
+            self.__compute_spacings()
             _, _, self.fps = self.read_video_info(video_name=video_name)
             if self.video_setting:
                 self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
                 self.video_save_path = os.path.join(self.data_table_path, video_name + '.mp4')
                 self.writer = cv2.VideoWriter(self.video_save_path, self.fourcc, self.fps, self.style_attr['size'])
             if self.frame_setting:
                 self.frame_save_path = os.path.join(self.data_table_path, video_name)
                 if not os.path.exists(self.frame_save_path): os.makedirs(self.frame_save_path)
-            video_data_lst = np.array_split(pd.DataFrame(video_data), int(len(video_data) / self.fps))
-            self.imgs = Parallel(n_jobs=self.cpu_to_use, verbose=1, backend="threading")(delayed(multiprocess_img_creation)(x, self.loc_dict, self.multi_animal_id_list, video_data, self.style_attr, self.body_part_attr) for x in video_data_lst)
+            video_data_lst = np.array_split(pd.DataFrame(self.video_data), int(len(self.video_data) / self.fps))
+            self.imgs = Parallel(n_jobs=self.cpu_to_use, verbose=1, backend="threading")(delayed(multiprocess_img_creation)(x, self.loc_dict, self.video_data.columns, self.video_data, self.style_attr, self.body_part_attr) for x in video_data_lst)
             frm_cnt = 0
             for img_cnt, img in enumerate(self.imgs):
                 for frame_cnt in range(int(self.fps)):
                     if self.video_setting:
                         self.writer.write(np.uint8(img))
                     if self.frame_setting:
                         frm_save_name = os.path.join(self.frame_save_path, '{}.png'.format(str(frm_cnt)))
                         cv2.imwrite(frm_save_name, np.uint8(img))
                     frm_cnt += 1
-                    print('Frame: {} / {}. Video: {} ({}/{})'.format(str(frm_cnt), str(len(video_data)),
+                    print('Frame: {} / {}. Video: {} ({}/{})'.format(str(frm_cnt), str(len(self.video_data)),
                                                                    video_name, str(file_cnt + 1),
                                                                    len(self.files_found)))
 
             print('Data tables created for video {}...'.format(video_name))
             if self.video_setting:
                 self.writer.release()
                 video_timer.stop_timer()
@@ -166,15 +159,15 @@
 #
 # test = DataPlotter(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                    style_attr=style_attr,
 #                    body_part_attr=body_part_attr,
 #                    data_paths=data_paths,
 #                    video_setting=True,
 #                    frame_setting=False)
-# test.create_data_plots()
+# test.run()
 
 # style_attr = {'bg_color': 'White', 'header_color': 'Black', 'font_thickness': 1, 'size': (640, 480), 'data_accuracy': 2}
 # body_part_attr = [['Ear_left_1', 'Grey'], ['Ear_right_2', 'Red']]
 # data_paths = ['/Users/simon/Desktop/envs/simba_dev/tests/test_data/two_C57_madlc/project_folder/csv/outlier_corrected_movement_location/Together_1.csv']
 #
 #
 # test = DataPlotter(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/two_C57_madlc/project_folder/project_config.ini',
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/path_plotter.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.no_animals_path_plot, self.clf_attr = len(animal_attr.keys()), None
         if not os.path.exists(self.path_plot_dir):
             os.makedirs(self.path_plot_dir)
         check_if_filepath_list_is_empty(filepaths=self.files_found,
                                         error_msg='Zero files found in the project_folder/csv/machine_results directory. To plot paths without performing machine classifications, use path plotter functions in [ROI] tab.')
         print(f'Processing {str(len(self.files_found))} videos...')
 
-    def create_path_plots(self):
+    def run(self):
         """
         Method to create path plot videos and/or frames.Results are store in the
         'project_folder/frames/path_plots' directory of the SimBA project.
         """
 
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer()
@@ -124,22 +124,22 @@
                     for animal_name, animal_data in self.deque_dict.items():
                         for i in range(len(self.deque_dict[animal_name]['deque'])-1):
                             line_clr = self.deque_dict[animal_name]['clr']
                             position_1 = self.deque_dict[animal_name]['deque'][i]
                             position_2 = self.deque_dict[animal_name]['deque'][i+1]
                             cv2.line(img, position_1, position_2, line_clr, self.style_attr['line width'])
 
-                    if self.clf_attr:
+                    if self.input_clf_attr:
                         animal_1_name = list(self.deque_dict.keys())[0]
                         animal_bp_x, animal_bp_y = self.deque_dict[animal_1_name]['bp'] + '_x', self.deque_dict[animal_1_name]['bp'] + '_y'
-                        for clf_cnt, clf_data in self.clf_attr.items():
-                            clf_size = int(clf_data[-1].split(': ')[-1])
-                            clf_clr = self.color_dict[clf_data[1]]
-                            sliced_df = clf_df.loc[0: frm_cnt]
-                            sliced_df_idx = list(sliced_df[sliced_df[clf_data[0]] == 1].index)
+                        for clf_cnt, clf_name in enumerate(self.clf_attr['data'].columns):
+                            clf_size = int(self.clf_attr['attr'][clf_cnt][-1].split(': ')[-1])
+                            clf_clr = self.color_dict[self.clf_attr['attr'][clf_cnt][1]]
+                            sliced_df = self.clf_attr['data'].loc[0: frm_cnt]
+                            sliced_df_idx = list(sliced_df[sliced_df[self.clf_attr['attr'][clf_cnt][0]] == 1].index)
                             locations = self.data_df.loc[sliced_df_idx, [animal_bp_x, animal_bp_y]].astype(int).values
                             for i in range(locations.shape[0]):
                                 cv2.circle(img, (locations[i][0], locations[i][1]), 0, clf_clr, clf_size)
 
                     img = cv2.resize(img, (self.style_attr['width'], self.style_attr['height']))
                     if self.video_setting:
                         self.writer.write(np.uint8(img))
@@ -186,37 +186,37 @@
         for animal_cnt, animal_data in self.animal_attr.items():
             animal_name = self.find_animal_name_from_body_part_name(bp_name=animal_data[0], bp_dict=self.animal_bp_dict)
             self.deque_dict[animal_name] = {}
             self.deque_dict[animal_name]['deque'] = deque(maxlen=self.style_attr['max lines'])
             self.deque_dict[animal_name]['bp'] = self.animal_attr[animal_cnt][0]
             self.deque_dict[animal_name]['clr'] = self.color_dict[self.animal_attr[animal_cnt][1]]
 
-#
+
 # style_attr = {'width': 'As input',
 #               'height': 'As input',
 #               'line width': 5,
 #               'font size': 5,
 #               'font thickness': 2,
 #               'circle size': 5,
 #               'bg color': 'White',
 #               'max lines': 10000}
 #
 # animal_attr = {0: ['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Green']}
-# clf_attr = {0: ['Attack', 'Black', 'Size: 30']}
+# clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Black', 'Size: 30']}
 #
 # test = PathPlotterSingleCore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                             frame_setting=False,
 #                             video_setting=True,
 #                              last_frame=True,
 #                             input_style_attr=style_attr,
 #                    animal_attr=animal_attr,
 #                              input_clf_attr=clf_attr,
 #                     files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv',
 #                                  '/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/machine_results/Together_1.csv'])
-# test.create_path_plots()
+# test.run()
 
 # test = PathPlotterSingleCore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                    frame_setting=False,
 #                    video_setting=False,
 #                              last_frame=True,
 #                    style_attr=style_attr,
 #                    animal_attr=animal_attr,
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.58.6/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.58.6/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.58.6/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.58.6/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,104 @@
-__author__ = "Simon Nilsson"
-
-import pandas as pd
 import os
-from collections import defaultdict
-import numpy as np
-from statistics import mean
+import pandas as pd
+import itertools
+from simba.roi_tools.ROI_analyzer import ROIAnalyzer
 from simba.utils.printing import stdout_success
-from simba.utils.read_write import read_config_entry, read_df, get_fn_ext
-from simba.utils.checks import check_if_filepath_list_is_empty
-from simba.utils.errors import NoSpecifiedOutputError
-from simba.utils.enums import ConfigKey
+from simba.utils.enums import ConfigKey, DirNames, Dtypes
 from simba.mixins.config_reader import ConfigReader
-from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
+from simba.utils.read_write import get_fn_ext, read_config_entry, read_df
 
-class MovementCalculator(ConfigReader,
-                         FeatureExtractionMixin):
+class ROITimebinCalculator(ConfigReader):
     """
-    Class for computing aggregate movement statistics.
+    Class for calulating how much time and how many entries animals are making into user-defined ROIs
+    in user-defined time bins. Results are stored in the `project_folder/logs` directory of the SimBA project.
 
     Parameters
     ----------
     config_path: str
         path to SimBA project config file in Configparser format
+    bin_length: int
+        length of time bins in seconds.
 
     Notes
     ----------
 
     Examples
     ----------
-    >>> movement_processor = MovementProcessor(config_path='MyConfigPath')
-    >>> movement_processor.run()
-    >>> movement_processor.save()
-
+    >>> roi_time_bin_calculator = ROITimebinCalculator(config_path='MySimBaConfigPath', bin_length=15)
+    >>> roi_time_bin_calculator.run()
+    >>> roi_time_bin_calculator.save()
     """
 
     def __init__(self,
                  config_path: str,
-                 visualization: bool = False,
-                 files: list=None):
+                 bin_length: int):
 
-        super().__init__(config_path=config_path)
-        self.save_path = os.path.join(self.logs_path, 'Movement_log_{}.csv'.format(self.datetime))
-        try:
-            self.animal_cnt = read_config_entry(self.config, ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'no_of_animals', 'int')
-            self.p_threshold = read_config_entry(self.config, ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'probability_threshold', 'float')
-        except:
-            raise NoSpecifiedOutputError(msg='Please analyze movements before visualizing data.')
-        self.bp_dict = defaultdict(list)
-        self.bp_columns = []
-        if not visualization:
-            for cnt, animal in enumerate(self.multi_animal_id_list):
-                bp_name = read_config_entry(self.config, ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(cnt + 1), 'str')
-                if bp_name == 'None':
-                    raise NoSpecifiedOutputError(msg=f'No body-parts found in config [process movements][animal_N_bp]')
-                for c in ['_x', '_y', '_p']:
-                    self.bp_dict[animal].append(bp_name + c)
-                    self.bp_columns.append(bp_name + c)
-            check_if_filepath_list_is_empty(filepaths=self.outlier_corrected_paths,
-                                            error_msg=f'SIMBA ERROR: Cannot process movement. ZERO data files found in the {self.outlier_corrected_dir} directory.')
-            self.files_found = self.outlier_corrected_paths
-        else:
-            for cnt in range(self.animal_cnt):
-                bp_name = read_config_entry(self.config, ConfigKey.PROCESS_MOVEMENT_SETTINGS.value, 'animal_{}_bp'.format(cnt + 1), 'str')
-                if bp_name == 'None':
-                    raise NoSpecifiedOutputError(msg=f'No body-parts found in config [process movements][animal_N_bp]')
-                for c in ['_x', '_y', '_p']:
-                    self.bp_dict[self.multi_animal_id_list[cnt]].append(bp_name + c)
-                    self.bp_columns.append(bp_name + c)
-            self.files_found = files
-        print(f'Processing {str(len(self.outlier_corrected_paths))} video(s)...')
+        ConfigReader.__init__(self, config_path=config_path)
+        self.bin_length = bin_length
+        self.roi_animal_cnt = read_config_entry(config=self.config, section=ConfigKey.ROI_SETTINGS.value, option=ConfigKey.ROI_ANIMAL_CNT.value, data_type=Dtypes.INT.value)
+        self.probability_threshold = read_config_entry(config=self.config, section=ConfigKey.ROI_SETTINGS.value, option=ConfigKey.PROBABILITY_THRESHOLD.value, data_type=Dtypes.FLOAT.value, default_value=0.00)
+        self.save_path_time = os.path.join(self.logs_path, 'ROI_time_bins_{}s_time_data_{}.csv'.format(str(bin_length), self.datetime))
+        self.save_path_entries = os.path.join(self.logs_path, 'ROI_time_bins_{}s_entry_data_{}.csv'.format(str(bin_length), self.datetime))
+        self.roi_analyzer = ROIAnalyzer(ini_path=self.config_path, data_path=DirNames.OUTLIER_MOVEMENT_LOCATION.value, calculate_distances=False)
+        self.roi_analyzer.run()
+        self.shape_names = self.roi_analyzer.shape_names
+        self.animal_names = list(self.roi_analyzer.bp_dict.keys())
+        self.entries_exits_df = self.roi_analyzer.detailed_df
 
     def run(self):
-        """
-        Method to run movement aggregation computations.
-
-        Returns
-        ----------
-        Attribute: dict
-            results
-
-        """
-        self.results = {}
-        self.movement_dict = {}
-        for file_path in self.files_found:
-            _, video_name, _ = get_fn_ext(file_path)
-            print('Analysing {}...'.format(video_name))
-            self.data_df = read_df(file_path, self.file_type)[self.bp_columns]
-            self.video_info, self.px_per_mm, self.fps = self.read_video_info(video_name=video_name)
-            self.results[video_name] = {}
-            self.movement_dict[video_name] = {}
-            for animal_name, animal_bps in self.bp_dict.items():
-                self.results[video_name][animal_name] = {}
-                animal_df = self.data_df[animal_bps]
-                if self.p_threshold > 0.00:
-                    animal_df = animal_df[animal_df[animal_bps[2]] >= self.p_threshold]
-                animal_df = animal_df.iloc[:, 0:2].reset_index(drop=True)
-                df_shifted = animal_df.shift(1)
-                df_shifted = df_shifted.combine_first(animal_df).add_suffix('_shifted')
-                animal_df = pd.concat([animal_df, df_shifted], axis=1)
-                bp_time_1 = animal_df[[animal_bps[0], animal_bps[1]]].values.astype(float)
-                bp_time_2 = animal_df[[animal_bps[0] + '_shifted', animal_bps[1] + '_shifted']].values.astype(float)
-                self.movement = pd.Series(self.framewise_euclidean_distance(location_1=bp_time_1, location_2=bp_time_2, px_per_mm=self.px_per_mm))
-                self.movement.loc[0] = 0
-                self.movement_dict[video_name][animal_name] = self.movement
-                self.results[video_name][animal_name]['Distance (cm)'] = round((self.movement.sum() / 10), 4)
-                velocity_lst = []
-                for df in np.array_split(self.movement, int(len(self.movement) / self.fps)):
-                    velocity_lst.append(df.sum())
-                self.results[video_name][animal_name]['Velocity (cm/s)'] = round((mean(velocity_lst) / 10), 4)
+        self.files_found = self.roi_analyzer.files_found
+        self.out_dict_time, self.out_dict_entries = {}, {}
+        print('Analyzing time-bin data for {} videos...'.format(str(len(self.files_found))))
+        for file_cnt, file_path in enumerate(self.files_found):
+            _, self.video_name, _ = get_fn_ext(filepath=file_path)
+            self.out_dict_time[self.video_name], self.out_dict_entries[self.video_name] = {}, {}
+            _, _, fps = self.read_video_info(video_name=self.video_name)
+            frames_per_bin = int(fps * self.bin_length)
+            video_frms = list(range(0, len(read_df(file_path=file_path, file_type=self.file_type))))
+            frame_bins = [video_frms[i * frames_per_bin:(i + 1) * frames_per_bin] for i in range((len(video_frms) + frames_per_bin - 1) // frames_per_bin )]
+            self.video_data = self.entries_exits_df[self.entries_exits_df['VIDEO'] == self.video_name]
+            for animal_name, shape_name in list(itertools.product(self.animal_names, self.shape_names)):
+                self.results_time, self.results_entries = {}, {}
+                self.results_time[shape_name], self.results_entries[shape_name] = {}, {}
+                self.results_time[shape_name][animal_name], self.results_entries[shape_name][animal_name] = {}, {}
+                data_df = self.video_data.loc[(self.video_data['SHAPE'] == shape_name) & (self.video_data['ANIMAL'] == animal_name)]
+                entry_frms = list(data_df['ENTRY FRAMES'])
+                inside_shape_frms = [list(range(x, y)) for x, y in zip(list(data_df['ENTRY FRAMES'].astype(int)), list(data_df['EXIT FRAMES'].astype(int) + 1))]
+                inside_shape_frms = [i for s in inside_shape_frms for i in s]
+                for bin_cnt, bin_frms in enumerate(frame_bins):
+                    frms_inside_roi_in_timebin = [x for x in inside_shape_frms if x in bin_frms]
+                    entry_roi_in_timebin = [x for x in entry_frms if x in bin_frms]
+                    self.results_time[shape_name][animal_name][bin_cnt] = len(frms_inside_roi_in_timebin) / fps
+                    self.results_entries[shape_name][animal_name][bin_cnt] = len(entry_roi_in_timebin)
+                self.out_dict_time[self.video_name].update(self.results_time)
+                self.out_dict_entries[self.video_name].update(self.results_entries)
 
     def save(self):
-        """
-        Method to save movement aggregation data into the `project_folder/logs` directory
-        of the SimBA project.
-
-        Returns
-        ----------
-        None
-
-        """
-
-        self.out_df = pd.DataFrame(columns=['Video', 'Animal', 'Measurement', 'Value'])
-        for video, video_data in self.results.items():
-            for animal, animal_data in video_data.items():
-                for measure, mesure_val in animal_data.items():
-                    self.out_df.loc[len(self.out_df)] = [video, animal, measure, mesure_val]
-        self.out_df.set_index('Video').to_csv(self.save_path)
+        results_time_df = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'TIME INSIDE SHAPE (S)'])
+        results_entries_df = pd.DataFrame(columns=['VIDEO', 'SHAPE', 'ANIMAL', 'TIME BIN', 'ENTRY COUNT'])
+        for video_name, video_data in self.out_dict_time.items():
+            for shape_name, shape_data in video_data.items():
+                for animal_name, animal_data in shape_data.items():
+                    for bin_name, bin_data in animal_data.items():
+                        results_time_df.loc[len(results_time_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
+        results_time_df['TIME INSIDE SHAPE (S)'] = results_time_df['TIME INSIDE SHAPE (S)'].round(6)
+        results_time_df.to_csv(self.save_path_time)
+        stdout_success(msg=f'ROI time bin time data saved at {self.save_path_time}')
+        for video_name, video_data in self.out_dict_entries.items():
+            for shape_name, shape_data in video_data.items():
+                for animal_name, animal_data in shape_data.items():
+                    for bin_name, bin_data in animal_data.items():
+                        results_entries_df.loc[len(results_entries_df)] = [video_name, shape_name, animal_name, bin_name, bin_data]
+        results_entries_df.to_csv(self.save_path_entries)
         self.timer.stop_timer()
-        stdout_success(msg= f'Movement log saved in {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'ROI time bin entry data saved at {self.save_path_entries}', elapsed_time=self.timer.elapsed_time_str)
+
 
-#test = MovementProcessor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
-# test.process_movement()
+# test = ROITimebinCalculator(config_path='/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini',bin_length=5)
+# test.analyze_time_bins()
 # test.save_results()
+
+
+# test = ROITimebinCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",bin_length=5)
+# test.run()
+# test.save_results()
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.58.6/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.58.6/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.58.6/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.58.6/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     `ROI tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial_new.md>`__.
 
     Examples
     ----------
     >>> settings = {'body_parts': {'Simon': 'Ear_left_1', 'JJ': 'Ear_left_2'}, 'threshold': 0.4}
     >>> roi_analyzer = ROIAnalyzer(ini_path='MyProjectConfig', data_path='outlier_corrected_movement_location', settings=settings, calculate_distances=True)
     >>> roi_analyzer.run()
-    >>> roi_analyzer.save_data()
+    >>> roi_analyzer.save()
     """
 
     def __init__(self,
                  ini_path: str,
                  data_path: str or None,
                  settings: dict or None = None,
                  calculate_distances: bool = False):
@@ -82,15 +82,18 @@
 
     def __check_that_roi_config_data_is_valid(self):
         all_bps = list(set([x[:-2] for x in self.bp_headers]))
         self.roi_bp_config = {}
         for k, v in self.roi_config.items():
             if ''.join([i for i in k if not i.isdigit()]) == 'animal__bp':
                 id = int(''.join(c for c in k if c.isdigit())) - 1
-                self.roi_bp_config[self.multi_animal_id_list[id]] = v
+                try:
+                    self.roi_bp_config[self.multi_animal_id_list[id]] = v
+                except:
+                    pass
         for animal, bp in self.roi_bp_config.items():
             if bp not in all_bps:
                 raise BodypartColumnNotFoundError(msg=f'Project config setting [{ConfigKey.ROI_SETTINGS.value}][{animal}] is not a valid body-part. Please make sure you have analyzed ROI data.')
 
     def __get_bouts(self, lst=None):
         lst=list(lst)
         return lst[0], lst[-1]
@@ -251,15 +254,15 @@
             self.movements_df = pd.DataFrame(columns=['VIDEO', 'ANIMAL', 'SHAPE', 'MOVEMENT INSIDE SHAPE (CM)'])
             for video_name, video_data in self.movement_dict.items():
                 for animal_name, animal_data in video_data.items():
                     for shape_name, shape_data in animal_data.items():
                         self.movements_df.loc[len(self.movements_df)] = [video_name, animal_name, shape_name, shape_data]
             self.movements_df['ANIMAL'] = self.movements_df['ANIMAL'].map(self.body_part_to_animal_lookup)
 
-    def save_data(self):
+    def save(self):
         """
         Method to save ROI data to disk. ROI latency and ROI entry data is saved in the "project_folder/logs/" directory.
         If ``calculate_distances`` is True, ROI movement data is saved in the "project_folder/logs/" directory.
 
         Returns
         -------
         None
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.58.6/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/madlc_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/misc/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/misc/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.58.6/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.58.6/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.58.6/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.58.6/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/SimBA.py` & `Simba-UW-tf-dev-1.58.6/simba/SimBA.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,19 @@
 from simba.roi_tools.ROI_reset import *
 from simba.utils.read_write import get_video_meta_data
 from simba.utils.data import run_user_defined_feature_extraction_class
 from simba.utils.printing import stdout_success, stdout_warning
 from simba.video_processors.video_processing import (video_to_greyscale,
                                                      superimpose_frame_count,
                                                      extract_frames_from_all_videos_in_directory)
-from simba.ui.setting_menu import SettingsMenu
+from simba.ui.pop_ups.roi_analysis_time_bins_pop_up import ROIAnalysisTimeBinsPopUp
+from simba.ui.pop_ups.movement_analysis_pop_up import MovementAnalysisPopUp
+from simba.ui.pop_ups.roi_analysis_pop_up import ROIAnalysisPopUp
+from simba.ui.pop_ups.append_roi_features_animals_pop_up import AppendROIFeaturesByAnimalPopUp
+from simba.ui.pop_ups.movement_analysis_time_bins_pop_up import MovementAnalysisTimeBinsPopUp
 from simba.ui.pop_ups.heatmap_location_pop_up import HeatmapLocationPopup
 from simba.ui.pop_ups.quick_path_plot_pop_up import QuickLineplotPopup
 from simba.ui.pop_ups.clf_by_roi_pop_up import ClfByROIPopUp
 from simba.ui.pop_ups.fsttc_pop_up import FSTTCPopUp
 from simba.ui.pop_ups.kleinberg_pop_up import KleinbergPopUp
 from simba.ui.pop_ups.clf_by_timebins_pop_up import TimeBinsClfPopUp
 from simba.ui.pop_ups.clf_descriptive_statistics_pop_up import ClfDescriptiveStatsPopUp
@@ -226,16 +230,16 @@
         self.delete_all_ROIs.image = self.btn_icons['trash']['img']
 
         self.new_ROI_frm.grid(row=0, sticky=NW)
         self.start_new_ROI.grid(row=0, sticky=NW)
         self.delete_all_ROIs.grid(row=1, column=0, sticky=NW)
 
         self.roi_draw = LabelFrame(tab6, text='ANALYZE ROI DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value)
-        analyze_roi_btn = Button(self.roi_draw, text='ANALYZE ROI DATA: AGGREGATES', fg='green', command=lambda: SettingsMenu(config_path=self.config_path, title='ROI ANALYSIS'))
-        analyze_roi_time_bins_btn = Button(self.roi_draw, text='ANALYZE ROI DATA: TIME-BINS',  fg='blue', command=lambda: SettingsMenu(config_path=self.config_path, title='TIME BINS: ANALYZE ROI'))
+        analyze_roi_btn = Button(self.roi_draw, text='ANALYZE ROI DATA: AGGREGATES', fg='green', command=lambda: ROIAnalysisPopUp(config_path=self.config_path))
+        analyze_roi_time_bins_btn = Button(self.roi_draw, text='ANALYZE ROI DATA: TIME-BINS',  fg='blue', command=lambda: ROIAnalysisTimeBinsPopUp(config_path=self.config_path))
 
         self.roi_draw.grid(row=0, column=1, sticky=N)
         analyze_roi_btn.grid(row=0, sticky='NW')
         analyze_roi_time_bins_btn.grid(row=1, sticky='NW')
 
         ###plot roi
         self.roi_draw1 = LabelFrame(tab6, text='VISUALIZE ROI DATA', font=Formats.LABELFRAME_HEADER_FORMAT.value)
@@ -246,16 +250,16 @@
 
         ##organize
         self.roi_draw1.grid(row=0, column=2, sticky=N)
         visualizeROI.grid(row=0, sticky='NW')
         visualizeROIfeature.grid(row=1, sticky='NW')
 
         processmovementdupLabel = LabelFrame(tab6,text='OTHER ANALYSES / VISUALIZATIONS', font=Formats.LABELFRAME_HEADER_FORMAT.value)
-        analyze_distances_velocity_btn = Button(processmovementdupLabel, text='ANALYZE DISTANCES / VELOCITY: AGGREGATES', fg='green', command=lambda: SettingsMenu(config_path=self.config_path, title='ANALYZE MOVEMENT'))
-        analyze_distances_velocity_timebins_btn = Button(processmovementdupLabel, text='ANALYZE DISTANCES / VELOCITY: TIME-BINS', fg='blue', command=lambda: SettingsMenu(config_path=self.config_path, title='TIME BINS: DISTANCE/VELOCITY'))
+        analyze_distances_velocity_btn = Button(processmovementdupLabel, text='ANALYZE DISTANCES / VELOCITY: AGGREGATES', fg='green', command=lambda: MovementAnalysisPopUp(config_path=self.config_path))
+        analyze_distances_velocity_timebins_btn = Button(processmovementdupLabel, text='ANALYZE DISTANCES / VELOCITY: TIME-BINS', fg='blue', command=lambda: MovementAnalysisTimeBinsPopUp(config_path=self.config_path))
 
         heatmaps_location_button = Button(processmovementdupLabel,text='CREATE LOCATION HEATMAPS', fg='red', command=lambda: HeatmapLocationPopup(config_path=self.config_path))
 
         button_lineplot = Button(processmovementdupLabel, text='CREATE PATH PLOTS', fg='orange', command=lambda: QuickLineplotPopup(config_path=self.config_path))
         button_analyzeDirection = Button(processmovementdupLabel,text='ANALYZE DIRECTIONALITY BETWEEN ANIMALS', fg='pink', command =lambda: self.directing_other_animals_analysis())
         button_visualizeDirection = Button(processmovementdupLabel,text='VISUALIZE DIRECTIONALITY BETWEEN ANIMALS', fg='brown', command=lambda:self.directing_other_animals_visualizer())
 
@@ -291,16 +295,15 @@
         labelframe_usrdef = LabelFrame(label_extractfeatures)
         self.scriptfile = FileSelect(labelframe_usrdef, 'Script path')
         self.scriptfile.btnFind.configure(state='disabled')
         self.user_defined_var = BooleanVar(value=False)
         userscript = Checkbutton(labelframe_usrdef,text='Apply user-defined feature extraction script',variable=self.user_defined_var, command=lambda: activate(self.user_defined_var, self.scriptfile.btnFind))
 
         roi_feature_frm = CreateLabelFrameWithIcon(parent=tab5, header='APPEND ROI FEATURES', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.APPEND_ROI_FEATURES.value)
-        #roi_feature_frm = LabelFrame(tab5, text='APPEND ROI FEATURES', pady=5, font=Formats.LABELFRAME_HEADER_FORMAT.value)
-        append_roi_features_by_animal = Button(roi_feature_frm, text='APPEND ROI DATA TO FEATURES: BY ANIMAL (CAUTION)', fg='red',command=lambda: SettingsMenu(config_path=self.config_path, title='APPEND ROI FEATURES'))
+        append_roi_features_by_animal = Button(roi_feature_frm, text='APPEND ROI DATA TO FEATURES: BY ANIMAL (CAUTION)', fg='red',command=lambda: AppendROIFeaturesByAnimalPopUp(config_path=self.config_path))
         append_roi_features_by_body_part = Button(roi_feature_frm, text='APPEND ROI DATA TO FEATURES: BY BODY-PARTS (CAUTION)', fg='orange',command=lambda: AppendROIFeaturesByBodyPartPopUp(config_path=self.config_path))
 
         feature_tools_frm = LabelFrame(tab5, text='FEATURE TOOLS', pady=5, font=Formats.LABELFRAME_HEADER_FORMAT.value)
         compute_feature_subset_btn = Button(feature_tools_frm, text='CALCULATE FEATURE SUBSETS', fg='blue',command=lambda: FeatureSubsetExtractorPopUp(config_path=self.config_path))
 
         label_behavior_frm = CreateLabelFrameWithIcon(parent=tab7, header='LABEL BEHAVIOR', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.LABEL_BEHAVIOR.value)
         #label_behavior_frm = LabelFrame(tab7,text='LABEL BEHAVIOR',font=Formats.LABELFRAME_HEADER_FORMAT.value,pady=5,padx=5,fg='black')
@@ -377,55 +380,42 @@
         button_runmachinemodel = Button(label_runmachinemodel,text='RUN MODELS', fg='green', compound='left', image=self.btn_icons['clf']['img'], command=self.runrfmodel)
         button_runmachinemodel.image = self.btn_icons['clf']['img']
 
         kleinberg_button = Button(label_runmachinemodel,text='KLEINBERG SMOOTHING', fg='green', command=lambda: KleinbergPopUp(config_path=self.config_path))
         fsttc_button = Button(label_runmachinemodel,text='FSTTC', fg='green', command=lambda:FSTTCPopUp(config_path=self.config_path))
 
         label_machineresults = CreateLabelFrameWithIcon(parent=tab9, header='ANALYZE MACHINE RESULTS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.ANALYZE_ML_RESULTS.value)
-        #label_machineresults = LabelFrame(tab9,text='ANALYZE MACHINE RESULTS',font=Formats.LABELFRAME_HEADER_FORMAT.value,padx=5,pady=5,fg='black')
         button_process_datalog = Button(label_machineresults, text='ANALYZE MACHINE PREDICTIONS: AGGREGATES', fg='blue', command=lambda: ClfDescriptiveStatsPopUp(config_path=self.config_path))
-        button_process_movement = Button(label_machineresults, text='ANALYZE DISTANCES/VELOCITY: AGGREGATES', fg='blue', command=lambda: SettingsMenu(config_path=self.config_path, title='ANALYZE MOVEMENT'))
-        button_movebins = Button(label_machineresults, text='ANALYZE DISTANCES/VELOCITY: TIME BINS', fg='blue', command=lambda: SettingsMenu(config_path=self.config_path, title='TIME BINS: DISTANCE/VELOCITY'))
+        button_process_movement = Button(label_machineresults, text='ANALYZE DISTANCES/VELOCITY: AGGREGATES', fg='blue', command=lambda: MovementAnalysisPopUp(config_path=self.config_path))
+        button_movebins = Button(label_machineresults, text='ANALYZE DISTANCES/VELOCITY: TIME BINS', fg='blue', command=lambda: MovementAnalysisTimeBinsPopUp(config_path=self.config_path))
         button_classifierbins = Button(label_machineresults,text='ANALYZE MACHINE PREDICTIONS: TIME-BINS', fg='blue', command=lambda: TimeBinsClfPopUp(config_path=self.config_path))
         button_classifier_ROI = Button(label_machineresults, text='ANALYZE MACHINE PREDICTION: BY ROI', fg='blue', command=lambda: ClfByROIPopUp(config_path=self.config_path))
         button_severity = Button(label_machineresults, text='ANALYZE MACHINE PREDICTION: BY SEVERITY', fg='blue', command=lambda: AnalyzeSeverityPopUp(config_path=self.config_path))
 
 
         visualization_frm = CreateLabelFrameWithIcon(parent=tab10, header='DATA VISUALIZATIONS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VISUALIZATION.value)
-        #visualization_frm = LabelFrame(tab10,text='DATA VISUALIZATIONS',font=Formats.LABELFRAME_HEADER_FORMAT.value,pady=5,padx=5,fg='black')
         sklearn_visualization_btn = Button(visualization_frm,text='VISUALIZE CLASSIFICATIONS', fg='black',command= lambda:SklearnVisualizationPopUp(config_path=self.config_path))
         sklearn_visualization_btn.grid(row=0, column=0, sticky=NW)
-
         gantt_visualization_btn = Button(visualization_frm,text='VISUALIZE GANTT', fg='blue', command=lambda:GanttPlotPopUp(config_path=self.config_path))
         gantt_visualization_btn.grid(row=1, column=0, sticky=NW)
-
         probability_visualization_btn = Button(visualization_frm,text='VISUALIZE PROBABILITIES', fg='green', command=lambda:VisualizeClassificationProbabilityPopUp(config_path=self.config_path))
         probability_visualization_btn.grid(row=2, column=0, sticky=NW)
-
         path_visualization_btn = Button(visualization_frm, text='VISUALIZE PATHS', fg='orange', command=lambda: PathPlotPopUp(config_path=self.config_path))
         path_visualization_btn.grid(row=3, column=0, sticky=NW)
-
         distance_visualization_btn = Button(visualization_frm, text='VISUALIZE DISTANCES', fg='red', command=lambda: DistancePlotterPopUp(config_path=self.config_path))
         distance_visualization_btn.grid(row=4, column=0, sticky=NW)
-
         heatmap_clf_visualization_btn = Button(visualization_frm, text='VISUALIZE CLASSIFICATION HEATMAPS', fg='pink', command=lambda: HeatmapClfPopUp(config_path=self.config_path))
         heatmap_clf_visualization_btn.grid(row=5, column=0, sticky=NW)
-
         data_plot_visualization_btn = Button(visualization_frm, text='VISUALIZE DATA PLOTS', fg='purple',command=lambda: DataPlotterPopUp(config_path=self.config_path))
         data_plot_visualization_btn.grid(row=6, column=0, sticky=NW)
-
         clf_validation_btn = Button(visualization_frm, text='CLASSIFIER VALIDATION CLIPS', fg='blue', command=lambda: ClassifierValidationPopUp(config_path=self.config_path))
         clf_validation_btn.grid(row=7, column=0, sticky=NW)
-
         merge_frm = CreateLabelFrameWithIcon(parent=tab10, header='MERGE FRAMES', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.CONCAT_VIDEOS.value)
-        #merge_frm = LabelFrame(tab10, text='MERGE FRAMES', pady=5, padx=5, font=("Helvetica", 12, 'bold'), fg='black')
         merge_frm_btn = Button(merge_frm, text='MERGE FRAMES', fg='black', command=lambda:ConcatenatorPopUp(config_path=self.config_path))
-
         plotlyInterface = CreateLabelFrameWithIcon(parent=tab10, header='PLOTLY / DASH', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.PLOTLY.value)
-        #plotlyInterface = LabelFrame(tab10, text= 'PLOTLY / DASH', font=("Helvetica", 12, 'bold'), pady=5, padx=5, fg='black')
         plotlyInterfaceTitles = ['Sklearn results', 'Time bin analyses', 'Probabilities', 'Severity analysis']
         toIncludeVar = []
         for i in range(len(plotlyInterfaceTitles)+1):
             toIncludeVar.append(IntVar())
         plotlyCheckbox = [0] * (len(plotlyInterfaceTitles)+1)
         for i in range(len(plotlyInterfaceTitles)):
             plotlyCheckbox[i] = Checkbutton(plotlyInterface, text=plotlyInterfaceTitles[i], variable=toIncludeVar[i])
```

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.58.6/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.58.6/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.58.6/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.58.6/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.58.6/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.58.6/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.58.6/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.58.6/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.58.6/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.58.6/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.58.6/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.58.6/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.58.6/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.58.6/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.58.6/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.58.6/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.58.5
+Version: 1.58.6
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -338,20 +338,20 @@
 simba/third_party_label_appenders/observer_importer.py
 simba/third_party_label_appenders/solomon_importer.py
 simba/third_party_label_appenders/third_party_appender.py
 simba/third_party_label_appenders/tools.py
 simba/ui/.DS_Store
 simba/ui/create_project_ui.py
 simba/ui/machine_model_settings_ui.py
-simba/ui/setting_menu.py
 simba/ui/tkinter_functions.py
 simba/ui/user_defined_pose_creator.py
 simba/ui/video_info_ui.py
 simba/ui/pop_ups/.DS_Store
 simba/ui/pop_ups/about_simba_pop_up.py
+simba/ui/pop_ups/append_roi_features_animals_pop_up.py
 simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
 simba/ui/pop_ups/archive_files_pop_up.py
 simba/ui/pop_ups/batch_preprocess_pop_up.py
 simba/ui/pop_ups/clf_add_remove_print_pop_up.py
 simba/ui/pop_ups/clf_by_roi_pop_up.py
 simba/ui/pop_ups/clf_by_timebins_pop_up.py
 simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
@@ -365,20 +365,24 @@
 simba/ui/pop_ups/distance_plot_pop_up.py
 simba/ui/pop_ups/fsttc_pop_up.py
 simba/ui/pop_ups/gantt_pop_up.py
 simba/ui/pop_ups/heatmap_clf_pop_up.py
 simba/ui/pop_ups/heatmap_location_pop_up.py
 simba/ui/pop_ups/kleinberg_pop_up.py
 simba/ui/pop_ups/make_path_plot_pop_up.py
+simba/ui/pop_ups/movement_analysis_pop_up.py
+simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
 simba/ui/pop_ups/outlier_settings_pop_up.py
 simba/ui/pop_ups/path_plot_pop_up.py
 simba/ui/pop_ups/pose_bp_drop_pop_up.py
 simba/ui/pop_ups/pose_reorganizer_pop_up.py
 simba/ui/pop_ups/pup_retrieval_pop_up.py
 simba/ui/pop_ups/quick_path_plot_pop_up.py
+simba/ui/pop_ups/roi_analysis_pop_up.py
+simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
 simba/ui/pop_ups/roi_features_plot_pop_up.py
 simba/ui/pop_ups/roi_tracking_plot_pop_up.py
 simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
 simba/ui/pop_ups/severity_analysis_pop_up.py
 simba/ui/pop_ups/smoothing_interpolation_pop_up.py
 simba/ui/pop_ups/subset_feature_extractor_pop_up.py
 simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
```

### Comparing `Simba-UW-tf-dev-1.58.5/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.58.6/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/LICENSE.md` & `Simba-UW-tf-dev-1.58.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/README.md` & `Simba-UW-tf-dev-1.58.6/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.58.5/setup.py` & `Simba-UW-tf-dev-1.58.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.58.5",
+    version="1.58.6",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

