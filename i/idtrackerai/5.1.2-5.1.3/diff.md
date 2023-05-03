# Comparing `tmp/idtrackerai-5.1.2.tar.gz` & `tmp/idtrackerai-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idtrackerai-5.1.2.tar", last modified: Wed Apr 26 11:46:31 2023, max compression
+gzip compressed data, was "idtrackerai-5.1.3.tar", last modified: Wed May  3 10:34:26 2023, max compression
```

## Comparing `idtrackerai-5.1.2.tar` & `idtrackerai-5.1.3.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.2/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1597 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3079 2023-04-26 11:36:15.000000 idtrackerai-5.1.2/pyproject.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/setup.cfg
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.671650 idtrackerai-5.1.2/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.671650 idtrackerai-5.1.2/src/idmatcherai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idmatcherai/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     9092 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idmatcherai/main.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3678 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idmatcherai/matcher.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.671650 idtrackerai-5.1.2/src/idtrackerai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/animals_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/animals_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/animals_detection/animals_detection.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15562 2023-04-26 11:34:40.000000 idtrackerai-5.1.2/src/idtrackerai/animals_detection/segmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31737 2023-04-26 11:35:45.000000 idtrackerai-5.1.2/src/idtrackerai/blob.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-04-24 13:20:28.000000 idtrackerai-5.1.2/src/idtrackerai/constants.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7524 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3144 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossings_detection.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7286 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5057 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/model_area.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:28.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      761 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5415 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4174 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.683650 idtrackerai-5.1.2/src/idtrackerai/data/
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-03-20 08:48:28.000000 idtrackerai-5.1.2/src/idtrackerai/data/test_A.avi
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/data/test_B.avi
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    25591 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/fragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/fragmentation/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/fragmentation/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/fragmentation/fragmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8913 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/globalfragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15885 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/list_of_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    23986 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/list_of_fragments.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13045 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/list_of_global_fragments.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      456 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4271 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/network/evaluate.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/learners.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1878 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/network_params.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4509 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/train.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8886 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/network/utils.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/postprocess/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27568 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/assign_them_all.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/compute_velocity_model.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21435 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3634 2023-04-26 11:34:55.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/erosion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8545 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/get_trajectories.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_creation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-26 09:35:16.000000 idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_to_csv.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.691650 idtrackerai-5.1.2/src/idtrackerai/tracker/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    36591 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-03-21 11:15:37.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8680 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/accumulator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4270 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/assigner.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3700 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5432 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/identity_transfer.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai/tracker/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1452 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/get_predictions.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/stop_training_criteria.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5035 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/network/trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7147 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/pre_trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    34367 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/tracker/tracker.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1144 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai/utils/check_PyPI_version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai/utils/confparams.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2990 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/utils/init_logger.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12519 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/utils/py_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    33060 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai/video.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.675650 idtrackerai-5.1.2/src/idtrackerai.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5669 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      371 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-04-26 11:46:31.000000 idtrackerai-5.1.2/src/idtrackerai.egg-info/top_level.txt
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6097 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/GUI_main_base.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/logo_256.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-04-12 07:40:32.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/themes.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5909 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_start_app/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4975 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-04-24 13:20:28.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/all_valid_parameters.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-04-24 13:20:28.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/arg_parser.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5405 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/run_idtrackerai.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16140 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.695651 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5827 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6625 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_start_app/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/src/idtrackerai_validator/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_validator/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-03-20 08:48:29.000000 idtrackerai-5.1.2/src/idtrackerai_validator/tooltips.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31781 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      425 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/errors_explorer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_groups.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-03-21 11:17:49.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_labels.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12940 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/interpolator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6246 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/paint_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/setup_points.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-26 11:46:31.699651 idtrackerai-5.1.2/src/idtrackerai_video/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_video/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6020 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_video/general_video.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4866 2023-04-12 10:06:11.000000 idtrackerai-5.1.2/src/idtrackerai_video/individual_videos.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2092 2023-04-26 09:35:10.000000 idtrackerai-5.1.2/src/idtrackerai_video/main.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-04-19 16:31:58.000000 idtrackerai-5.1.3/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1597 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3079 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/pyproject.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/setup.cfg
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idmatcherai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idmatcherai/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9092 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idmatcherai/main.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3678 2023-05-03 10:01:42.000000 idtrackerai-5.1.3/src/idmatcherai/matcher.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/animals_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/animals_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/animals_detection/animals_detection.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15562 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/animals_detection/segmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31737 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/blob.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/constants.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7524 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3144 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossings_detection.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7286 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5057 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/model_area.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.573556 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      761 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5415 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4174 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.573556 idtrackerai-5.1.3/src/idtrackerai/data/
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/data/test_A.avi
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/data/test_B.avi
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    26226 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/fragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/fragmentation/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/fragmentation/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/fragmentation/fragmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8913 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/globalfragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15885 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/list_of_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    23949 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/list_of_fragments.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13045 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/list_of_global_fragments.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      456 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4271 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/network/evaluate.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/learners.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1878 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/network_params.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4509 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/train.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8886 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/utils.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/postprocess/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27568 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/assign_them_all.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/compute_velocity_model.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    21435 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3634 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/erosion.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8545 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/get_trajectories.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_creation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_to_csv.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/tracker/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    36591 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8680 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/accumulator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4270 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/assigner.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3700 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5432 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/identity_transfer.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/tracker/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1452 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/get_predictions.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/stop_training_criteria.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5035 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7147 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/pre_trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    34367 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/tracker.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1144 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/utils/check_PyPI_version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/utils/confparams.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2990 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/utils/init_logger.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12515 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/utils/py_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    33048 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/video.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5732 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      371 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6154 2023-05-03 10:04:54.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/GUI_main_base.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/logo_256.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/themes.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5909 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-03 10:01:51.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_start_app/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4975 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/all_valid_parameters.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/arg_parser.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5405 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/run_idtrackerai.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16140 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5827 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6625 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_validator/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_validator/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/tooltips.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    30957 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      491 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1752 2023-05-03 10:06:36.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/additional_info.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/errors_explorer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_groups.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_labels.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12940 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/interpolator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6246 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/paint_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/setup_points.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/src/idtrackerai_video/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_video/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5289 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_video/general_video.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4110 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_video/individual_videos.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2961 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.1.2/LICENSE` & `idtrackerai-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/PKG-INFO` & `idtrackerai-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.2
+Version: 5.1.3
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.2/README.md` & `idtrackerai-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/pyproject.toml` & `idtrackerai-5.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "idtrackerai"
-version = "5.1.2"
+version = "5.1.3"
 authors = [
     { name = "Jordi Torrents", email = "jordi.torrentsm@gmail.com" },
     { name = "Francisco Romero Ferrero" },
     { name = "Mattia G. Bergomi" },
     { name = "Francisco J.H. Heras" },
     { name = "Ricardo Ribeiro" },
 ]
```

### Comparing `idtrackerai-5.1.2/src/idmatcherai/main.py` & `idtrackerai-5.1.3/src/idmatcherai/main.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idmatcherai/matcher.py` & `idtrackerai-5.1.3/src/idmatcherai/matcher.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/__init__.py` & `idtrackerai-5.1.3/src/idtrackerai/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/animals_detection/animals_detection.py` & `idtrackerai-5.1.3/src/idtrackerai/animals_detection/animals_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/animals_detection/segmentation.py` & `idtrackerai-5.1.3/src/idtrackerai/animals_detection/segmentation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/blob.py` & `idtrackerai-5.1.3/src/idtrackerai/blob.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 from functools import cached_property
 from itertools import chain
 from math import atan2, sqrt
 from pathlib import Path
+from typing import Sequence
 
 import cv2
 import h5py
 import numpy as np
 
 
 class Blob:
@@ -351,19 +352,18 @@
         points = other.contour.astype(float)
         for point in chain(points[0::3], points[1::3], points[2::3]):
             if self.contour_contains_point(point):
                 return True
 
         # Check for every point in `self`'s contour
         points = self.contour.astype(float)
-        for point in chain(points[0::3], points[1::3], points[2::3]):
-            if other.contour_contains_point(point):
-                return True
-
-        return False
+        return any(
+            other.contour_contains_point(point)
+            for point in chain(points[0::3], points[1::3], points[2::3])
+        )
 
     def contour_contains_point(self, point: tuple[float, float]) -> bool:
         return cv2.pointPolygonTest(self.contour, point, False) >= 0
 
     def bbox_contains_point(self, point: tuple[float, float]) -> bool:
         return (
             point[0] >= self.bbox_in_frame_coordinates[0][0]
@@ -837,17 +837,19 @@
             except ValueError:  # centroid not found on "current"
                 continue
             blobs_stack += [(prev_blob, new_centroid) for prev_blob in current.previous]
             first_frame_modified = current.frame_number
 
         return first_frame_modified, last_frame_modified
 
-    def __str__(self):
-        out = [
-            ("Individual" if self.is_an_individual else "Crossing") + " Blob",
+    @property
+    def properties(self) -> Sequence[str]:
+        return (
+            ("Individual" if self.is_an_individual else "Crossing")
+            + f" Blob ({hex(id(self))})",
             f"{self.contour.shape[0]} vertices in contour of {self.area:.0f} px area",
             ("Used" if self.used_for_training else "Not used") + " for training",
             f"In fragment {self.fragment_identifier}",
             f"Linked to {len(self.previous)} previous blobs",
             f"Linked to {len(self.next)} next blobs",
             ("Used" if self.used_for_training_crossings else "Not used")
             + " for training crossings",
@@ -859,17 +861,15 @@
             f"Id correcting gaps: {self.identities_corrected_closing_gaps}",
             f"assigned identities: {self.assigned_identities}",
             f"assigned centroids: {repr_of_list_of_points(self.assigned_centroids)}",
             f"user identities: {self.user_generated_identities}",
             f"user centroids: {repr_of_list_of_points(self.user_generated_centroids)}",
             f"final identities: {self.final_identities}",
             f"final centroids: {repr_of_list_of_points(self.final_centroids)}",
-            f"Located in {hex(id(self))}",
-        ]
-        return "\n".join(out)
+        )
 
 
 def repr_of_list_of_points(list_of_points) -> str:
     if list_of_points is None:
         return "None"
     list_of_str = [
         f"({point[0]:.1f}, {point[1]:.1f})" if point is not None else "None"
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai/constants.toml` & `idtrackerai-5.1.3/src/idtrackerai/constants.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossing_detector.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/crossings_detection.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossings_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/model_area.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/model_area.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py` & `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/data/test_A.avi` & `idtrackerai-5.1.3/src/idtrackerai/data/test_A.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/data/test_B.avi` & `idtrackerai-5.1.3/src/idtrackerai/data/test_B.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/fragment.py` & `idtrackerai-5.1.3/src/idtrackerai/fragment.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import sys
+from typing import Sequence
 
 import numpy as np
 
 from .utils import conf
 
 
 class Fragment:
@@ -44,21 +45,14 @@
     fragment_identifier : int
         It uniquely identifies the fragment.
         It is also used to link blobs to fragments, as blobs have an attribute
         called `blob.Blob.fragment_identifier`.
     start_end : tuple
         Indicates the start and end of the fragment.
         The end is exclusive, i.e. follows Python standards.
-    blob_hierarchy_in_first_frame : int
-        Indicates the hierarchy in the blob in the first frame of the fragment.
-        The hierarchy is the order by which the function blob_extractor
-        (see segmentation_utils.py) extracts information about the blobs
-        of a frame.
-        This attribute was used to plot the accumulation steps figures of the
-        paper.
     images : list
         List of integers indicating the index of the identification image
         in the episode.
         This corresponds to the `identification_image_index` of the blob.
         Note that the images are stored in the identification_images folder
         inside of the session folder.
         Then the images are loaded using this index and the episode index.
@@ -172,25 +166,23 @@
     jumps. It has nothing to do with the manual validation."""
 
     def __init__(
         self,
         fragment_identifier: int,
         start_frame: int,
         end_frame: int,
-        blob_hierarchy_in_first_frame: int,
         images: list[int],
         centroids: list,
         episodes: list[int],
         is_an_individual: bool,
         number_of_animals: int,
     ):
         self.identifier = fragment_identifier
         self.start_frame = start_frame
         self.end_frame = end_frame
-        self.blob_hierarchy_in_first_frame = blob_hierarchy_in_first_frame
         self.images = images
         self.centroids = np.asarray(centroids)
         self.episodes = episodes
         self.is_an_individual = is_an_individual
         self.number_of_animals = number_of_animals
         self.distance_travelled = self.set_distance_travelled(self.centroids)
 
@@ -642,7 +634,31 @@
             Can be "global" or "partial"
 
         """
         if accumulation_strategy == "global":
             self.accumulated_globally = True
         elif accumulation_strategy == "partial":
             self.accumulated_partially = True
+
+    @property
+    def properties(self) -> Sequence[str]:
+        return (
+            f"Fragment {self.identifier}",
+            f"Frames from {self.start_frame} to {self.end_frame}",
+            ("Individual" if self.is_an_individual else "Crossing") + " fragment",
+            ("Used" if self.used_for_training else "Not used") + " for training",
+            ("Used" if self.used_for_pretraining else "Not used") + " for pretraining",
+            ("Acceptable" if self.acceptable_for_training else "Not acceptable")
+            + " for training",
+            f"{self.temporary_id}",
+            f"{self.identity}",
+            f"{self.identity_corrected_solving_jumps}",
+            f"{self.identity_is_fixed}",
+            f"{self.accumulated_globally}",
+            f"{self.accumulated_partially}",
+            f"{self.accumulation_step}",
+            f"{self.is_certain}",
+            "Non consistent" if self.non_consistent else "Consistent",
+            f"Certainty: {self.certainty}",
+            f"P1 vector: {self.P1_vector}",
+            f"P1 below random: {self.P1_below_random}",
+        )
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai/fragmentation/fragmentation.py` & `idtrackerai-5.1.3/src/idtrackerai/fragmentation/fragmentation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/globalfragment.py` & `idtrackerai-5.1.3/src/idtrackerai/globalfragment.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py` & `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py` & `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py` & `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_groundtruth.py` & `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py` & `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/list_of_blobs.py` & `idtrackerai-5.1.3/src/idtrackerai/list_of_blobs.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/list_of_fragments.py` & `idtrackerai-5.1.3/src/idtrackerai/list_of_fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,14 @@
 
                 end = current.frame_number
 
                 fragment = Fragment(
                     current_fragment_identifier,
                     start,
                     end + 1,  # it is not inclusive
-                    blob.blob_index,
                     images,
                     centroids,
                     episodes,
                     blob.is_an_individual,
                     number_of_animals,
                 )
                 used_fragment_identifiers.add(current_fragment_identifier)
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai/list_of_global_fragments.py` & `idtrackerai-5.1.3/src/idtrackerai/list_of_global_fragments.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/network/evaluate.py` & `idtrackerai-5.1.3/src/idtrackerai/network/evaluate.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/network/learners.py` & `idtrackerai-5.1.3/src/idtrackerai/network/learners.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/network/models.py` & `idtrackerai-5.1.3/src/idtrackerai/network/models.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/network/network_params.py` & `idtrackerai-5.1.3/src/idtrackerai/network/network_params.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/network/train.py` & `idtrackerai-5.1.3/src/idtrackerai/network/train.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/network/utils.py` & `idtrackerai-5.1.3/src/idtrackerai/network/utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/assign_them_all.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/assign_them_all.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/compute_velocity_model.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/compute_velocity_model.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/erosion.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/erosion.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/get_trajectories.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/get_trajectories.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_creation.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_creation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/postprocess/trajectories_to_csv.py` & `idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_to_csv.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/accumulation_manager_utils.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/accumulator.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/accumulator.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/assigner.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/assigner.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataloader.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataloader.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/dataset/identification_dataset.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataset.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/identity_transfer.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/identity_transfer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/network/get_predictions.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/network/get_predictions.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/network/stop_training_criteria.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/network/stop_training_criteria.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/network/trainer.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/network/trainer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/pre_trainer.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/pre_trainer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/tracker/tracker.py` & `idtrackerai-5.1.3/src/idtrackerai/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/utils/__init__.py` & `idtrackerai-5.1.3/src/idtrackerai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/utils/check_PyPI_version.py` & `idtrackerai-5.1.3/src/idtrackerai/utils/check_PyPI_version.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/utils/confparams.py` & `idtrackerai-5.1.3/src/idtrackerai/utils/confparams.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/utils/init_logger.py` & `idtrackerai-5.1.3/src/idtrackerai/utils/init_logger.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai/utils/py_utils.py` & `idtrackerai-5.1.3/src/idtrackerai/utils/py_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     # Create entire output array
     with h5py.File(id_images_file_paths[0], "r") as file:
         test_dataset = file["id_images"]
         images = np.empty(
             (len(images_indices), *test_dataset.shape[1:]), test_dataset.dtype
         )
 
-    for episode in track(set(episodes), "Loading identification images from the disk"):
+    for episode in track(set(episodes), "Loading identification images from disk"):
         where = episodes == episode
         with h5py.File(id_images_file_paths[episode], "r") as file:
             images[where] = file["id_images"][:][img_indices[where]]
 
     return images
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai/video.py` & `idtrackerai-5.1.3/src/idtrackerai/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,19 +618,19 @@
             candidate_new_video_paths = [
                 folder_candidate / path.name for path in self.video_paths
             ]
 
             try:
                 assert_all_files_exist(candidate_new_video_paths)
             except FileNotFoundError:
-                logging.info(f"Video files not found on {folder_candidate}")
-            else:
-                logging.info(f"All video files found on {folder_candidate}")
-                found = True
-                break
+                continue
+
+            logging.info(f"All video files found on {folder_candidate}")
+            found = True
+            break
         else:
             found = False
             logging.error(f"Video file paths not found: {self.video_paths}")
 
         need_to_save = False
         if self.session_folder != new_video_object_path:
             logging.info(
@@ -878,8 +878,9 @@
             ):
                 for key in original_file.keys():
                     compressed_file.create_dataset(
                         key,
                         data=original_file[key],
                         compression="gzip" if "image" in key else None,
                     )
+            path.unlink()  # Windows needs this call before rename()
             tmp_path.rename(path)
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai.egg-info/PKG-INFO` & `idtrackerai-5.1.3/src/idtrackerai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.2
+Version: 5.1.3
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai.egg-info/SOURCES.txt` & `idtrackerai-5.1.3/src/idtrackerai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
 src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
 src/idtrackerai_validator/__init__.py
 src/idtrackerai_validator/__main__.py
 src/idtrackerai_validator/tooltips.toml
 src/idtrackerai_validator/validation_GUI.py
 src/idtrackerai_validator/validator_widgets/__init__.py
+src/idtrackerai_validator/validator_widgets/additional_info.py
 src/idtrackerai_validator/validator_widgets/errors_explorer.py
 src/idtrackerai_validator/validator_widgets/id_groups.py
 src/idtrackerai_validator/validator_widgets/id_labels.py
 src/idtrackerai_validator/validator_widgets/interpolator.py
 src/idtrackerai_validator/validator_widgets/paint_blobs.py
 src/idtrackerai_validator/validator_widgets/setup_points.py
 src/idtrackerai_video/__init__.py
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/GUI_main_base.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/GUI_main_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
 
     def change_theme(self, dark_theme: bool):
         if dark_theme:
             QApplication.setPalette(dark)
         else:
             QApplication.setPalette(light)
 
+        self.setStyleSheet("QToolTip { color: black;}")
+
     def closeEvent(self, event: QCloseEvent):
         json.dump(
             {
                 "dark_theme": self.themeAction.isChecked(),
                 "fontsize": self.font().pointSize(),
             },
             self.json_path.open("w"),
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/__init__.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/logo_256.png` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/logo_256.png`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/themes.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/themes.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/tooltips.toml` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/canvas.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/canvas.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_GUI_tools/widgets_utils/video_player.py` & `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_player.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/__main__.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/__main__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/all_valid_parameters.dat` & `idtrackerai-5.1.3/src/idtrackerai_start_app/all_valid_parameters.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/arg_parser.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/run_idtrackerai.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/run_idtrackerai.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_GUI.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_GUI.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py` & `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_start_app/tooltips.toml` & `idtrackerai-5.1.3/src/idtrackerai_start_app/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/__main__.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/tooltips.toml` & `idtrackerai-5.1.3/src/idtrackerai_validator/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validation_GUI.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validation_GUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     QSpinBox,
     QSplitter,
     QTabWidget,
     QVBoxLayout,
     QWidget,
 )
 
-from idtrackerai import Blob, ListOfBlobs, Video
+from idtrackerai import Blob, ListOfBlobs, Video, ListOfFragments
 from idtrackerai.postprocess import (
     convert_trajectories_file_to_csv_and_json,
     produce_output_dict,
 )
 from idtrackerai.utils import resolve_path, track
 from idtrackerai_GUI_tools import (
     CanvasMouseEvent,
@@ -45,14 +45,15 @@
     IdGroups,
     IdLabels,
     Interpolator,
     SetupPoints,
     find_selected_blob,
     paintBlobs,
     paintTrails,
+    AdditionalInfo,
 )
 
 parent_dir = Path(idtrackerai_GUI_tools_file).parent
 for file in parent_dir.glob("cmap_*"):
     general_cmap = np.loadtxt(parent_dir / file, dtype=np.uint8)
 assert general_cmap is not None
 
@@ -133,26 +134,14 @@
 
         new_id = self.spinbox.value()
         if new_id == -1:
             new_id = None
         return answer, new_id, self.propagate.isChecked()
 
 
-class CustomListWidget(QListWidget):
-    def keyPressEvent(self, e: QKeyEvent):
-        event = key_event_modifier(e)
-        if event is not None:
-            super().keyPressEvent(event)
-
-    def keyReleaseEvent(self, e: QKeyEvent):
-        event = key_event_modifier(e)
-        if event is not None:
-            super().keyReleaseEvent(event)
-
-
 class ValidationGUI(GUIBase):
     def __init__(self, session_path: Path | None = None):
         super().__init__()
 
         # TODO logging.getLogger().addHandler(WarningRedirector(self))
 
         self.setWindowTitle("idtracker.ai | Validation GUI")
@@ -166,19 +155,14 @@
 
         self.video_player.canvas.click_event.connect(self.click_on_canvas)
         self.video_player.canvas.double_click_event.connect(self.double_click_on_canvas)
 
         def new_changes():
             self.unsaved_changes = True
 
-        self.info_widget = CustomListWidget()
-        self.info_widget.setAlternatingRowColors(True)
-        self.following_label = QLabel()
-        self.following_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
-
         self.id_groups = IdGroups(self)
         self.id_groups.needToDraw.connect(self.video_player.update)
         self.id_groups.unsaved_changes.connect(new_changes)
 
         self.errorsExplorer = ErrorsExplorer()
         self.errorsExplorer.go_to_error.connect(self.go_to_error)
 
@@ -200,28 +184,24 @@
         self.setup_points.needToDraw.connect(new_changes)
 
         self.video_player.canvas.click_event.connect(self.setup_points.click_event)
         self.video_player.canvas.click_event.connect(self.interpolator.click_event)
 
         right_splitter = QSplitter(Qt.Orientation.Vertical)
         right_splitter.setContentsMargins(8, 0, 0, 0)
-        info_layout = QVBoxLayout()
-        info_layout.setContentsMargins(0, 0, 0, 8)
-        info_widget = QWidget()
-        info_widget.setLayout(info_layout)
-        info_layout.addWidget(self.following_label)
-        info_layout.addWidget(self.info_widget)
+
+        self.additional_info = AdditionalInfo()
 
         tabs = QTabWidget()
         tabs.addTab(self.id_groups, "Groups")
         tabs.addTab(self.id_labels, "Labels")
         tabs.addTab(self.setup_points, "Setup Points")
         tabs.currentChanged.connect(self.video_player.update)
         right_splitter.addWidget(tabs)
-        right_splitter.addWidget(info_widget)
+        right_splitter.addWidget(self.additional_info)
         self.interpolator.enabled_changed.connect(
             lambda enabled: tabs.setEnabled(not enabled)
         )
 
         left_splitter = QVBoxLayout()
         left_splitter.addWidget(self.errorsExplorer)
         left_splitter.addWidget(QHLine())
@@ -470,14 +450,21 @@
             QMessageBox.warning(
                 self,
                 "Loading session error",
                 f"List of blobs not found on any of {blobs_paths_candidates}",
             )
             return
 
+        if video.fragments_path.is_file():
+            self.additional_info.list_of_fragments = ListOfFragments.load(
+                video.fragments_path
+            )
+        else:
+            self.additional_info.list_of_fragments = None
+
         self.video_player.update_video_paths(
             video.video_paths,
             video.number_of_frames,
             (video.original_width, video.original_height),
             video.frames_per_second,
             res_reduct=video.resolution_reduction,
         )
@@ -588,24 +575,14 @@
             assert self.selected_id is not None and self.selected_id > 0
             self.interpolator.set_interpolation_params(
                 self.selected_id,
                 self.current_frame_number,
                 self.current_frame_number + 1,
             )
 
-    def update_right_bar(self, blob: Blob | None):
-        self.info_widget.clear()
-        if blob is not None:
-            self.info_widget.addItems(str(blob).splitlines())
-        self.following_label.setText(
-            ""
-            if self.selected_id in (-1, None)
-            else f"Identity {self.selected_id}: extra info"
-        )
-
     def paint(self, painter: CanvasPainter, frame_number: int):
         blobs_in_frame = self.blobs.blobs_in_video[frame_number]
         if self.id_groups.is_active():
             cmap, cmap_alpha = self.id_groups.get_cmaps(self.video.number_of_animals)
         else:
             cmap, cmap_alpha = self.cmap, self.cmap_alpha
 
@@ -642,15 +619,15 @@
         if self.setup_points.isVisible():
             self.setup_points.paint_on_canvas(painter)
 
         if self.interpolator.isEnabled():
             self.interpolator.paint_on_canvas(painter, frame_number)
 
         if update_info_widget:
-            self.update_right_bar(self.selected_blob)
+            self.additional_info.set_data(self.selected_blob)
 
     def closeEvent(self, event: QCloseEvent):
         if not self.unsaved_changes:
             return super().closeEvent(event)
 
         answer = QMessageBox.question(
             self,
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/errors_explorer.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/errors_explorer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_groups.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_groups.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/id_labels.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_labels.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/interpolator.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/interpolator.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/paint_blobs.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/paint_blobs.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_validator/validator_widgets/setup_points.py` & `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/setup_points.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.2/src/idtrackerai_video/general_video.py` & `idtrackerai-5.1.3/src/idtrackerai_video/general_video.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,54 +97,37 @@
             )
 
     return arr_img
 
 
 def generate_trajectories_video(
     video: Video,
-    trajectories_path: Path | None,
+    trajectories: np.ndarray,
     draw_in_gray: bool,
     centroid_trace_length: int,
     starting_frame: int,
     ending_frame: int,
 ):
-    if trajectories_path is None:
-        if (video.trajectories_folder / "trajectories_wo_gaps.npy").is_file():
-            trajectories = np.load(
-                video.trajectories_folder / "trajectories_wo_gaps.npy",
-                allow_pickle=True,
-            ).item()["trajectories"]
-        elif (video.trajectories_folder / "trajectories.npy").is_file():
-            trajectories = np.load(
-                video.trajectories_folder / "trajectories.npy", allow_pickle=True
-            ).item()["trajectories"]
-        else:
-            raise FileNotFoundError(
-                f"Could not find the trajectory file in {video.trajectories_folder}"
-            )
-    else:
-        trajectories = np.load(trajectories_path, allow_pickle=True).item()[
-            "trajectories"
-        ]
-
     if draw_in_gray:
         logging.info("Drawing original video in grayscale")
 
     resize_factor = min(1920 / video.original_width, 1080 / video.original_height, 1)
 
     if resize_factor != 1:
         logging.info(f"Applying resize of factor {resize_factor}")
 
     trajectories = np.nan_to_num(trajectories * resize_factor, nan=-1).astype(int)
 
     video_name = video.video_paths[0].stem + "_tracked.avi"
 
     colors = setColormap(video.number_of_animals)
 
-    labels = video.identities_labels
+    labels = video.identities_labels or list(
+        map(str, range(1, video.number_of_animals + 1))
+    )
 
     path_to_save_video = video.session_folder / video_name
 
     out_video_width = int(video.original_width * resize_factor)
     out_video_height = int(video.original_height * resize_factor)
 
     video_writer = cv2.VideoWriter(
```

### Comparing `idtrackerai-5.1.2/src/idtrackerai_video/main.py` & `idtrackerai-5.1.3/src/idtrackerai_video/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import logging
 from pathlib import Path
 
+import numpy as np
+
 from idtrackerai import Video
 from idtrackerai.utils import initLogger, wrap_exceptions
 
 from .general_video import generate_trajectories_video
 from .individual_videos import generate_individual_video
 
 
@@ -55,26 +58,47 @@
     parser.add_argument(
         "--e", type=int, default=None, help="Frame where to end the video", metavar=""
     )
     args = parser.parse_args()
 
     video = Video.load(args.session_path)
 
+    if args.t is None:
+        possible_files = (
+            "trajectories_validated.npy",
+            "trajectories_wo_gaps.npy",
+            "trajectories.npy",
+            "trajectories_wo_identification.npy",
+        )
+        for file in possible_files:
+            path = video.trajectories_folder / file
+            if path.is_file():
+                logging.info("Loading trajectories from %s", path)
+                trajectories = np.load(path, allow_pickle=True).item()["trajectories"]
+                break
+        else:
+            raise FileNotFoundError(
+                f"Could not find the trajectory file in {video.trajectories_folder}"
+            )
+    else:
+        logging.info("Loading trajectories from %s", args.t)
+        trajectories = np.load(args.t, allow_pickle=True).item()["trajectories"]
+
     if args.individual:
         generate_individual_video(
             video,
-            args.t,
+            trajectories,
             draw_in_gray=args.gray,
             starting_frame=args.s,
             ending_frame=args.e,
         )
     else:
         generate_trajectories_video(
             video,
-            args.t,
+            trajectories,
             draw_in_gray=args.gray,
             centroid_trace_length=args.tl,
             starting_frame=args.s,
             ending_frame=args.e,
         )
```

