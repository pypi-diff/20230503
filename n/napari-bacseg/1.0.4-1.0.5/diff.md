# Comparing `tmp/napari-bacseg-1.0.4.tar.gz` & `tmp/napari-bacseg-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bacseg-1.0.4.tar", last modified: Wed Mar 22 17:19:13 2023, max compression
+gzip compressed data, was "napari-bacseg-1.0.5.tar", last modified: Wed May  3 11:59:06 2023, max compression
```

## Comparing `napari-bacseg-1.0.4.tar` & `napari-bacseg-1.0.5.tar`

### file list

```diff
@@ -1,110 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.937716 napari-bacseg-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.621413 napari-bacseg-1.0.4/.github/
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.652629 napari-bacseg-1.0.4/.github/workflows/
--rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.4/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.659133 napari-bacseg-1.0.4/.napari-hub/
--rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/.napari-hub/DESCRIPTION.md
--rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/.napari-hub/config.yml
--rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.4/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4732 2023-03-22 17:19:13.937716 napari-bacseg-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/README.md
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/bacseg_ui.py
--rw-rw-rw-   0        0        0      988 2023-03-22 17:14:16.000000 napari-bacseg-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     2035 2023-03-22 17:19:13.937716 napari-bacseg-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.621413 napari-bacseg-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.837480 napari-bacseg-1.0.4/src/_dev/
--rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.4/src/_dev/Export Masks to AKSEG v5 dev.py
--rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.4/src/_dev/ScanR dev.py
--rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.4/src/_dev/Troodos dev.py
--rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.4/src/_dev/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.4/src/_dev/akseg_db_stats.py
--rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/akseg_dev.py
--rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/akseg_dev2.py
--rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.4/src/_dev/akseg_txt_metadata.py
--rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/align_alex_datadump.py
--rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/alison_datadump.py
--rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.4/src/_dev/autocontast_dev.py
--rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/cellposedev.py
--rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.4/src/_dev/cellposeshapely.py
--rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/check_metadata.py
--rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.4/src/_dev/colicoords_cellldist_dev.py
--rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.4/src/_dev/colicoords_ldist_dev.py
--rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.4/src/_dev/database_dev.py
--rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.4/src/_dev/edit_database_columns.py
--rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.4/src/_dev/fits_dev.py
--rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/fix_alison_missing_file_list.py
--rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/generate_scanr_movie.py
--rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/get_akseg_stats.py
--rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.4/src/_dev/get_species_info.py
--rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/luke__script.py
--rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.4/src/_dev/matplotlib_Events.py
--rw-rw-rw-   0        0        0    40859 2023-03-22 17:10:43.000000 napari-bacseg-1.0.4/src/_dev/move_AluGasketDFP.py
--rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.4/src/_dev/move_conor_nim_dfp_data.py
--rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.4/src/_dev/move_pillar_data.py
--rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/move_pillar_zstack_data.py
--rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.4/src/_dev/move_unlearning_files.py
--rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.4/src/_dev/new_metadata2.pickle.py
--rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.4/src/_dev/new_read_akseg_directory.py
--rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/nim_dev.py
--rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/omnipose_dev.py
--rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.4/src/_dev/omnipose_midlines.py
--rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.4/src/_dev/omnipose_train.py
--rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.4/src/_dev/oufti_dilate.py
--rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.4/src/_dev/oufti_dilate_with_midlines.py
--rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/process_alex_datadump.py
--rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/process_alex_datadump_clinical.py
--rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/process_conor_datadump.py
--rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/process_gramstain_datadump.py
--rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.4/src/_dev/read_non_tif.py
--rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/rebuild_usermeta.py
--rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/rebuild_usermeta_2.py
--rw-rw-rw-   0        0        0     1066 2023-03-22 15:20:16.000000 napari-bacseg-1.0.4/src/_dev/recreate_user_metadata.py
--rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/sort_midlines.py
--rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/stelios_stats.py
--rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/tile_meta_check.py
--rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.4/src/_dev/tiler_dev.py
--rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.4/src/_dev/updade_akseg_metadata.py
--rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.4/src/_dev/update_img_metadata.py
--rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.4/src/_dev/video_iamges.py
--rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.4/src/_dev/zooniverse.py
--rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.4/src/_dev/zooniverse_move.py
--rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.4/src/_dev/zooniverse_move_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.4/src/_dev/zooniverse_titration_upload.py
--rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.4/src/_dev/zooniverse_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.4/src/_dev/zooniverse_upload.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.906473 napari-bacseg-1.0.4/src/napari_bacseg/
--rw-rw-rw-   0        0        0      155 2023-03-22 17:14:16.000000 napari-bacseg-1.0.4/src/napari_bacseg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.937716 napari-bacseg-1.0.4/src/napari_bacseg/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/src/napari_bacseg/_tests/__init__.py
--rw-rw-rw-   0        0        0    26396 2023-03-22 17:12:50.000000 napari-bacseg-1.0.4/src/napari_bacseg/_tests/test_bacseg.py
--rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/_tests/test_widget.py
--rw-rw-rw-   0        0        0    84377 2023-03-21 16:02:29.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils.py
--rw-rw-rw-   0        0        0    13488 2023-03-21 16:02:26.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_cellpose.py
--rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_colicoords.py
--rw-rw-rw-   0        0        0    18409 2023-03-22 17:12:50.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_database.py
--rw-rw-rw-   0        0        0    43435 2023-03-22 17:12:50.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_database_IO.py
--rw-rw-rw-   0        0        0     1645 2023-03-09 18:16:07.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_imagej.py
--rw-rw-rw-   0        0        0    41284 2023-03-07 17:38:57.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_interface_events.py
--rw-rw-rw-   0        0        0     4220 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_json.py
--rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_oufti.py
--rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_refine.py
--rw-rw-rw-   0        0        0    21188 2023-03-07 17:38:57.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_statistics.py
--rw-rw-rw-   0        0        0     7055 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/_utils_tiler.py
--rw-rw-rw-   0        0        0      164 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg/_version.py
--rw-rw-rw-   0        0        0    68849 2023-03-22 17:12:50.000000 napari-bacseg-1.0.4/src/napari_bacseg/_widget.py
--rw-rw-rw-   0        0        0   132638 2023-03-22 17:12:50.000000 napari-bacseg-1.0.4/src/napari_bacseg/bacseg_ui.py
--rw-rw-rw-   0        0        0   132135 2023-03-22 17:12:50.000000 napari-bacseg-1.0.4/src/napari_bacseg/bacseg_ui.ui
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/gapseq_ui.py
--rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.4/src/napari_bacseg/napari.yaml
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.4/src/napari_bacseg/napari_ui.py
-drwxrwxrwx   0        0        0        0 2023-03-22 17:19:13.922095 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3015 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      352 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-22 17:19:13.000000 napari-bacseg-1.0.4/src/napari_bacseg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.4/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.168787 napari-bacseg-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:05.982743 napari-bacseg-1.0.5/.github/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:05.999644 napari-bacseg-1.0.5/.github/workflows/
+-rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.5/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.003644 napari-bacseg-1.0.5/.napari-hub/
+-rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/.napari-hub/DESCRIPTION.md
+-rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/.napari-hub/config.yml
+-rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.5/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4732 2023-05-03 11:59:06.168787 napari-bacseg-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/README.md
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/bacseg_ui.py
+-rw-rw-rw-   0        0        0      988 2023-05-03 11:58:10.000000 napari-bacseg-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     2035 2023-05-03 11:59:06.172787 napari-bacseg-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:05.984746 napari-bacseg-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.110818 napari-bacseg-1.0.5/src/_dev/
+-rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.5/src/_dev/Export Masks to AKSEG v5 dev.py
+-rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/ScanR dev.py
+-rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.5/src/_dev/Troodos dev.py
+-rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.5/src/_dev/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.5/src/_dev/akseg_db_stats.py
+-rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/akseg_dev.py
+-rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/akseg_dev2.py
+-rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.5/src/_dev/akseg_txt_metadata.py
+-rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/align_alex_datadump.py
+-rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/alison_datadump.py
+-rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.5/src/_dev/autocontast_dev.py
+-rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/cellposedev.py
+-rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.5/src/_dev/cellposeshapely.py
+-rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.5/src/_dev/chatGPT_midlines.py
+-rw-rw-rw-   0        0        0     4328 2023-05-03 08:47:29.000000 napari-bacseg-1.0.5/src/_dev/check_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/check_metadata.py
+-rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.5/src/_dev/colicoords_cellldist_dev.py
+-rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.5/src/_dev/colicoords_ldist_dev.py
+-rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.5/src/_dev/database_dev.py
+-rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.5/src/_dev/deepsegmattest.py
+-rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.5/src/_dev/edit_database_columns.py
+-rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.5/src/_dev/fits_dev.py
+-rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/fix_alison_missing_file_list.py
+-rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/generate_scanr_movie.py
+-rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/get_akseg_stats.py
+-rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.5/src/_dev/get_species_info.py
+-rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/luke__script.py
+-rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.5/src/_dev/matplotlib_Events.py
+-rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP.py
+-rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP_poster.py
+-rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.5/src/_dev/move_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.5/src/_dev/move_conor_nim_dfp_data.py
+-rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.5/src/_dev/move_pillar_data.py
+-rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/move_pillar_zstack_data.py
+-rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.5/src/_dev/move_unlearning_files.py
+-rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.5/src/_dev/new_metadata2.pickle.py
+-rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.5/src/_dev/new_read_akseg_directory.py
+-rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/nim_dev.py
+-rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/omnipose_dev.py
+-rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/omnipose_midlines.py
+-rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/omnipose_train.py
+-rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.5/src/_dev/oufti_dilate.py
+-rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.5/src/_dev/oufti_dilate_with_midlines.py
+-rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_alex_datadump.py
+-rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_alex_datadump_clinical.py
+-rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_conor_datadump.py
+-rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/process_gramstain_datadump.py
+-rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.5/src/_dev/read_non_tif.py
+-rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/rebuild_usermeta.py
+-rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/rebuild_usermeta_2.py
+-rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.5/src/_dev/recreate_user_metadata.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.5/src/_dev/scalebar_dev.py
+-rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/sort_midlines.py
+-rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/stelios_stats.py
+-rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/tile_meta_check.py
+-rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.5/src/_dev/tiler_dev.py
+-rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.5/src/_dev/updade_akseg_metadata.py
+-rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.5/src/_dev/update_img_metadata.py
+-rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.5/src/_dev/video_iamges.py
+-rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.5/src/_dev/zooniverse.py
+-rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_move.py
+-rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_move_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_titration_upload.py
+-rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.5/src/_dev/zooniverse_upload.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.146818 napari-bacseg-1.0.5/src/napari_bacseg/
+-rw-rw-rw-   0        0        0      155 2023-05-03 08:55:44.000000 napari-bacseg-1.0.5/src/napari_bacseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.168787 napari-bacseg-1.0.5/src/napari_bacseg/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/src/napari_bacseg/_tests/__init__.py
+-rw-rw-rw-   0        0        0    26398 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_bacseg.py
+-rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    88996 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils.py
+-rw-rw-rw-   0        0        0    13550 2023-04-21 11:56:56.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_cellpose.py
+-rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_colicoords.py
+-rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_database.py
+-rw-rw-rw-   0        0        0    57080 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_database_IO.py
+-rw-rw-rw-   0        0        0     1645 2023-03-09 18:16:07.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_imagej.py
+-rw-rw-rw-   0        0        0    39007 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_interface_events.py
+-rw-rw-rw-   0        0        0     4279 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_json.py
+-rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_oufti.py
+-rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_refine.py
+-rw-rw-rw-   0        0        0    21190 2023-03-27 09:54:48.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_statistics.py
+-rw-rw-rw-   0        0        0     7055 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_utils_tiler.py
+-rw-rw-rw-   0        0        0      164 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg/_version.py
+-rw-rw-rw-   0        0        0    92177 2023-05-03 08:53:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/_widget.py
+-rw-rw-rw-   0        0        0   158964 2023-04-21 13:35:29.000000 napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.py
+-rw-rw-rw-   0        0        0   156906 2023-04-21 13:28:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.ui
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/gapseq_ui.py
+-rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.5/src/napari_bacseg/napari.yaml
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.5/src/napari_bacseg/napari_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:59:06.164787 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3202 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      352 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-03 11:59:05.000000 napari-bacseg-1.0.5/src/napari_bacseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.5/tox.ini
```

### Comparing `napari-bacseg-1.0.4/.github/workflows/test_and_deploy.yml` & `napari-bacseg-1.0.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/.gitignore` & `napari-bacseg-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/.napari-hub/config.yml` & `napari-bacseg-1.0.5/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/.pre-commit-config.yaml` & `napari-bacseg-1.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/LICENSE` & `napari-bacseg-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/PKG-INFO` & `napari-bacseg-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.4/README.md` & `napari-bacseg-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/pyproject.toml` & `napari-bacseg-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [project]
 name = "napari-bacseg"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Piers Turner", email="piers.turner@physics.ox.ac.uk"},
 ]
 description = "Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `napari-bacseg-1.0.4/setup.cfg` & `napari-bacseg-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/Export Masks to AKSEG v5 dev.py` & `napari-bacseg-1.0.5/src/_dev/Export Masks to AKSEG v5 dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/ScanR dev.py` & `napari-bacseg-1.0.5/src/_dev/ScanR dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/akseg_db_stats.py` & `napari-bacseg-1.0.5/src/_dev/akseg_db_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/akseg_dev.py` & `napari-bacseg-1.0.5/src/_dev/akseg_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/akseg_dev2.py` & `napari-bacseg-1.0.5/src/_dev/akseg_dev2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/akseg_txt_metadata.py` & `napari-bacseg-1.0.5/src/_dev/akseg_txt_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/align_alex_datadump.py` & `napari-bacseg-1.0.5/src/_dev/align_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/alison_datadump.py` & `napari-bacseg-1.0.5/src/_dev/alison_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/autocontast_dev.py` & `napari-bacseg-1.0.5/src/_dev/autocontast_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/check_metadata.py` & `napari-bacseg-1.0.5/src/_dev/check_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/colicoords_cellldist_dev.py` & `napari-bacseg-1.0.5/src/_dev/colicoords_cellldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/colicoords_ldist_dev.py` & `napari-bacseg-1.0.5/src/_dev/colicoords_ldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/database_dev.py` & `napari-bacseg-1.0.5/src/_dev/database_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/edit_database_columns.py` & `napari-bacseg-1.0.5/src/_dev/edit_database_columns.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/fits_dev.py` & `napari-bacseg-1.0.5/src/_dev/fits_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/fix_alison_missing_file_list.py` & `napari-bacseg-1.0.5/src/_dev/fix_alison_missing_file_list.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/generate_scanr_movie.py` & `napari-bacseg-1.0.5/src/_dev/generate_scanr_movie.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/get_akseg_stats.py` & `napari-bacseg-1.0.5/src/_dev/get_akseg_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/get_species_info.py` & `napari-bacseg-1.0.5/src/_dev/get_species_info.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/luke__script.py` & `napari-bacseg-1.0.5/src/_dev/luke__script.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/matplotlib_Events.py` & `napari-bacseg-1.0.5/src/_dev/matplotlib_Events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/move_AluGasketDFP.py` & `napari-bacseg-1.0.5/src/_dev/move_AluGasketDFP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1015,50 +1015,50 @@
 user_metadata_path = os.path.join(r"\\physics\dfs\DAQ\CondensedMatterGroups\AKGroup\Piers\AKSEG\Images", user_initial, f"{user_initial}_file_metadata.txt")
 user_metadata = pd.read_csv(user_metadata_path, sep=",", low_memory=False)
 
 
 user_metadata = user_metadata[user_metadata["user_meta1"] != "Direct From Plate GASKET"]
 
 
-dat = upload_data[0]
+# dat = upload_data[0]
 
 # upload_data = upload_files(dat, unfold, image_lap_thr, tile_shape)
 
-focused_image_data, index_list, focus_list = get_focused_image_data(dat, unfold, image_lap_thr, remove_blurred, tile_shape)
+# focused_image_data, index_list, focus_list = get_focused_image_data(dat, unfold, image_lap_thr, remove_blurred, tile_shape)
 
 # upload_data = upload_files(dat, unfold, image_lap_thr, remove_blurred, tile_shape)
 
-# if __name__ == '__main__':
+if __name__ == '__main__':
     
-#     with Pool() as p:
+    with Pool() as p:
         
-#         results = list(tqdm.tqdm(p.imap(partial(upload_files,
-#                                                 unfold=unfold,
-#                                                 image_lap_thr=image_lap_thr,
-#                                                 remove_blurred=remove_blurred,
-#                                                 tile_shape=tile_shape),upload_data), total=len(upload_data)))
-#         p.close()
-#         p.join()
+        results = list(tqdm.tqdm(p.imap(partial(upload_files,
+                                                unfold=unfold,
+                                                image_lap_thr=image_lap_thr,
+                                                remove_blurred=remove_blurred,
+                                                tile_shape=tile_shape),upload_data), total=len(upload_data)))
+        p.close()
+        p.join()
         
-#         results = [item for item in results if results != None]
-#         results = [file_metadata for file_metadata_list in results for file_metadata in file_metadata_list if file_metadata != None]
+        results = [item for item in results if results != None]
+        results = [file_metadata for file_metadata_list in results for file_metadata in file_metadata_list if file_metadata != None]
         
-#         new_metadata = pd.DataFrame.from_dict(results)
+        new_metadata = pd.DataFrame.from_dict(results)
 
-#         with open('new_metadata.pickle', 'wb') as handle:
-#             pickle.dump(new_metadata, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        with open('new_metadata.pickle', 'wb') as handle:
+            pickle.dump(new_metadata, handle, protocol=pickle.HIGHEST_PROTOCOL)
     
-#         # with open('new_metadata.pickle', 'rb') as handle:
-#         #     new_metadata = pickle.load(handle)
+        # with open('new_metadata.pickle', 'rb') as handle:
+        #     new_metadata = pickle.load(handle)
     
-#         user_metadata = pd.concat([user_metadata,new_metadata],ignore_index=True).reset_index(drop=True)
+        user_metadata = pd.concat([user_metadata,new_metadata],ignore_index=True).reset_index(drop=True)
         
-#         user_metadata = user_metadata.drop_duplicates(subset=['akseg_hash'],keep="last")
+        user_metadata = user_metadata.drop_duplicates(subset=['akseg_hash'],keep="last")
         
-#         user_metadata.to_csv(user_metadata_path, sep=",", index = False) 
+        user_metadata.to_csv(user_metadata_path, sep=",", index = False)
```

### Comparing `napari-bacseg-1.0.4/src/_dev/move_conor_nim_dfp_data.py` & `napari-bacseg-1.0.5/src/_dev/move_conor_nim_dfp_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/move_pillar_data.py` & `napari-bacseg-1.0.5/src/_dev/move_pillar_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/move_pillar_zstack_data.py` & `napari-bacseg-1.0.5/src/_dev/move_pillar_zstack_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/move_unlearning_files.py` & `napari-bacseg-1.0.5/src/_dev/move_unlearning_files.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/new_metadata2.pickle.py` & `napari-bacseg-1.0.5/src/_dev/new_metadata2.pickle.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/new_read_akseg_directory.py` & `napari-bacseg-1.0.5/src/_dev/new_read_akseg_directory.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/nim_dev.py` & `napari-bacseg-1.0.5/src/_dev/nim_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/omnipose_dev.py` & `napari-bacseg-1.0.5/src/_dev/omnipose_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/omnipose_midlines.py` & `napari-bacseg-1.0.5/src/_dev/omnipose_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/omnipose_train.py` & `napari-bacseg-1.0.5/src/_dev/omnipose_train.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/oufti_dilate.py` & `napari-bacseg-1.0.5/src/_dev/oufti_dilate.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/oufti_dilate_with_midlines.py` & `napari-bacseg-1.0.5/src/_dev/oufti_dilate_with_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/process_alex_datadump.py` & `napari-bacseg-1.0.5/src/_dev/process_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/process_alex_datadump_clinical.py` & `napari-bacseg-1.0.5/src/_dev/process_alex_datadump_clinical.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/process_conor_datadump.py` & `napari-bacseg-1.0.5/src/_dev/process_conor_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/process_gramstain_datadump.py` & `napari-bacseg-1.0.5/src/_dev/process_gramstain_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/read_non_tif.py` & `napari-bacseg-1.0.5/src/_dev/read_non_tif.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/rebuild_usermeta.py` & `napari-bacseg-1.0.5/src/_dev/rebuild_usermeta.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/rebuild_usermeta_2.py` & `napari-bacseg-1.0.5/src/_dev/rebuild_usermeta_2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/sort_midlines.py` & `napari-bacseg-1.0.5/src/_dev/sort_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/stelios_stats.py` & `napari-bacseg-1.0.5/src/_dev/stelios_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/tile_meta_check.py` & `napari-bacseg-1.0.5/src/_dev/tile_meta_check.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/tiler_dev.py` & `napari-bacseg-1.0.5/src/_dev/tiler_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/updade_akseg_metadata.py` & `napari-bacseg-1.0.5/src/_dev/updade_akseg_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/update_img_metadata.py` & `napari-bacseg-1.0.5/src/_dev/update_img_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/video_iamges.py` & `napari-bacseg-1.0.5/src/_dev/video_iamges.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/zooniverse.py` & `napari-bacseg-1.0.5/src/_dev/zooniverse.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/zooniverse_move.py` & `napari-bacseg-1.0.5/src/_dev/zooniverse_move.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/zooniverse_move_titrations.py` & `napari-bacseg-1.0.5/src/_dev/zooniverse_move_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/zooniverse_titration_upload.py` & `napari-bacseg-1.0.5/src/_dev/zooniverse_titration_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/zooniverse_titrations.py` & `napari-bacseg-1.0.5/src/_dev/zooniverse_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/_dev/zooniverse_upload.py` & `napari-bacseg-1.0.5/src/_dev/zooniverse_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_tests/test_bacseg.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_bacseg.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,14 +388,15 @@
         database_directory = self.BacSeg._create_bacseg_database(path=path)
 
         self.BacSeg.database_path = database_directory
 
         return database_directory
 
     def get_database_metadata(self, user_initial="all"):
+
         database_directory = self.BacSeg.database_path
 
         if user_initial != "all":
             meta_path = os.path.join(self.BacSeg.database_path, "images", user_initial, f"{user_initial}_file_metadata.txt", )
 
             if os.path.exists(meta_path) == True:
                 metadata = pd.read_csv(meta_path, sep=",", low_memory=False)
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_tests/test_widget.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2168,21 +2168,92 @@
         beta = -minimum_gray * alpha
 
         image = cv2.convertScaleAbs(image, alpha=alpha, beta=beta)
 
     return image
 
 
+def add_scale_bar(
+    image,
+    pixel_resolution=100,
+    pixel_resolution_units="nm",
+    scalebar_size=20,
+    scalebar_size_units="um",
+    scalebar_colour="white",
+    scalebar_thickness=10,
+    scalebar_margin=10,
+):
+    try:
+        if float(pixel_resolution) > 0 and float(scalebar_size) > 0:
+            h, w = image.shape
+
+            pixel_resolution = float(pixel_resolution)
+            scalebar_size = float(scalebar_size)
+
+            scalebar_margin = int(w / 100 * scalebar_margin)
+
+            if pixel_resolution_units != "nm":
+                rescaled_pixel_resolution = pixel_resolution * 1000
+            else:
+                rescaled_pixel_resolution = pixel_resolution
+
+            if scalebar_size_units != "nm":
+                rescaled_scalebar_size = scalebar_size * 1000
+            else:
+                rescaled_scalebar_size = scalebar_size
+
+            scalebar_len = int(
+                rescaled_scalebar_size / rescaled_pixel_resolution
+            )
+
+            if scalebar_len > 0 and scalebar_len < w:
+                if scalebar_colour == "White":
+                    bit_depth = str(image.dtype)
+                    bit_depth = int(bit_depth.replace("uint", ""))
+                    colour = (2**bit_depth) - 1
+                else:
+                    colour = 0
+
+                scalebar_pos = (
+                    w - scalebar_margin - scalebar_len,
+                    h - scalebar_margin - int(scalebar_thickness),
+                )  # Position of the scale bar in the image (in pixels)
+
+                image = cv2.rectangle(
+                    image,
+                    scalebar_pos,
+                    (
+                        scalebar_pos[0] + scalebar_len,
+                        scalebar_pos[1] + int(scalebar_thickness),
+                    ),
+                    colour,
+                    -1,
+                )
+
+            else:
+                show_info(
+                    f"{int(scalebar_size)} ({scalebar_size_units}) Scale bar is too large for the {(rescaled_pixel_resolution/1000)*w}x{(rescaled_pixel_resolution/1000)*h} (um) image"
+                )
+
+    except:
+        print(traceback.format_exc())
+
+    return image
+
+
 def generate_export_image(
     self,
     export_channel,
     dim,
     normalize=False,
     invert=False,
     autocontrast=False,
+    scalebar=False,
+    cropzoom=False,
+    mask_background=False,
 ):
     layer_names = [
         layer.name
         for layer in self.viewer.layers
         if layer.name not in ["Segmentations", "Classes", "center_lines"]
     ]
 
@@ -2195,64 +2266,119 @@
     else:
         mode = "single"
         layer_names = [export_channel]
 
     if mode == "rgb":
         layer_names = layer_names[:3]
 
+    mask = self.segLayer.data
+    label = self.classLayer.data
+    metadata = self.viewer.layers[layer_names[0]].metadata
+
+    mask = mask[dim]
+    label = label[dim]
+    metadata = metadata[dim[0]]
+
+    if cropzoom:
+        layer = self.viewer.layers[layer_names[0]]
+        crop = layer.corner_pixels.T
+        y_range = crop[-2]
+        x_range = crop[-1]
+        mask = mask[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+        label = label[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+
     image = []
 
     for layer in layer_names:
-        img = self.viewer.layers[layer].data
+        img = self.viewer.layers[layer].data.copy()
 
         img = img[dim]
 
+        if cropzoom:
+            img = img[y_range[0] : y_range[1], x_range[0] : x_range[1]]
+
+        if mask_background:
+            img[mask == 0] = 0
+
         if invert:
             img = cv2.bitwise_not(img)
 
         if normalize:
             img = normalize99(img)
 
         if autocontrast:
             img = automatic_brightness_and_contrast(img)
 
+        if scalebar:
+            pixel_resolution = self.export_scalebar_resolution.text()
+            pixel_resolution_units = (
+                self.export_scalebar_resolution_units.currentText()
+            )
+            scalebar_size = self.export_scalebar_size.text()
+            scalebar_size_units = self.export_scalebar_size_units.currentText()
+            scalebar_colour = self.export_scalebar_colour.currentText()
+            scalebar_thickness = self.export_scalebar_thickness.currentText()
+
+            img = add_scale_bar(
+                img,
+                pixel_resolution=pixel_resolution,
+                pixel_resolution_units=pixel_resolution_units,
+                scalebar_size=scalebar_size,
+                scalebar_size_units=scalebar_size_units,
+                scalebar_colour=scalebar_colour,
+                scalebar_thickness=scalebar_thickness,
+            )
+
         image.append(img)
 
     if mode == "rgb":
         while len(image) < 3:
-            image.append(np.zeros(img.shape))
+            blank = np.zeros(img.shape, dtype=img.dtype)
+
+            if scalebar:
+                blank = add_scale_bar(
+                    blank,
+                    pixel_resolution=pixel_resolution,
+                    pixel_resolution_units=pixel_resolution_units,
+                    scalebar_size=scalebar_size,
+                    scalebar_size_units=scalebar_size_units,
+                    scalebar_colour=scalebar_colour,
+                    scalebar_thickness=scalebar_thickness,
+                )
+
+                print(True)
+
+            image.append(blank)
 
     if mode == "rgb":
         image = np.stack(image, axis=-1)
-    elif mode == "stack":
-        image = np.stack(image, axis=0)
 
-    image = rescale01(image)
-    image = image * (2**16 - 1)
-    image = image.astype(np.uint16)
+        image = rescale01(image)
+        image = image * (2**16 - 1)
+        image = image.astype(np.uint16)
 
-    mask = self.segLayer.data
-    label = self.classLayer.data
-    metadata = self.viewer.layers[layer_names[0]].metadata
-
-    mask = mask[dim]
-    label = label[dim]
-    metadata = metadata[dim[0]]
+    elif mode == "stack":
+        image = np.stack(image, axis=0)
+    else:
+        image = image[0]
 
     return image, mask, label, metadata, mode
 
 
 def export_files(self, progress_callback, mode):
     desktop = os.path.expanduser("~/Desktop")
 
     overwrite = self.export_overwrite_setting.isChecked()
     export_images = self.export_image_setting.isChecked()
     normalise = self.export_normalise.isChecked()
     invert = self.export_invert.isChecked()
     autocontrast = self.export_autocontrast.isChecked()
+    scalebar = self.export_scalebar.isChecked()
+    cropzoom = self.export_cropzoom.isChecked()
+    mask_background = self.export_mask_background.isChecked()
 
     export_channel = self.export_channel.currentText()
     export_modifier = self.export_modifier.text()
     export_labels = get_export_labels(self)
 
     data_shape = self.viewer.layers[0].data.shape
 
@@ -2272,15 +2398,23 @@
                 for tile_index in range(*viewer_dims[1]):
                     dim_list.append((image_index, tile_index))
             else:
                 dim_list.append((image_index,))
 
     for i, dim in enumerate(dim_list):
         image, mask, label, meta, mode = generate_export_image(
-            self, export_channel, dim, normalise, invert, autocontrast
+            self,
+            export_channel,
+            dim,
+            normalise,
+            invert,
+            autocontrast,
+            scalebar,
+            cropzoom,
+            mask_background,
         )
         contours = get_contours_from_mask(mask, label, export_labels)
 
         if "midlines" in meta.keys():
             midlines = meta["midlines"].copy()
         else:
             midlines = None
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_cellpose.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_cellpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,27 +128,30 @@
         self.cellpose_progressbar.setValue(0)
         self._autoClassify(reset=True)
         self._autoContrast()
 
         if self.cellpose_resetimage.isChecked() == True:
             self.viewer.reset_view()
 
-        layer_names = [
-            layer.name
-            for layer in self.viewer.layers
-            if layer.name not in ["Segmentations", "Classes", "center_lines"]
-        ]
-
-        # ensures segmentation and classes is in correct order in the viewer
-        for layer in layer_names:
-            layer_index = self.viewer.layers.index(layer)
-            self.viewer.layers.move(layer_index, 0)
+        self._reorderLayers()
+
+        # layer_names = [
+        #     layer.name
+        #     for layer in self.viewer.layers
+        #     if layer.name not in ["Segmentations", "Classes", "center_lines"]
+        # ]
+        #
+        # # ensures segmentation and classes is in correct order in the viewer
+        # for layer in layer_names:
+        #     layer_index = self.viewer.layers.index(layer)
+        #     self.viewer.layers.move(layer_index, 0)
 
 
 def load_cellpose_dependencies(self, omni=False):
+
     if self.widget_notifications:
         show_info("Loading Cellpose dependencies")
 
     if omni == True:
         from omnipose.core import labels_to_flows
     else:
         from cellpose.dynamics import labels_to_flows
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_colicoords.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_colicoords.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_database.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 import numpy as np
 import pandas as pd
 from glob2 import glob
 from napari.utils.notifications import show_info
 from qtpy.QtWidgets import (QCheckBox, QComboBox, QFileDialog, QLabel, QProgressBar, QPushButton, QTabWidget, )
 
+from napari_bacseg._utils_database_IO import read_user_metadata
 
 def _create_bacseg_database(self, viewer=None, database_name="BacSeg", path=None):
+
     if type(path) != str:
         desktop = os.path.expanduser("~/Desktop")
         path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
 
     if os.path.isdir(path):
         database_directory = str(pathlib.PurePath(path, f"{database_name}_Database"))
 
@@ -36,15 +38,15 @@
 
             folder_paths = [str(pathlib.PurePath(database_directory, folder)) for folder in folders]
 
             for folder_path in folder_paths:
                 if os.path.exists(folder_path) == False:
                     os.mkdir(folder_path)
 
-            database_metadata_list = ["abxconcentration", "antibiotic", "content", "microscope", "modality", "mount", "protocol", "source", "stain", "treatment_time", "user_initial", ]
+            database_metadata_list = ["abxconcentration", "antibiotic", "content", "microscope", "modality", "mount", "protocol", "source", "stain", "treatment_time", "user_initial", "strain", "phenotype"]
 
             user_metadata_list = ["example_user"]
 
             for meta_item in database_metadata_list:
                 txt_meta = f"# {database_name} Database Metadata: {meta_item} (Add new entries below):"
 
                 txt_meta_path = pathlib.PurePath(database_directory, "Metadata", f"{database_name} Database Metadata [{meta_item}].txt", )
@@ -97,26 +99,35 @@
 
     load_database_controls = ["create_database", "load_database", "display_database_path", "display_database_label", "database_io_title", ]
 
     [item.setVisible(visible) for item in all_database_controls if item.objectName() not in load_database_controls]
 
 
 def generate_txt_metadata(self, database_directory):
+
     database_name = (pathlib.Path(database_directory).parts[-1].replace("_Database", ""))
 
     path = pathlib.PurePath(database_directory, "Metadata", f"{database_name} Metadata.xlsx")
 
     if os.path.exists:
         akmeta = pd.read_excel(path, usecols="B:M", header=2)
 
-        akmeta = dict(user_initial=akmeta["User Initial"].dropna().astype(str).tolist(), content=akmeta["Image Content"].dropna().astype(str).tolist(), microscope=akmeta[
-            "Microscope"].dropna().astype(str).tolist(), modality=akmeta["Modality"].dropna().astype(str).tolist(), source=akmeta["Light Source"].dropna().astype(str).tolist(), antibiotic=akmeta[
-            "Antibiotic"].dropna().astype(str).tolist(), abxconcentration=akmeta["Antibiotic Concentration"].dropna().astype(str).tolist(), treatment_time=akmeta[
-            "Treatment Time (mins)"].dropna().astype(str).tolist(), stain=akmeta["Stains"].dropna().astype(str).tolist(), stain_target=akmeta["Stain Target"].dropna().astype(str).tolist(), mount=
-        akmeta["Mounting Method"].dropna().astype(str).tolist(), protocol=akmeta["Protocol"].dropna().astype(str).tolist(), )
+        akmeta = dict(
+            user_initial=akmeta["User Initial"].dropna().astype(str).tolist(),
+            content=akmeta["Image Content"].dropna().astype(str).tolist(),
+            microscope=akmeta["Microscope"].dropna().astype(str).tolist(),
+            modality=akmeta["Modality"].dropna().astype(str).tolist(),
+            source=akmeta["Light Source"].dropna().astype(str).tolist(),
+            antibiotic=akmeta["Antibiotic"].dropna().astype(str).tolist(),
+            abxconcentration=akmeta["Antibiotic Concentration"].dropna().astype(str).tolist(),
+            treatment_time=akmeta["Treatment Time (mins)"].dropna().astype(str).tolist(),
+            stain=akmeta["Stains"].dropna().astype(str).tolist(),
+            stain_target=akmeta["Stain Target"].dropna().astype(str).tolist(),
+            mount=akmeta["Mounting Method"].dropna().astype(str).tolist(),
+            protocol=akmeta["Protocol"].dropna().astype(str).tolist(), )
 
         # generate file metadata
 
         for key, value in akmeta.items():
             txt_meta = f"# {database_name} Database Metadata: {key} (Add new entries below):"
 
             txt_meta_path = pathlib.PurePath(database_directory, "Metadata", f"{database_name} Database Metadata [{key}].txt", )
@@ -246,14 +257,18 @@
         self.upload_abxconcentration.addItems([""] + akmeta["abxconcentration"])
         self.upload_treatmenttime.clear()
         self.upload_treatmenttime.addItems([""] + akmeta["treatment_time"])
         self.upload_mount.clear()
         self.upload_mount.addItems([""] + akmeta["mount"])
         self.upload_protocol.clear()
         self.upload_protocol.addItems([""] + akmeta["protocol"])
+        self.upload_strain.clear()
+        self.upload_strain.addItems([""] + akmeta["strain"])
+        self.upload_phenotype.clear()
+        self.upload_phenotype.addItems([""] + akmeta["phenotype"])
 
     except:
         print(traceback.format_exc())
 
 
 def update_database_metadata(self, control=None):
 
@@ -266,15 +281,15 @@
         user_intial_index = self.upload_initial.currentIndex()
 
         database_name = (pathlib.Path(database_directory).parts[-1].replace("_Database", ""))
 
         dbmeta, usermeta = read_txt_metadata(self, self.database_path)
 
         control_dict = {"abxconcentration": "upload_abxconcentration", "antibiotic": "upload_antibiotic", "content": "upload_content",
-                        "microscope": "upload_microscope", "modality": "label_modality", "mount": "upload_mount",
+                        "microscope": "upload_microscope", "modality": "label_modality", "mount": "upload_mount", "strain": "upload_strain", "phenotype": "upload_phenotype",
                         "protocol": "upload_protocol", "source": "label_light_source", "stain": "label_stain", "stain_target":
                         "label_stain_target", "treatment_time": "upload_treatmenttime", "user_initial": "upload_initial"}
 
         num_keys = self.user_metadata_keys
 
         for i in range(1, num_keys + 1):
             control_dict[f"meta{i}"] = f"upload_usermeta{i}"
@@ -397,32 +412,82 @@
         self.upload_initial.setCurrentIndex(user_intial_index)
 
         for control_name, control_text in upload_control_dict.items():
             combo_box = getattr(self, control_name)
             combo_box.setCurrentText(control_text)
 
 
+def read_file_metadata(self):
+
+    control_dict = {}
+
+    user_file_meta = {}
+
+    user_key_list = np.arange(1, self.user_metadata_keys + 1).tolist()
+    user_key_list.reverse()
+
+    for key in user_key_list:
+        user_key = f"meta{key}"
+        control_dict[user_key] = f"user_meta{key}"
+
+    database_path = self.database_path
+    user_initial = self.upload_initial.currentText()
+
+    if database_path != "" and user_initial != "":
+
+        user_metadata_path = os.path.join(database_path, "Images", user_initial, f"{user_initial}_file_metadata.txt", )
+
+        if os.path.exists(user_metadata_path):
+
+            user_metadata, _ = read_user_metadata(self, user_metadata_path = user_metadata_path)
+
+            for key, dfkey in control_dict.items():
+
+                if dfkey in user_metadata.columns:
+
+                    values = user_metadata[dfkey].unique().tolist()
+
+                    user_file_meta[key] = values
+
+                else:
+
+                    user_file_meta[key] = []
+
+    return user_file_meta
+
+
+
+
+
 def _populateUSERMETA(self):
+
     try:
         _, usermeta = read_txt_metadata(self, self.database_path)
 
+        file_usermeta = read_file_metadata(self)
+
         user_initial = self.upload_initial.currentText()
 
         num_keys = self.user_metadata_keys
 
         for key in range(1, num_keys + 1 ):
 
             control_name = f"upload_usermeta{key}"
             combo_box = getattr(self, control_name)
             combo_box.clear()
 
             if user_initial in usermeta.keys():
+                user_meta_values = usermeta[user_initial][f"meta{key}"]
+                file_meta_values = file_usermeta[f"meta{key}"]
 
-                meta_values = usermeta[user_initial][f"meta{key}"]
-                combo_box.addItems([""] + meta_values)
+                meta_values = np.unique(user_meta_values + file_meta_values).tolist()
 
+                meta_values = [value for value in meta_values if value not in ["", " ", "nan", "Required for upload",
+                                                                               'example_item1', 'example_item2', 'example_item3',
+                                                                               None, np.nan]]
+                combo_box.addItems([""] + meta_values)
             else:
                 combo_box.setCurrentText("")
 
     except:
         # print(traceback.format_exc())
         pass
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_database_IO.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_database_IO.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 import json
 import os
 import shutil
 import tempfile
 
 # from napari_bacseg._utils_json import import_coco_json, export_coco_json
 import traceback
+from csv import Sniffer
 from multiprocessing import Pool
 
+import cv2
 import numpy as np
 import pandas as pd
 import tifffile
-import cv2
 from napari.utils.notifications import show_info
-from napari_bacseg._utils_json import export_coco_json
 
+from napari_bacseg._utils_json import export_coco_json, import_coco_json
 
-def check_metadata_format(metadata, expected_columns):
-    if "stains" in metadata.columns:
-        metadata = metadata.rename(columns={"stains": "stain"})
 
-    missing_columns = list(set(expected_columns) - set(metadata.columns))
-    extra_columns = list(set(metadata.columns) - set(expected_columns))
+def check_metadata_format(metadata, expected_columns):
+    missing_columns = list(
+        set(expected_columns) - set(metadata.columns.tolist())
+    )
+    extra_columns = list(
+        set(metadata.columns.tolist()) - set(expected_columns)
+    )
 
-    all_columns = expected_columns + extra_columns
+    all_columns = list(set(expected_columns + extra_columns))
 
     metadata[missing_columns] = pd.DataFrame(
         [[None] * len(missing_columns)], index=metadata.index
     )
 
     date = datetime.datetime.now()
 
@@ -55,160 +58,131 @@
         data = meta[value]
     else:
         data = None
 
     return data
 
 
+def list_from_string(string):
+    string_list = string.strip("[]")
+    string_list = string_list.split(",")
+    string_list = [x.strip() for x in string_list]
+
+    return string_list
+
+
 def read_bacseg_images(self, progress_callback, measurements, channels):
+    database_path = self.database_path
+
     imported_images = {}
     iter = 1
 
     import_limit = self.database_download_limit.currentText()
 
     if import_limit == "All":
         import_limit = len(measurements)
     else:
         if int(import_limit) > len(measurements):
             import_limit = len(measurements)
 
-    for i in range(int(import_limit)):
+    if import_limit == str(1):
         try:
-            measurement = measurements.get_group(list(measurements.groups)[i])
-            iter += 1
-
-            for j in range(len(channels)):
-                channel = channels[j]
-
-                measurement_channels = measurement["channel"].unique()
-
-                if channel in measurement_channels:
-                    dat = measurement[measurement["channel"] == channel]
+            measurement = measurements.get_group(list(measurements.groups)[0])
+            imported_data = [
+                download_bacseg_files(measurement, channels, database_path)
+            ]
+            progress_callback.emit(100)
+        except:
+            pass
+    else:
+        measurements = [
+            measurements.get_group(i) for i in measurements.groups
+        ][: int(import_limit)]
+        with Pool(4) as pool:
+            iter = []
+
+            def callback(*args):
+                iter.append(1)
+                progress = (len(iter) / int(import_limit)) * 100
 
-                    progress = int(((iter + 1) / int(import_limit)) * 100)
+                if progress_callback != None:
                     try:
                         progress_callback.emit(progress)
                     except:
                         pass
 
-                    if self.widget_notifications:
-                        show_info(
-                            "loading image["
-                            + str(channel)
-                            + "] "
-                            + str(i + 1)
-                            + " of "
-                            + str(int(import_limit))
-                        )
+                return
 
-                    file_name = dat["file_name"].item()
-                    user_initial = dat["user_initial"].item()
-                    folder = dat["folder"].item()
-
-                    database_path = self.database_path
-
-                    image_path = os.path.join(
-                        database_path,
-                        "Images",
-                        user_initial,
-                        "images",
-                        folder,
-                        file_name,
-                    )
-                    mask_path = os.path.join(
-                        database_path,
-                        "Images",
-                        user_initial,
-                        "masks",
-                        folder,
-                        file_name,
-                    )
-                    label_path = os.path.join(
-                        database_path,
-                        "Images",
-                        user_initial,
-                        "labels",
-                        folder,
-                        file_name,
-                    )
+            results = [
+                pool.apply_async(
+                    download_bacseg_files,
+                    args=(measurement, channels, database_path),
+                    callback=callback,
+                )
+                for measurement in measurements
+            ]
 
-                    image_path = os.path.abspath(image_path)
-                    mask_path = os.path.abspath(mask_path)
-                    label_path = os.path.abspath(label_path)
-
-                    image = tifffile.imread(image_path)
-                    mask = tifffile.imread(mask_path)
-                    label = tifffile.imread(label_path)
-
-                    with tifffile.TiffFile(image_path) as tif:
-                        try:
-                            meta = tif.pages[0].tags["ImageDescription"].value
-                            meta = json.loads(meta)
-                        except:
-                            meta = {}
+            try:
+                results[-1].get()
+            except:
+                print(traceback.format_exc())
+            else:
+                results = [r.get() for r in results]
+                imported_data = [dat for dat in results if dat != {}]
+                pool.close()
+                pool.join()
 
-                    meta["import_mode"] = "BacSeg"
+    try:
+        imported_images = {}
 
-                else:
-                    image = np.zeros((100, 100), dtype=np.uint16)
-                    mask = np.zeros((100, 100), dtype=np.uint16)
-                    label = np.zeros((100, 100), dtype=np.uint16)
-
-                    meta = {}
-
-                    meta["image_name"] = "missing image channel"
-                    meta["image_path"] = "missing image channel"
-                    meta["folder"] = (None,)
-                    meta["parent_folder"] = (None,)
-                    meta["akseg_hash"] = None
-                    meta["fov_mode"] = None
-                    meta["import_mode"] = "BacSeg"
-                    meta["contrast_limit"] = None
-                    meta["contrast_alpha"] = None
-                    meta["contrast_beta"] = None
-                    meta["contrast_gamma"] = None
-                    meta["dims"] = [image.shape[-1], image.shape[-2]]
-                    meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
-                    meta["light_source"] = channel
+        for dat in imported_data:
+            for channel, channel_data in dat.items():
+                image = channel_data["images"]
+                mask = channel_data["masks"]
+                label = channel_data["classes"]
+                meta = channel_data["metadata"]
 
-                if channel not in imported_images:
+                if channel not in imported_images.keys():
                     imported_images[channel] = dict(
                         images=[image],
                         masks=[mask],
                         classes=[label],
-                        metadata={i: meta},
+                        metadata={0: meta},
                     )
                 else:
+                    image_index = len(imported_images[channel]["images"])
+
                     imported_images[channel]["images"].append(image)
                     imported_images[channel]["masks"].append(mask)
                     imported_images[channel]["classes"].append(label)
-                    imported_images[channel]["metadata"][i] = meta
+                    imported_images[channel]["metadata"][image_index] = meta
 
-        except:
-            print(traceback.format_exc())
+    except:
+        print(traceback.format_exc())
 
     imported_data = dict(imported_images=imported_images)
 
     return imported_data
 
 
 def generate_multichannel_stack(self):
-
     segChannel = self.cellpose_segchannel.currentText()
     user_initial = self.upload_initial.currentText()
     content = self.upload_content.currentText()
     microscope = self.upload_microscope.currentText()
     antibiotic = self.upload_antibiotic.currentText()
     abxconcentration = self.upload_abxconcentration.currentText()
     treatmenttime = self.upload_treatmenttime.currentText()
     mount = self.upload_mount.currentText()
     protocol = self.upload_protocol.currentText()
     overwrite_all_metadata = self.overwrite_all_metadata.isChecked()
     overwrite_selected_metadata = self.overwrite_selected_metadata.isChecked()
     date_uploaded = datetime.datetime.now()
+    strain = self.upload_strain.currentText()
+    phenotype = self.upload_phenotype.currentText()
 
     segmented = False
     segmented_curated = False
     labelled = False
     labelled_curated = False
 
     if self.upload_segmentation_combo.currentIndex() == 2:
@@ -228,19 +202,22 @@
         user_initial=user_initial,
         content=content,
         microscope=microscope,
         antibiotic=antibiotic,
         abxconcentration=abxconcentration,
         treatmenttime=treatmenttime,
         mount=mount,
-        protocol=protocol)
+        protocol=protocol,
+        strain=strain,
+        phenotype=phenotype,
+    )
 
     num_user_keys = self.user_metadata_keys
 
-    for key in range(1, num_user_keys+1):
+    for key in range(1, num_user_keys + 1):
         control_name = f"upload_usermeta{key}"
         combo_box = getattr(self, control_name)
         combo_box_value = combo_box.currentText()
         metadata[f"usermeta{key}"] = combo_box_value
 
     layer_names = [
         layer.name
@@ -279,35 +256,49 @@
 
                 if meta["image_name"] != "missing image channel":
                     file_list.append(meta["image_name"])
                     layer_list.append(layer)
 
                     meta["user_initial"] = user_initial
 
-                    if (meta["import_mode"] != "BacSeg" or overwrite_all_metadata is True):
-
+                    if (
+                        meta["import_mode"] != "BacSeg"
+                        or overwrite_all_metadata is True
+                    ):
                         meta["microscope"] = microscope
                         meta["image_content"] = content
                         meta["antibiotic"] = antibiotic
+                        meta["strain"] = strain
+                        meta["phenotype"] = phenotype
                         meta["treatmenttime"] = treatmenttime
                         meta["abxconcentration"] = abxconcentration
                         meta["mount"] = mount
                         meta["protocol"] = protocol
                         meta["channel"] = layer
                         meta["segmentation_channel"] = segChannel
                         meta["file_list"] = []
                         meta["layer_list"] = []
                         meta["segmentation_file"] = segmentation_file
 
-                        for key in range(1, num_user_keys+1):
+                        for key in range(1, num_user_keys + 1):
                             meta[f"usermeta{key}"] = metadata[f"usermeta{key}"]
-                            print(meta[f"usermeta{key}"], metadata[f"usermeta{key}"])
+                            print(
+                                meta[f"usermeta{key}"],
+                                metadata[f"usermeta{key}"],
+                            )
 
-                    if (meta["import_mode"] == "BacSeg"and overwrite_all_metadata is True):
-                        metadata = {key: val for key, val in metadata.items() if val != "Required for upload"}
+                    if (
+                        meta["import_mode"] == "BacSeg"
+                        and overwrite_all_metadata is True
+                    ):
+                        metadata = {
+                            key: val
+                            for key, val in metadata.items()
+                            if val != "Required for upload"
+                        }
 
                         for key, value in metadata.items():
                             meta[key] = value
 
                     if overwrite_selected_metadata is True:
                         metadata = {
                             key: val
@@ -362,15 +353,119 @@
 
         except:
             pass
 
     return multi_image_stack, multi_meta_stack, layer_names
 
 
-def upload_bacseg_files(path, widget_notifications=True, num_user_keys = 5):
+def download_bacseg_files(measurement, channels, database_path):
+    imported_images = {}
+
+    try:
+        segmentation_channel = measurement["segmentation_channel"].unique()[0]
+
+        segmentation_file = measurement[
+            measurement["channel"] == segmentation_channel
+        ]["file_name"].item()
+        user_initial = measurement[
+            measurement["channel"] == segmentation_channel
+        ]["user_initial"].item()
+        folder = measurement[measurement["channel"] == segmentation_channel][
+            "folder"
+        ].item()
+
+        json_path = os.path.join(
+            database_path,
+            "Images",
+            user_initial,
+            "json",
+            folder,
+            segmentation_file,
+        )
+
+        mask, label = import_coco_json(json_path)
+
+        for j in range(len(channels)):
+            channel = channels[j]
+
+            measurement_channels = measurement["channel"].unique()
+
+            if channel in measurement_channels:
+                dat = measurement[measurement["channel"] == channel]
+
+                file_name = dat["file_name"].item()
+                user_initial = dat["user_initial"].item()
+                folder = dat["folder"].item()
+
+                image_path = os.path.join(
+                    database_path,
+                    "Images",
+                    user_initial,
+                    "images",
+                    folder,
+                    file_name,
+                )
+                image_path = os.path.abspath(image_path)
+
+                image = tifffile.imread(image_path)
+
+                with tifffile.TiffFile(image_path) as tif:
+                    try:
+                        meta = tif.pages[0].tags["ImageDescription"].value
+                        meta = json.loads(meta)
+                    except:
+                        meta = {}
+
+                meta["import_mode"] = "BacSeg"
+
+                for key, value in dat.to_dict("records")[0].items():
+                    meta[key] = value
+
+                if "segmentation_file" in meta.keys():
+                    if meta["segmentation_file"] in [None, "None"]:
+                        meta["segmentation_file"] = list_from_string(
+                            measurement["file_list"].iloc[0]
+                        )[0]
+                        meta["segmentation_channel"] = list_from_string(
+                            measurement["channel_list"].iloc[0]
+                        )[0]
+
+            else:
+                image = np.zeros((100, 100), dtype=np.uint16)
+                mask = np.zeros((100, 100), dtype=np.uint16)
+                label = np.zeros((100, 100), dtype=np.uint16)
+
+                meta = {}
+
+                meta["image_name"] = "missing image channel"
+                meta["image_path"] = "missing image channel"
+                meta["folder"] = (None,)
+                meta["parent_folder"] = (None,)
+                meta["akseg_hash"] = None
+                meta["fov_mode"] = None
+                meta["import_mode"] = "BacSeg"
+                meta["contrast_limit"] = None
+                meta["contrast_alpha"] = None
+                meta["contrast_beta"] = None
+                meta["contrast_gamma"] = None
+                meta["dims"] = [image.shape[-1], image.shape[-2]]
+                meta["crop"] = [0, image.shape[-2], 0, image.shape[-1]]
+                meta["light_source"] = channel
+
+            imported_images[channel] = dict(
+                images=image, masks=mask, classes=label, metadata=meta
+            )
+
+    except:
+        pass
+
+    return imported_images
+
+
+def upload_bacseg_files(path, widget_notifications=True, num_user_keys=6):
     file_metadata_list = []
 
     try:
         dat = np.load(path, allow_pickle=True).item()
 
         user_metadata = dat["user_metadata"]
         image = dat["image"]
@@ -379,14 +474,17 @@
         class_mask = dat["class_mask"]
         save_dir = dat["save_dir"]
         overwrite_images = dat["overwrite_images"]
         overwrite_masks = dat["overwrite_masks"]
         overwrite_metadata = dat["overwrite_metadata"]
         overwrite_selected_metadata = dat["overwrite_selected_metadata"]
         overwrite_all_metadata = dat["overwrite_all_metadata"]
+        upload_images = dat["upload_images"]
+        upload_segmentations = dat["upload_segmentations"]
+        upload_metadata = dat["upload_metadata"]
         image_dir = dat["image_dir"]
         mask_dir = dat["mask_dir"]
         class_dir = dat["class_dir"]
         json_dir = dat["json_dir"]
 
         metadata_file_names = user_metadata["file_name"].tolist()
         metadata_akseg_hash = user_metadata["akseg_hash"].tolist()
@@ -398,14 +496,16 @@
         for j, layer in enumerate(channel_list):
             img = image[j, :, :]
             meta = image_meta[layer]
 
             file_name = get_meta_value(meta, "image_name")
             folder = get_meta_value(meta, "folder")
             akseg_hash = get_meta_value(meta, "akseg_hash")
+            strain = get_meta_value(meta, "strain")
+            phenotype = get_meta_value(meta, "phenotype")
 
             import_mode = meta["import_mode"]
 
             if "posX" in meta.keys():
                 posX = meta["posX"]
                 posY = meta["posX"]
                 posZ = meta["posX"]
@@ -513,15 +613,17 @@
                 else:
                     img = img[y1:y2, x1:x2]
 
                 mask = mask[y1:y2, x1:x2]
                 class_mask = class_mask[y1:y2, x1:x2]
 
                 unique_segmentations = np.unique(mask)
-                unique_segmentations = np.delete(unique_segmentations, np.where(unique_segmentations == 0))
+                unique_segmentations = np.delete(
+                    unique_segmentations, np.where(unique_segmentations == 0)
+                )
 
                 num_segmentations = len(unique_segmentations)
                 image_laplacian = cv2.Laplacian(img, cv2.CV_64F).var()
 
                 meta.pop("shape", None)
 
                 file_name = os.path.splitext(meta["image_name"])[0] + ".tif"
@@ -529,35 +631,46 @@
                 image_path = os.path.join(image_dir, file_name)
                 mask_path = os.path.join(mask_dir, file_name)
                 json_path = os.path.join(
                     json_dir, file_name.replace(".tif", ".txt")
                 )
                 class_path = os.path.join(class_dir, file_name)
 
-                if (
-                    os.path.isfile(image_path) is False
-                    or import_mode == "BacSeg"
-                    or overwrite_images is True
-                    or overwrite_metadata is True
-                ):
-                    tifffile.imwrite(
-                        os.path.abspath(image_path), img, metadata=meta
-                    )
+                segmentation_file = get_meta_value(meta, "segmentation_file")
 
-                if (
-                    os.path.isfile(mask_path) is False
-                    or import_mode == "BacSeg"
-                    or overwrite_masks is True
-                    or overwrite_metadata is True
-                ):
-                    tifffile.imwrite(mask_path, mask, metadata=meta)
-                    tifffile.imwrite(class_path, class_mask, metadata=meta)
-                    export_coco_json(
-                        file_name, img, mask, class_mask, json_path
-                    )
+                if segmentation_file is None:
+                    segmentation_channel = channel_list[0]
+                    segmentation_file = image_meta[segmentation_channel][
+                        "image_name"
+                    ]
+                    meta["segmentation_file"] = segmentation_file
+                    meta["segmentation_channel"] = segmentation_channel
+
+                if upload_images is True:
+                    if (
+                        os.path.isfile(image_path) is False
+                        or import_mode == "BacSeg"
+                        or overwrite_images is True
+                        or overwrite_metadata is True
+                    ):
+                        tifffile.imwrite(
+                            os.path.abspath(image_path), img, metadata=meta
+                        )
+
+                if upload_segmentations is True:
+                    if (
+                        os.path.isfile(mask_path) is False
+                        or import_mode == "BacSeg"
+                        or overwrite_masks is True
+                        or overwrite_metadata is True
+                    ):
+                        if file_name == segmentation_file:
+                            export_coco_json(
+                                file_name, img, mask, class_mask, json_path
+                            )
 
                 if "mask_path" not in meta.keys():
                     meta["mask_path"] = None
                 if "label_path" not in meta.keys():
                     meta["label_path"] = None
 
                 file_metadata = {
@@ -570,52 +683,63 @@
                     "channel_list": get_meta_value(meta, "channel_list"),
                     "segmentation_file": get_meta_value(
                         meta, "segmentation_file"
                     ),
                     "segmentation_channel": get_meta_value(
                         meta, "segmentation_channel"
                     ),
+                    "strain": get_meta_value(meta, "strain"),
+                    "phenotype": get_meta_value(meta, "phenotype"),
                     "akseg_hash": get_meta_value(meta, "akseg_hash"),
                     "user_initial": get_meta_value(meta, "user_initial"),
                     "content": get_meta_value(meta, "image_content"),
                     "microscope": get_meta_value(meta, "microscope"),
                     "modality": get_meta_value(meta, "modality"),
                     "source": get_meta_value(meta, "light_source"),
                     "stain": get_meta_value(meta, "stain"),
                     "stain_target": get_meta_value(meta, "stain_target"),
                     "antibiotic": get_meta_value(meta, "antibiotic"),
-                    "treatment time (mins)": get_meta_value(meta, "treatmenttime"),
-                    "antibiotic concentration": get_meta_value(meta, "abxconcentration"),
+                    "treatment time (mins)": get_meta_value(
+                        meta, "treatmenttime"
+                    ),
+                    "antibiotic concentration": get_meta_value(
+                        meta, "abxconcentration"
+                    ),
                     "mounting method": get_meta_value(meta, "mount"),
                     "protocol": get_meta_value(meta, "protocol"),
                     "folder": get_meta_value(meta, "folder"),
                     "parent_folder": get_meta_value(meta, "parent_folder"),
                     "num_segmentations": num_segmentations,
                     "image_laplacian": image_laplacian,
                     "image_focus": get_meta_value(meta, "image_focus"),
                     "image_debris": get_meta_value(meta, "image_debris"),
                     "segmented": get_meta_value(meta, "segmented"),
                     "labelled": get_meta_value(meta, "labelled"),
-                    "segmentation_curated": get_meta_value(meta, "segmentations_curated"),
+                    "segmentation_curated": get_meta_value(
+                        meta, "segmentations_curated"
+                    ),
                     "label_curated": get_meta_value(meta, "labels_curated"),
                     "posX": posX,
                     "posY": posY,
                     "posZ": posZ,
                     "image_load_path": get_meta_value(meta, "image_path"),
                     "image_save_path": image_path,
                     "mask_load_path": get_meta_value(meta, "mask_path"),
                     "mask_save_path": mask_path,
                     "label_load_path": get_meta_value(meta, "label_path"),
                     "label_save_path": class_path,
                 }
 
                 for key in range(1, num_user_keys + 1):
-                    file_metadata[f"user_meta{key}"] = get_meta_value(meta, f"usermeta{key}")
+                    file_metadata[f"user_meta{key}"] = get_meta_value(
+                        meta, f"usermeta{key}"
+                    )
 
                 file_metadata_list.append(file_metadata)
+
     except:
         file_metadata_list = []
         print(traceback.format_exc())
 
     return file_metadata_list
 
 
@@ -627,14 +751,17 @@
     class_stack,
     save_dir,
     overwrite_images,
     overwrite_masks,
     overwrite_metadata,
     overwrite_selected_metadata,
     overwrite_all_metadata,
+    upload_images,
+    upload_segmentations,
+    upload_metadata,
 ):
     upload_tempfiles = []
 
     upload_dir = os.path.join(tempfile.gettempdir(), "BacSeg")
 
     if os.path.isdir(upload_dir) != True:
         os.mkdir(upload_dir)
@@ -682,16 +809,26 @@
                 overwrite_metadata=overwrite_metadata,
                 overwrite_selected_metadata=overwrite_selected_metadata,
                 overwrite_all_metadata=overwrite_all_metadata,
                 image_dir=image_dir,
                 mask_dir=mask_dir,
                 json_dir=json_dir,
                 class_dir=class_dir,
+                upload_images=upload_images,
+                upload_segmentations=upload_segmentations,
+                upload_metadata=upload_metadata,
             )
 
+            # if "segmentation_file" in user_metadata:
+            #     print("segmentation_file in user_metadata")
+            # elif "segmentation_channel" in image_meta:
+            #     print("segmentation_channel in image_meta")
+            # else:
+            #     print("segmentation_file not in user_metadata and segmentation_channel not in image_meta")
+
             if os.path.isdir(upload_dir) is False:
                 os.mkdir(upload_dir)
 
             temp_path = tempfile.TemporaryFile(
                 prefix="BacSeg", suffix=".npy", dir=upload_dir
             ).name
 
@@ -720,15 +857,24 @@
             source = self.label_light_source.currentText()
             stain = self.label_stain.currentText()
             stain_target = self.label_stain_target.currentText()
             date_modified = datetime.datetime.now()
             overwrite_images = self.upload_overwrite_images.isChecked()
             overwrite_masks = self.upload_overwrite_masks.isChecked()
             overwrite_all_metadata = self.overwrite_all_metadata.isChecked()
-            overwrite_selected_metadata = (self.overwrite_selected_metadata.isChecked())
+            overwrite_selected_metadata = (
+                self.overwrite_selected_metadata.isChecked()
+            )
+            upload_images = self.upload_images_setting.isChecked()
+            upload_segmentations = (
+                self.upload_segmentations_setting.isChecked()
+            )
+            upload_metadata = self.upload_metadata_setting.isChecked()
+            strain = self.upload_strain.currentText()
+            phenotype = self.upload_phenotype.currentText()
 
             num_user_keys = self.user_metadata_keys
 
             save_dir = os.path.join(database_path, "Images", user_initial)
 
             if (
                 overwrite_all_metadata is True
@@ -742,20 +888,16 @@
                 database_path,
                 "Images",
                 user_initial,
                 f"{user_initial}_file_metadata.txt",
             )
 
             if os.path.exists(user_metadata_path):
-                user_metadata = pd.read_csv(
-                    user_metadata_path, sep=",", low_memory=False
-                )
-
-                user_metadata, expected_columns = check_metadata_format(
-                    user_metadata, self.metadata_columns
+                user_metadata, expected_columns = read_user_metadata(
+                    self, user_metadata_path=user_metadata_path
                 )
 
                 metadata_file_names = user_metadata["file_name"].tolist()
                 metadata_akseg_hash = user_metadata["akseg_hash"].tolist()
 
             else:
                 expected_columns = self.metadata_columns
@@ -808,14 +950,16 @@
                 ]
 
                 if segChannel == "":
                     if self.widget_notifications:
                         show_info("Please pick an image channel to upload")
 
                 else:
+                    backup_user_metadata(self, user_metadata)
+
                     image_layer = self.viewer.layers[segChannel]
 
                     (
                         image_stack,
                         meta_stack,
                         channel_list,
                     ) = generate_multichannel_stack(self)
@@ -847,18 +991,23 @@
                         class_stack,
                         save_dir,
                         overwrite_images,
                         overwrite_masks,
                         overwrite_metadata,
                         overwrite_selected_metadata,
                         overwrite_all_metadata,
+                        upload_images,
+                        upload_segmentations,
+                        upload_metadata,
                     )
 
                     if mode == "active":
-                        results = upload_bacseg_files(upload_tempfiles[0], num_user_keys)
+                        results = upload_bacseg_files(
+                            upload_tempfiles[0], num_user_keys
+                        )
 
                     else:
                         with Pool(4) as pool:
                             iter = []
 
                             def callback(*args):
                                 iter.append(1)
@@ -873,15 +1022,15 @@
                                         pass
 
                                 return
 
                             results = [
                                 pool.apply_async(
                                     upload_bacseg_files,
-                                    args=(i,num_user_keys),
+                                    args=(i, num_user_keys),
                                     callback=callback,
                                 )
                                 for i in upload_tempfiles
                             ]
 
                             try:
                                 results[-1].get()
@@ -898,218 +1047,432 @@
                                 pool.close()
                                 pool.join()
 
                             results = [
                                 dat for dat in results if results != None
                             ]
 
-                    for file_metadata in results:
-                        if file_metadata != None:
-                            akseg_hash = file_metadata["akseg_hash"]
+                    if upload_metadata is True:
+                        for file_metadata in results:
+                            if file_metadata != None:
+                                akseg_hash = file_metadata["akseg_hash"]
 
-                            file_metadata = pd.DataFrame.from_dict(
-                                file_metadata, dtype=object
-                            )
+                                file_metadata = pd.DataFrame.from_dict(
+                                    file_metadata, dtype=object
+                                )
 
-                            columns = file_metadata.columns.tolist()
-                            column_dict = {
-                                col: "first"
-                                for col in columns
-                                if col not in ["file_list", "channel_list"]
-                            }
+                                columns = file_metadata.columns.tolist()
+                                column_dict = {
+                                    col: "first"
+                                    for col in columns
+                                    if col not in ["file_list", "channel_list"]
+                                }
+
+                                df = (
+                                    file_metadata.groupby(["file_name"]).agg(
+                                        {
+                                            **{
+                                                "file_list": lambda x: x.tolist(),
+                                                "channel_list": lambda x: x.tolist(),
+                                            },
+                                            **column_dict,
+                                        }
+                                    )
+                                ).reset_index(drop=True)
 
-                            df = (
-                                file_metadata.groupby(["file_name"]).agg(
+                                file_metadata = df[columns]
+
+                                file_metadata = file_metadata.astype(
                                     {
-                                        **{
-                                            "file_list": lambda x: x.tolist(),
-                                            "channel_list": lambda x: x.tolist(),
-                                        },
-                                        **column_dict,
+                                        "segmented": bool,
+                                        "labelled": bool,
+                                        "segmentation_curated": bool,
+                                        "label_curated": bool,
                                     }
                                 )
-                            ).reset_index(drop=True)
-
-                            file_metadata = df[columns]
-
-                            file_metadata = file_metadata.astype(
-                                {
-                                    "segmented": bool,
-                                    "labelled": bool,
-                                    "segmentation_curated": bool,
-                                    "label_curated": bool,
-                                }
-                            )
-
-                            user_metadata = user_metadata.astype(
-                                {
-                                    "segmented": bool,
-                                    "labelled": bool,
-                                    "segmentation_curated": bool,
-                                    "label_curated": bool,
-                                }
-                            )
 
-                            user_metadata.reset_index(drop=True, inplace=True)
-                            file_metadata.reset_index(drop=True, inplace=True)
+                                user_metadata = user_metadata.astype(
+                                    {
+                                        "segmented": bool,
+                                        "labelled": bool,
+                                        "segmentation_curated": bool,
+                                        "label_curated": bool,
+                                    }
+                                )
 
-                            if akseg_hash in metadata_akseg_hash:
-                                user_metadata = pd.concat(
-                                    (user_metadata, file_metadata),
-                                    ignore_index=True,
-                                    axis=0,
-                                ).reset_index(drop=True)
-                                user_metadata.drop_duplicates(
-                                    subset=["akseg_hash"],
-                                    keep="last",
-                                    inplace=True,
+                                user_metadata.reset_index(
+                                    drop=True, inplace=True
+                                )
+                                file_metadata.reset_index(
+                                    drop=True, inplace=True
                                 )
 
-                            else:
-                                user_metadata = pd.concat(
-                                    (user_metadata, file_metadata),
-                                    ignore_index=True,
-                                    axis=0,
-                                ).reset_index(drop=True)
+                                user_metadata = user_metadata.loc[
+                                    :, ~user_metadata.columns.duplicated()
+                                ].copy()
+                                file_metadata = file_metadata.loc[
+                                    :, ~file_metadata.columns.duplicated()
+                                ].copy()
+
+                                for column in user_metadata.columns.tolist():
+                                    if (
+                                        column
+                                        not in file_metadata.columns.tolist()
+                                    ):
+                                        file_metadata[column] = ""
+
+                                if akseg_hash in metadata_akseg_hash:
+                                    user_metadata = pd.concat(
+                                        (user_metadata, file_metadata),
+                                        ignore_index=True,
+                                        axis=0,
+                                    )  # .reset_index(drop=True)
+                                    user_metadata.drop_duplicates(
+                                        subset=["akseg_hash"],
+                                        keep="last",
+                                        inplace=True,
+                                    )
+
+                                else:
+                                    user_metadata = pd.concat(
+                                        (user_metadata, file_metadata),
+                                        ignore_index=True,
+                                        axis=0,
+                                    ).reset_index(drop=True)
 
-                    user_metadata = user_metadata.astype("str")
+                    if upload_metadata is True:
+                        user_metadata = user_metadata.astype("str")
 
-                    user_metadata.drop_duplicates(
-                        subset=["akseg_hash"], keep="first", inplace=True
-                    )
-                    user_metadata = user_metadata[expected_columns]
+                        user_metadata.drop_duplicates(
+                            subset=["akseg_hash"], keep="first", inplace=True
+                        )
+                        user_metadata = user_metadata[expected_columns]
 
-                    user_metadata.to_csv(
-                        user_metadata_path, sep=",", index=False
-                    )
+                        user_metadata.to_csv(
+                            user_metadata_path, sep=",", index=False
+                        )
 
     except:
         print(traceback.format_exc())
 
 
-def get_filtered_database_metadata(self):
+def read_user_metadata(self, user_metadata_path=""):
+    try:
+        if user_metadata_path == "":
+            database_path = self.database_path
+            user_initial = self.upload_initial.currentText()
 
-    database_metadata = {
-        "user_initial": self.upload_initial.currentText(),
-        "content": self.upload_content.currentText(),
-        "microscope": self.upload_microscope.currentText(),
-        "antibiotic": self.upload_antibiotic.currentText(),
-        "antibiotic concentration": self.upload_abxconcentration.currentText(),
-        "treatment time (mins)": self.upload_treatmenttime.currentText(),
-        "mounting method": self.upload_mount.currentText(),
-        "protocol": self.upload_protocol.currentText(),
-    }
+            user_metadata_path = os.path.join(
+                database_path,
+                "Images",
+                user_initial,
+                f"{user_initial}_file_metadata.txt",
+            )
 
-    num_user_keys = self.user_metadata_keys
+        if os.path.isfile(user_metadata_path) == False:
+            if self.widget_notifications:
+                show_info("Could not find metadata for user: " + user_initial)
 
-    for key in range(1, num_user_keys + 1):
-        control_name = f"upload_usermeta{key}"
-        combo_box = getattr(self, control_name)
-        combo_box_text = combo_box.currentText()
-        database_metadata[f"user_meta{key}"] = combo_box_text
+            measurements = []
+            file_paths = []
+            channels = []
+
+        else:
+            sniffer = Sniffer()
 
-    database_metadata = {
-        key: val
-        for key, val in database_metadata.items()
-        if val not in ["", "Required for upload", 'example_item1', 'example_item2', 'example_item3']
-    }
+            # checks the delimiter of the metadata file
 
-    database_path = self.database_path
+            with open(user_metadata_path) as f:
+                for row in range(10):
+                    line = next(f).strip()
+                    delim = sniffer.sniff(line)
 
-    user_initial = database_metadata["user_initial"]
+            user_metadata = pd.read_csv(
+                user_metadata_path, sep=delim.delimiter, low_memory=False
+            )
 
-    user_metadata_path = os.path.join(
-        database_path,
-        "Images",
-        user_initial,
-        f"{user_initial}_file_metadata.txt",
-    )
+            user_metadata, expected_columns = check_metadata_format(
+                user_metadata, self.metadata_columns
+            )
 
-    if os.path.isfile(user_metadata_path) == False:
-        if self.widget_notifications:
-            show_info("Could not find metadata for user: " + user_initial)
-
-        measurements = []
-        file_paths = []
-        channels = []
+            user_metadata["segmentation_channel"] = user_metadata[
+                "segmentation_channel"
+            ].astype(str)
 
-    else:
-        user_metadata = pd.read_csv(
-            user_metadata_path, sep=",", low_memory=False
+            self.user_metadata = user_metadata
+            self.expected_columns = expected_columns
+
+    except:
+        user_metadata = None
+
+    return user_metadata, expected_columns
+
+
+def backup_user_metadata(self, user_metadata=""):
+    try:
+        if type(user_metadata) is str:
+            user_metadata, _ = read_user_metadata(self)
+
+        database_path = self.database_path
+
+        user_initial = self.upload_initial.currentText()
+
+        todays_date = datetime.datetime.now().strftime("%y%m%d-%H%M")
+
+        user_metadata_path = os.path.join(
+            database_path,
+            "Images",
+            user_initial,
+            "file metadata backup",
+            f"{user_initial}_file_metadata_{todays_date}.txt",
         )
 
-        user_metadata, expected_columns = check_metadata_format(
-            user_metadata, self.metadata_columns
+        if os.path.exists(os.path.dirname(user_metadata_path)) == False:
+            os.makedirs(os.path.dirname(user_metadata_path))
+
+        user_metadata = user_metadata.astype("str")
+
+        user_metadata.drop_duplicates(
+            subset=["akseg_hash"], keep="first", inplace=True
         )
 
-        user_metadata["segmentation_channel"] = user_metadata[
-            "segmentation_channel"
-        ].astype(str)
-
-        for key, value in database_metadata.items():
-            user_metadata = user_metadata[user_metadata[key] == value]
-
-        if self.upload_segmentation_combo.currentIndex() == 1:
-            user_metadata = user_metadata[user_metadata["segmented"] == False]
-        if self.upload_segmentation_combo.currentIndex() == 2:
-            user_metadata = user_metadata[user_metadata["segmented"] == True]
-        if self.upload_segmentation_combo.currentIndex() == 3:
-            user_metadata = user_metadata[
-                (user_metadata["segmented"] == True)
-                & (user_metadata["segmentation_curated"] == True)
-            ]
-        if self.upload_label_combo.currentIndex() == 1:
-            user_metadata = user_metadata[user_metadata["labelled"] == False]
-        if self.upload_label_combo.currentIndex() == 2:
-            user_metadata = user_metadata[user_metadata["labelled"] == False]
-        if self.upload_label_combo.currentIndex() == 3:
-            user_metadata = user_metadata[
-                (user_metadata["labelled"] == False)
-                & (user_metadata["label_curated"] == True)
+        show_info("Creating metadata backup for user: " + user_initial)
+
+        user_metadata.to_csv(user_metadata_path, sep=",", index=False)
+
+    except:
+        print(traceback.format_exc())
+
+
+def get_filtered_database_metadata(self):
+    try:
+        database_metadata = {
+            "user_initial": self.upload_initial.currentText(),
+            "content": self.upload_content.currentText(),
+            "microscope": self.upload_microscope.currentText(),
+            "phenotype": self.upload_phenotype.currentText(),
+            "strain": self.upload_strain.currentText(),
+            "antibiotic": self.upload_antibiotic.currentText(),
+            "antibiotic concentration": self.upload_abxconcentration.currentText(),
+            "treatment time (mins)": self.upload_treatmenttime.currentText(),
+            "mounting method": self.upload_mount.currentText(),
+            "protocol": self.upload_protocol.currentText(),
+        }
+
+        num_user_keys = self.user_metadata_keys
+
+        for key in range(1, num_user_keys + 1):
+            control_name = f"upload_usermeta{key}"
+            combo_box = getattr(self, control_name)
+            combo_box_text = combo_box.currentText()
+            database_metadata[f"user_meta{key}"] = combo_box_text
+
+        database_metadata = {
+            key: val
+            for key, val in database_metadata.items()
+            if val
+            not in [
+                "",
+                "Required for upload",
+                "example_item1",
+                "example_item2",
+                "example_item3",
             ]
+        }
+
+        database_path = self.database_path
 
-        user_metadata.sort_values(by=["posX", "posY", "posZ"], ascending=True)
+        user_initial = database_metadata["user_initial"]
 
-        if self.download_sort_order.currentIndex() == 0:
-            user_metadata = user_metadata.sample(frac=1).reset_index(drop=True)
-        if self.download_sort_order.currentIndex() == 1:
-            user_metadata = user_metadata.sort_values(
-                ["date_uploaded"], ascending=True
-            ).reset_index(drop=True)
-        if self.download_sort_order.currentIndex() == 2:
-            user_metadata = user_metadata.sort_values(
-                ["date_uploaded"], ascending=False
-            ).reset_index(drop=True)
-        if self.download_sort_order.currentIndex() == 3:
-            user_metadata = user_metadata.sort_values(
-                ["date_modified"], ascending=True
-            ).reset_index(drop=True)
-        if self.download_sort_order.currentIndex() == 4:
-            user_metadata = user_metadata.sort_values(
-                ["date_modified"], ascending=False
-            ).reset_index(drop=True)
+        user_metadata_path = os.path.join(
+            database_path,
+            "Images",
+            user_initial,
+            f"{user_initial}_file_metadata.txt",
+        )
 
-        import_limit = self.database_download_limit.currentText()
+        if os.path.isfile(user_metadata_path) == False:
+            if self.widget_notifications:
+                show_info("Could not find metadata for user: " + user_initial)
 
-        segmentation_files = user_metadata["segmentation_file"].unique()
-        num_measurements = len(segmentation_files)
+            measurements = []
+            file_paths = []
+            channels = []
 
-        if import_limit == "All":
-            import_limit = num_measurements
         else:
-            if int(import_limit) > num_measurements:
-                import_limit = num_measurements
+            user_metadata, expected_columns = read_user_metadata(self)
+
+            user_metadata["segmentation_channel"] = user_metadata[
+                "segmentation_channel"
+            ].astype(str)
+
+            for key, value in database_metadata.items():
+                if key in user_metadata.columns:
+                    user_metadata = user_metadata[user_metadata[key] == value]
+
+            if self.upload_segmentation_combo.currentIndex() == 1:
+                user_metadata = user_metadata[
+                    user_metadata["segmented"] == False
+                ]
+            if self.upload_segmentation_combo.currentIndex() == 2:
+                user_metadata = user_metadata[
+                    user_metadata["segmented"]
+                    == True & (user_metadata["segmentation_curated"] == False)
+                ]
+            if self.upload_segmentation_combo.currentIndex() == 3:
+                user_metadata = user_metadata[
+                    (user_metadata["segmented"] == True)
+                    & (user_metadata["segmentation_curated"] == True)
+                ]
+            if self.upload_label_combo.currentIndex() == 1:
+                user_metadata = user_metadata[
+                    user_metadata["labelled"] == False
+                ]
+            if self.upload_label_combo.currentIndex() == 2:
+                user_metadata = user_metadata[
+                    user_metadata["labelled"]
+                    == True & (user_metadata["label_curated"] == False)
+                ]
+            if self.upload_label_combo.currentIndex() == 3:
+                user_metadata = user_metadata[
+                    (user_metadata["labelled"] == True)
+                    & (user_metadata["label_curated"] == True)
+                ]
 
-        user_metadata = user_metadata[
-            user_metadata["segmentation_file"].isin(
-                segmentation_files[: int(import_limit)]
+            user_metadata.sort_values(
+                by=["posX", "posY", "posZ"], ascending=True
             )
-        ]
 
-        user_metadata["path"] = user_metadata["image_save_path"]
+            sort_names = []
+            sort_directions = []
+
+            if self.download_sort_order_1.currentIndex() > 1:
+                if self.download_sort_direction_1.currentIndex() == 1:
+                    sort_directions.append(True)
+                if self.download_sort_direction_1.currentIndex() == 2:
+                    sort_directions.append(False)
+
+            if self.download_sort_order_2.currentIndex() > 1:
+                if self.download_sort_direction_2.currentIndex() == 1:
+                    sort_directions.append(True)
+                if self.download_sort_direction_2.currentIndex() == 2:
+                    sort_directions.append(False)
+
+            if self.download_sort_order_1.currentIndex() == 1:
+                user_metadata = user_metadata.sample(frac=1).reset_index(
+                    drop=True
+                )
+            if self.download_sort_order_1.currentIndex() == 2:
+                sort_names.append("date_uploaded")
+            if self.download_sort_order_1.currentIndex() == 3:
+                sort_names.append("date_modified")
+            if self.download_sort_order_1.currentIndex() == 4:
+                if "image_laplacian" in user_metadata.columns:
+                    sort_names.append("image_laplacian")
+            if self.download_sort_order_1.currentIndex() == 5:
+                if "num_segmentations" in user_metadata.columns:
+                    sort_names.append("num_segmentations")
+            if self.download_sort_order_1.currentIndex() == 6:
+                if "image_focus" in user_metadata.columns:
+                    sort_names.append("image_focus")
+            if self.download_sort_order_1.currentIndex() == 7:
+                if "image_debris" in user_metadata.columns:
+                    sort_names.append("image_debris")
+
+            if self.download_sort_order_2.currentIndex() == 1:
+                user_metadata = user_metadata.sample(frac=1).reset_index(
+                    drop=True
+                )
+            if self.download_sort_order_2.currentIndex() == 2:
+                sort_names.append("date_uploaded")
+            if self.download_sort_order_2.currentIndex() == 3:
+                sort_names.append("date_modified")
+            if self.download_sort_order_2.currentIndex() == 4:
+                if "image_laplacian" in user_metadata.columns:
+                    sort_names.append("image_laplacian")
+            if self.download_sort_order_2.currentIndex() == 5:
+                if "num_segmentations" in user_metadata.columns:
+                    sort_names.append("num_segmentations")
+            if self.download_sort_order_2.currentIndex() == 6:
+                if "image_focus" in user_metadata.columns:
+                    sort_names.append("image_focus")
+            if self.download_sort_order_2.currentIndex() == 7:
+                if "image_debris" in user_metadata.columns:
+                    sort_names.append("image_debris")
+
+            if len(sort_names) > 0:
+                if len(sort_names) != len(sort_directions):
+                    sort_directions = [False] * len(sort_names)
+                user_metadata = user_metadata.sort_values(
+                    sort_names, ascending=sort_directions
+                ).reset_index(drop=True)
+
+            import_limit = self.database_download_limit.currentText()
 
-        channels = user_metadata["channel"].unique().tolist()
-        file_paths = user_metadata["image_save_path"].tolist()
+            segmentation_files = user_metadata["segmentation_file"].unique()
+            num_measurements = len(segmentation_files)
 
-        measurements = user_metadata.groupby(["folder", "segmentation_file"])
+            if import_limit == "All":
+                import_limit = num_measurements
+            else:
+                if int(import_limit) > num_measurements:
+                    import_limit = num_measurements
+
+            user_metadata = user_metadata[
+                user_metadata["segmentation_file"].isin(
+                    segmentation_files[: int(import_limit)]
+                )
+            ]
+
+            user_metadata["path"] = user_metadata["image_save_path"]
+
+            channels = user_metadata["channel"].unique().tolist()
+            file_paths = user_metadata["image_save_path"].tolist()
+
+            len1 = len(user_metadata)
+
+            user_metadata = user_metadata[
+                ~user_metadata["segmentation_file"].isin(
+                    ["None", None, np.nan]
+                )
+            ]
+            user_metadata = user_metadata[
+                ~user_metadata["folder"].isin(["None", None, np.nan])
+            ]
+
+            len2 = len(user_metadata)
+
+            if len2 < len1:
+                show_info(
+                    f"{len1 - len2} files with missing critical metadata removed."
+                )
+
+            sort_columns = []
+
+            if "folder" in user_metadata.columns:
+                sort_columns.append("folder")
+                user_metadata.loc[
+                    user_metadata["folder"].isna(), "folder"
+                ] = "None"
+            if "segmentation_file" in user_metadata.columns:
+                sort_columns.append("segmentation_file")
+                user_metadata.loc[
+                    user_metadata["segmentation_file"].isna(),
+                    "segmentation_file",
+                ] = "None"
+            if "posX" in user_metadata.columns:
+                sort_columns.append("posX")
+                user_metadata.loc[user_metadata["posX"].isna(), "posX"] = 0
+            if "posY" in user_metadata.columns:
+                sort_columns.append("posY")
+                user_metadata.loc[user_metadata["posY"].isna(), "posY"] = 0
+            if "posZ" in user_metadata.columns:
+                sort_columns.append("posZ")
+                user_metadata.loc[user_metadata["posZ"].isna(), "posZ"] = 0
+
+            measurements = user_metadata.groupby(sort_columns)
+
+    except:
+        print(traceback.format_exc())
+        measurements, file_paths, channels = None, None, None
 
     return measurements, file_paths, channels
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_imagej.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_imagej.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_interface_events.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_interface_events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,525 +1,565 @@
+import os
+import tempfile
 import traceback
 
-import numpy as np
 import cv2
-from colicoords import Data, Cell, CellPlot, data_to_cells
-import tempfile
-import os
+import numpy as np
 from napari.utils.notifications import show_info
 
-def find_contours(img):
 
+def find_contours(img):
     # finds contours of shapes, only returns the external contours of the shapes
-    contours, hierarchy = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)
+    contours, hierarchy = cv2.findContours(
+        img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
+    )
     contours = sorted(contours, key=cv2.contourArea, reverse=True)
     return contours
 
+
 def fill_holes(mask, colour):
+    try:
+        fill_mask = mask.copy()
+        fill_mask[fill_mask != colour] = 0
+        fill_mask[fill_mask == colour] == 255
+        fill_mask = fill_mask.astype(np.uint8)
 
-    fill_mask = mask.copy()
-    fill_mask[fill_mask != colour] = 0
-    fill_mask[fill_mask == colour] == 255
-    fill_mask = fill_mask.astype(np.uint8)
+        cnt = find_contours(fill_mask.astype(np.uint8))
+        cv2.drawContours(fill_mask, [cnt[0]], -1, 255, -1)
 
-    cnt = find_contours(fill_mask.astype(np.uint8))
-    cv2.drawContours(fill_mask, [cnt[0]], -1, 255, -1)
+        mask[fill_mask == 255] = colour
 
-    mask[fill_mask == 255] = colour
+    except:
+        pass
 
     return mask
 
 
-
 def _segmentationEvents(self, viewer, event):
+    try:
+        if "Control" in event.modifiers:
+            self._modifyMode(mode="delete")
 
-    if "Control" in event.modifiers:
-        self._modifyMode(mode="delete")
-
-    if "Shift" in event.modifiers:
-        self._modifyMode(mode="add")
-
-    if self.interface_mode == "segment":
-
-        # add segmentation
-        if self.segmentation_mode in ["add", "extend"]:
-
-            self.segLayer.mode = "paint"
-            self.segLayer.brush_size = 1
-
-            stored_mask = self.segLayer.data.copy()
-            stored_class = self.classLayer.data.copy()
-            meta = self.segLayer.metadata.copy()
+        if "Shift" in event.modifiers:
+            self._modifyMode(mode="add")
 
-            if self.segmentation_mode == "add":
-                new_colour = _newSegColour(self)
-            else:
-                data_coordinates = self.segLayer.world_to_data(event.position)
-                coord = np.round(data_coordinates).astype(int)
-                new_colour = self.segLayer.get_value(coord)
+        if self.interface_mode == "segment":
+            # add segmentation
+            if self.segmentation_mode in ["add", "extend"]:
+                self.segLayer.mode = "paint"
+                self.segLayer.brush_size = 1
 
-                self.segLayer.selected_label = new_colour
-                new_colour = self.segLayer.get_value(coord)
+                stored_mask = self.segLayer.data.copy()
+                stored_class = self.classLayer.data.copy()
+                meta = self.segLayer.metadata.copy()
 
-                new_class = self.classLayer.get_value(coord)
+                if self.segmentation_mode == "add":
+                    new_colour = _newSegColour(self)
+                else:
+                    data_coordinates = self.segLayer.world_to_data(
+                        event.position
+                    )
+                    coord = np.round(data_coordinates).astype(int)
+                    new_colour = self.segLayer.get_value(coord)
+
+                    self.segLayer.selected_label = new_colour
+                    new_colour = self.segLayer.get_value(coord)
 
-                if new_class != None:
-                    self.class_colour = new_class
+                    new_class = self.classLayer.get_value(coord)
 
-            dragged = False
-            coordinates = []
+                    if new_class != None:
+                        self.class_colour = new_class
 
-            yield
+                dragged = False
+                coordinates = []
 
-            # # on move
-            while event.type == 'mouse_move':
-                coordinates.append(event.position)
-                dragged = True
                 yield
 
-            # on release
-            if dragged:
-
-                if new_colour != 0 and new_colour != None and self.class_colour != None:
-
-                    coordinates = np.round(np.array(coordinates)).astype(np.int32)
-
-                    mask_dim = tuple(list(coordinates[0][:-2]) + [...])
-
-                    cnt = coordinates[:, -2:]
-
-                    cnt = np.fliplr(cnt)
-                    cnt = cnt.reshape((-1, 1, 2))
-
-                    seg_stack = self.segLayer.data
-
-                    seg_mask = seg_stack[mask_dim]
-
-                    cv2.drawContours(seg_mask, [cnt], -1, int(new_colour), -1)
+                # # on move
+                while event.type == "mouse_move":
+                    coordinates.append(event.position)
+                    dragged = True
+                    yield
 
-                    seg_mask = fill_holes(seg_mask, new_colour)
+                # on release
+                if dragged:
+                    if (
+                        new_colour != 0
+                        and new_colour != None
+                        and self.class_colour != None
+                    ):
+                        coordinates = np.round(np.array(coordinates)).astype(
+                            np.int32
+                        )
 
-                    seg_stack[mask_dim] = seg_mask
+                        mask_dim = tuple(list(coordinates[0][:-2]) + [...])
 
-                    self.segLayer.data = seg_stack
+                        cnt = coordinates[:, -2:]
 
-                    # update class
+                        cnt = np.fliplr(cnt)
+                        cnt = cnt.reshape((-1, 1, 2))
 
-                    class_stack = self.classLayer.data
-                    class_colour = self.class_colour
-                    seg_stack = self.segLayer.data
+                        seg_stack = self.segLayer.data
 
-                    seg_mask = seg_stack[mask_dim]
-                    class_mask = class_stack[mask_dim]
+                        seg_mask = seg_stack[mask_dim]
 
-                    class_mask[seg_mask == int(new_colour)] = class_colour
-                    class_stack[mask_dim] = class_mask
+                        cv2.drawContours(
+                            seg_mask, [cnt], -1, int(new_colour), -1
+                        )
 
-                    self.classLayer.data = class_stack
+                        seg_mask = fill_holes(seg_mask, new_colour)
 
-                    # update metadata
+                        seg_stack[mask_dim] = seg_mask
 
-                    meta["manual_segmentation"] = True
-                    self.segLayer.metadata = meta
-                    self.segLayer.mode = "pan_zoom"
-                    self.update_image_folds()
+                        self.segLayer.data = seg_stack
 
-                else:
-                    self.segLayer.data = stored_mask
-                    self.classLayer.data = stored_class
-                    self.segLayer.mode = "pan_zoom"
+                        # update class
 
-        # join segmentations
-        if self.segmentation_mode == "join":
+                        class_stack = self.classLayer.data
+                        class_colour = self.class_colour
+                        seg_stack = self.segLayer.data
 
-            self.segLayer.mode = "paint"
-            self.segLayer.brush_size = 1
+                        seg_mask = seg_stack[mask_dim]
+                        class_mask = class_stack[mask_dim]
 
-            stored_mask = self.segLayer.data.copy()
-            stored_class = self.classLayer.data.copy()
-            meta = self.segLayer.metadata.copy()
+                        class_mask[seg_mask == int(new_colour)] = class_colour
+                        class_stack[mask_dim] = class_mask
 
-            data_coordinates = self.segLayer.world_to_data(event.position)
-            coord = np.round(data_coordinates).astype(int)
-            new_colour = self.segLayer.get_value(coord)
+                        self.classLayer.data = class_stack
 
-            self.segLayer.selected_label = new_colour
-            new_colour = self.segLayer.get_value(coord)
+                        # update metadata
 
-            new_class = self.classLayer.get_value(coord)
+                        meta["manual_segmentation"] = True
+                        self.segLayer.metadata = meta
+                        self.segLayer.mode = "pan_zoom"
+                        self.update_image_folds()
 
-            if new_class != None:
-                self.class_colour = new_class
+                    else:
+                        self.segLayer.data = stored_mask
+                        self.classLayer.data = stored_class
+                        self.segLayer.mode = "pan_zoom"
 
+            # join segmentations
+            if self.segmentation_mode == "join":
+                self.segLayer.mode = "paint"
+                self.segLayer.brush_size = 1
 
-            dragged = False
-            colours = []
-            classes = []
-            coords = []
-            yield
+                stored_mask = self.segLayer.data.copy()
+                stored_class = self.classLayer.data.copy()
+                meta = self.segLayer.metadata.copy()
 
-            # on move
-            while event.type == 'mouse_move':
                 data_coordinates = self.segLayer.world_to_data(event.position)
                 coord = np.round(data_coordinates).astype(int)
-                mask_val = self.segLayer.get_value(coord)
-                class_val = self.classLayer.get_value(coord)
-                colours.append(mask_val)
-                classes.append(class_val)
-                coords.append(coord)
-                dragged = True
-                yield
-
-            # on release
-            if dragged:
-
-                colours = np.array(colours)
-                colours = np.unique(colours)
-                colours = np.delete(colours, np.where(colours == 0))
-
-                if new_colour in colours:
-                    colours = np.delete(colours, np.where(colours == new_colour))
-
-                if len(colours) == 1 and new_colour not in colours and new_colour != None:
+                new_colour = self.segLayer.get_value(coord)
 
-                    mask_stack = self.segLayer.data
+                self.segLayer.selected_label = new_colour
+                new_colour = self.segLayer.get_value(coord)
 
-                    mask_dim = tuple(list(coords[0][:-2]) + [...])
+                new_class = self.classLayer.get_value(coord)
 
-                    mask = mask_stack[mask_dim]
+                if new_class != None:
+                    self.class_colour = new_class
 
-                    mask[mask == colours[0]] = new_colour
+                dragged = False
+                colours = []
+                classes = []
+                coords = []
+                yield
 
-                    mask = fill_holes(mask,new_colour)
+                # on move
+                while event.type == "mouse_move":
+                    data_coordinates = self.segLayer.world_to_data(
+                        event.position
+                    )
+                    coord = np.round(data_coordinates).astype(int)
+                    mask_val = self.segLayer.get_value(coord)
+                    class_val = self.classLayer.get_value(coord)
+                    colours.append(mask_val)
+                    classes.append(class_val)
+                    coords.append(coord)
+                    dragged = True
+                    yield
 
-                    mask_stack[mask_dim] = mask
+                # on release
+                if dragged:
+                    colours = np.array(colours)
+                    colours = np.unique(colours)
+                    colours = np.delete(colours, np.where(colours == 0))
 
-                    self.segLayer.data = mask_stack
+                    if new_colour in colours:
+                        colours = np.delete(
+                            colours, np.where(colours == new_colour)
+                        )
 
-                    # update class
+                    if (
+                        len(colours) == 1
+                        and new_colour not in colours
+                        and new_colour != None
+                    ):
+                        mask_stack = self.segLayer.data
 
-                    class_stack = self.classLayer.data
-                    seg_stack = self.segLayer.data
+                        mask_dim = tuple(list(coords[0][:-2]) + [...])
 
-                    seg_mask = seg_stack[mask_dim]
-                    class_mask = class_stack[mask_dim]
+                        mask = mask_stack[mask_dim]
 
-                    class_mask[seg_mask == new_colour] = 2
-                    class_stack[mask_dim] = class_mask
+                        mask[mask == colours[0]] = new_colour
 
-                    self.classLayer.data = class_stack
+                        mask = fill_holes(mask, new_colour)
 
-                    # update metadata
+                        mask_stack[mask_dim] = mask
 
-                    meta["manual_segmentation"] = True
-                    self.segLayer.metadata = meta
-                    self.segLayer.mode = "pan_zoom"
-                    self.update_image_folds()
+                        self.segLayer.data = mask_stack
 
+                        # update class
 
-                else:
+                        class_stack = self.classLayer.data
+                        seg_stack = self.segLayer.data
 
-                    self.segLayer.data = stored_mask
-                    self.classLayer.data = stored_class
-                    self.segLayer.mode = "pan_zoom"
+                        seg_mask = seg_stack[mask_dim]
+                        class_mask = class_stack[mask_dim]
 
-        # split segmentations
-        if self.segmentation_mode == "split":
+                        class_mask[seg_mask == new_colour] = 2
+                        class_stack[mask_dim] = class_mask
 
-            self.segLayer.mode = "paint"
-            self.segLayer.brush_size = 1
+                        self.classLayer.data = class_stack
 
-            new_colour = _newSegColour(self)
-            stored_mask = self.segLayer.data.copy()
-            stored_class = self.classLayer.data
-            meta = self.segLayer.metadata.copy()
-
-            dragged = False
-            colours = []
-            yield
+                        # update metadata
 
-            # on move
-            while event.type == 'mouse_move':
-                data_coordinates = self.segLayer.world_to_data(event.position)
-                coords = np.round(data_coordinates).astype(int)
-                mask_val = self.segLayer.get_value(coords)
-                colours.append(mask_val)
-                dragged = True
-                yield
-
-            # on release
-            if dragged:
-
-                colours = np.array(colours)
-                colours = np.delete(colours, np.where(colours == new_colour))
-
-                colours[colours==None] = 0
-
-                num_colours = len(np.unique(colours))
-
-                if num_colours == 2 or num_colours == 3:
+                        meta["manual_segmentation"] = True
+                        self.segLayer.metadata = meta
+                        self.segLayer.mode = "pan_zoom"
+                        self.update_image_folds()
 
-                    if num_colours == 2:
-                        maskref = colours[colours != 0][0]
                     else:
-                        maskref = sorted(set(colours.tolist()), key=lambda x: colours.tolist().index(x))[1]
-
-                    bisection = colours[0] != maskref and colours[-1] != maskref
-
-                    if bisection and new_colour != None:
-
-                        mask_dim = tuple(list(coords[:-2]) + [...])
-                        shape_mask = stored_mask[mask_dim].copy()
-
-                        class_mask = stored_class[mask_dim].copy()
-                        class_mask[shape_mask == maskref] = 3
-                        stored_class[mask_dim] = class_mask
-                        self.classLayer.data = stored_class
-
-                        shape_mask[shape_mask != maskref] = 0
-                        shape_mask[shape_mask == maskref] = 255
-                        shape_mask = shape_mask.astype(np.uint8)
-
-                        line_mask = self.segLayer.data.copy()
-                        line_mask = line_mask[mask_dim]
-                        line_mask[line_mask != new_colour] = 0
-                        line_mask[line_mask == new_colour] = 255
-                        line_mask = line_mask.astype(np.uint8)
-
-                        overlap = cv2.bitwise_and(shape_mask, line_mask)
-
-                        shape_mask_split = cv2.bitwise_xor(shape_mask, overlap).astype(np.uint8)
-
-                        # update labels layers with split shape
-                        split_mask = stored_mask[mask_dim]
-                        split_mask[overlap == 255] = new_colour
-                        stored_mask[mask_dim] = split_mask
                         self.segLayer.data = stored_mask
+                        self.classLayer.data = stored_class
+                        self.segLayer.mode = "pan_zoom"
 
-                        # fill one have of the split shape with the new colour
-                        indices = np.where(shape_mask_split == 255)
-                        split_dim = list(list(mask_dim[:-1]) + [indices[0][0], indices[1][0]])
-                        split_dim = np.array(split_dim).flatten().tolist()
+            # split segmentations
+            if self.segmentation_mode == "split":
+                self.segLayer.mode = "paint"
+                self.segLayer.brush_size = 1
 
-                        self.segLayer.fill(split_dim, new_colour)
+                new_colour = _newSegColour(self)
+                stored_mask = self.segLayer.data.copy()
+                stored_class = self.classLayer.data
+                meta = self.segLayer.metadata.copy()
 
-                        meta["manual_segmentation"] = True
-                        self.segLayer.metadata = meta
-                        self.segLayer.mode = "pan_zoom"
-                        self.update_image_folds()
+                dragged = False
+                colours = []
+                yield
 
+                # on move
+                while event.type == "mouse_move":
+                    data_coordinates = self.segLayer.world_to_data(
+                        event.position
+                    )
+                    coords = np.round(data_coordinates).astype(int)
+                    mask_val = self.segLayer.get_value(coords)
+                    colours.append(mask_val)
+                    dragged = True
+                    yield
+
+                # on release
+                if dragged:
+                    colours = np.array(colours)
+                    colours = np.delete(
+                        colours, np.where(colours == new_colour)
+                    )
+
+                    colours[colours == None] = 0
+
+                    num_colours = len(np.unique(colours))
+
+                    if num_colours == 2 or num_colours == 3:
+                        if num_colours == 2:
+                            maskref = colours[colours != 0][0]
+                        else:
+                            maskref = sorted(
+                                set(colours.tolist()),
+                                key=lambda x: colours.tolist().index(x),
+                            )[1]
+
+                        bisection = (
+                            colours[0] != maskref and colours[-1] != maskref
+                        )
+
+                        if bisection and new_colour != None:
+                            mask_dim = tuple(list(coords[:-2]) + [...])
+                            shape_mask = stored_mask[mask_dim].copy()
+
+                            class_mask = stored_class[mask_dim].copy()
+                            class_mask[shape_mask == maskref] = 3
+                            stored_class[mask_dim] = class_mask
+                            self.classLayer.data = stored_class
+
+                            shape_mask[shape_mask != maskref] = 0
+                            shape_mask[shape_mask == maskref] = 255
+                            shape_mask = shape_mask.astype(np.uint8)
+
+                            line_mask = self.segLayer.data.copy()
+                            line_mask = line_mask[mask_dim]
+                            line_mask[line_mask != new_colour] = 0
+                            line_mask[line_mask == new_colour] = 255
+                            line_mask = line_mask.astype(np.uint8)
+
+                            overlap = cv2.bitwise_and(shape_mask, line_mask)
+
+                            shape_mask_split = cv2.bitwise_xor(
+                                shape_mask, overlap
+                            ).astype(np.uint8)
+
+                            # update labels layers with split shape
+                            split_mask = stored_mask[mask_dim]
+                            split_mask[overlap == 255] = new_colour
+                            stored_mask[mask_dim] = split_mask
+                            self.segLayer.data = stored_mask
+
+                            # fill one have of the split shape with the new colour
+                            indices = np.where(shape_mask_split == 255)
+                            split_dim = list(
+                                list(mask_dim[:-1])
+                                + [indices[0][0], indices[1][0]]
+                            )
+                            split_dim = np.array(split_dim).flatten().tolist()
+
+                            self.segLayer.fill(split_dim, new_colour)
+
+                            meta["manual_segmentation"] = True
+                            self.segLayer.metadata = meta
+                            self.segLayer.mode = "pan_zoom"
+                            self.update_image_folds()
+
+                        else:
+                            self.segLayer.data = stored_mask
+                            self.segLayer.mode = "pan_zoom"
                     else:
                         self.segLayer.data = stored_mask
                         self.segLayer.mode = "pan_zoom"
                 else:
                     self.segLayer.data = stored_mask
                     self.segLayer.mode = "pan_zoom"
-            else:
-                self.segLayer.data = stored_mask
-                self.segLayer.mode = "pan_zoom"
-
 
-        # delete segmentations
-        if self.segmentation_mode == "delete":
+            # delete segmentations
+            if self.segmentation_mode == "delete":
+                self.segLayer.mode = "paint"
+                self.segLayer.brush_size = 1
 
-            self.segLayer.mode = "paint"
-            self.segLayer.brush_size = 1
+                new_colour = _newSegColour(self)
+                stored_mask = self.segLayer.data.copy()
+                stored_class = self.classLayer.data
+                meta = self.segLayer.metadata.copy()
 
-            new_colour = _newSegColour(self)
-            stored_mask = self.segLayer.data.copy()
-            stored_class = self.classLayer.data
-            meta = self.segLayer.metadata.copy()
-
-            dragged = False
-            coordinates = []
-            yield
-
-            # on move
-            while event.type == 'mouse_move':
-                coordinates.append(event.position)
-                dragged = True
+                dragged = False
+                coordinates = []
                 yield
 
-            # on release
-            if dragged:
-
-                self.segLayer.data = stored_mask
-
-                coordinates = np.round(np.array(coordinates)).astype(np.int32)
-                cnt = coordinates[:, -2:]
+                # on move
+                while event.type == "mouse_move":
+                    coordinates.append(event.position)
+                    dragged = True
+                    yield
 
-                cnt = np.fliplr(cnt)
-                cnt = cnt.reshape((-1, 1, 2))
-
-                mask_dim = tuple(list(coordinates[0][:-2]) + [...])
-
-                seg_stack = self.segLayer.data.copy()
-                class_stack = self.classLayer.data.copy()
-
-                seg_mask = seg_stack[mask_dim]
-                class_mask = class_stack[mask_dim]
-
-                delete_mask = np.zeros_like(seg_mask)
-                cv2.drawContours(delete_mask, [cnt], -1, 255, -1)
-
-                delete_colours = np.unique(seg_mask[delete_mask==255])
-
-                for colour in delete_colours:
-                    seg_mask[seg_mask == colour] = 0
-
-                class_mask[seg_mask == 0] = 0
-
-                seg_stack[mask_dim] = seg_mask
-                class_stack[mask_dim] = class_mask
-
-                self.segLayer.data = seg_stack
-                self.classLayer.data = class_stack
-
-                pass
+                # on release
+                if dragged:
+                    self.segLayer.data = stored_mask
 
-            else:
+                    coordinates = np.round(np.array(coordinates)).astype(
+                        np.int32
+                    )
+                    cnt = coordinates[:, -2:]
 
-                self.segLayer.data = stored_mask
-                self.segLayer.mode = "pan_zoom"
-                self.update_image_folds()
+                    cnt = np.fliplr(cnt)
+                    cnt = cnt.reshape((-1, 1, 2))
 
-                meta = self.segLayer.metadata.copy()
+                    mask_dim = tuple(list(coordinates[0][:-2]) + [...])
 
-                data_coordinates = self.segLayer.world_to_data(event.position)
-                coord = np.round(data_coordinates).astype(int)
-                mask_val = self.segLayer.get_value(coord)
+                    seg_stack = self.segLayer.data.copy()
+                    class_stack = self.classLayer.data.copy()
 
-                if mask_val != 0:
+                    seg_mask = seg_stack[mask_dim]
+                    class_mask = class_stack[mask_dim]
 
-                    mask_dim = tuple(list(coord[:-2]) + [...])[0]
+                    delete_mask = np.zeros_like(seg_mask)
+                    cv2.drawContours(delete_mask, [cnt], -1, 255, -1)
 
-                    mask_stack = self.segLayer.data
-                    class_stack = self.classLayer.data
+                    delete_colours = np.unique(seg_mask[delete_mask == 255])
 
-                    mask = mask_stack[mask_dim]
-                    class_mask = class_stack[mask_dim]
+                    for colour in delete_colours:
+                        seg_mask[seg_mask == colour] = 0
 
-                    class_mask[mask == mask_val] = 0
-                    mask[mask == mask_val] = 0
+                    class_mask[seg_mask == 0] = 0
 
+                    seg_stack[mask_dim] = seg_mask
                     class_stack[mask_dim] = class_mask
-                    mask_stack[mask_dim] = mask
 
+                    self.segLayer.data = seg_stack
                     self.classLayer.data = class_stack
-                    self.segLayer.data = mask_stack
-
-                    # update metadata
 
-                    meta["manual_segmentation"] = True
-                    self.segLayer.metadata = meta
+                else:
+                    self.segLayer.data = stored_mask
                     self.segLayer.mode = "pan_zoom"
                     self.update_image_folds()
 
-        if self.segmentation_mode == "refine":
+                    meta = self.segLayer.metadata.copy()
 
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes","center_lines"]]
+                    data_coordinates = self.segLayer.world_to_data(
+                        event.position
+                    )
+                    coord = np.round(data_coordinates).astype(int)
+                    mask_val = self.segLayer.get_value(coord)
 
-            self.segLayer.mode == "pan_zoom"
-            self.segLayer.brush_size = 1
+                    if mask_val != 0:
+                        mask_dim = tuple(list(coord[:-2]) + [...])[0]
 
-            data_coordinates = self.segLayer.world_to_data(event.position)
-            coord = np.round(data_coordinates).astype(int)
-            mask_id = self.segLayer.get_value(coord)
+                        mask_stack = self.segLayer.data
+                        class_stack = self.classLayer.data
 
-            self.segLayer.selected_label = mask_id
+                        mask = mask_stack[mask_dim]
+                        class_mask = class_stack[mask_dim]
 
-            if mask_id != 0:
+                        class_mask[mask == mask_val] = 0
+                        mask[mask == mask_val] = 0
 
-                current_fov = self.viewer.dims.current_step[0]
+                        class_stack[mask_dim] = class_mask
+                        mask_stack[mask_dim] = mask
 
-                channel = self.refine_channel.currentText()
-                channel = channel.replace("Mask + ", "")
+                        self.classLayer.data = class_stack
+                        self.segLayer.data = mask_stack
 
-                label_stack = self.classLayer.data
-                mask_stack = self.segLayer.data
+                        # update metadata
 
-                mask = mask_stack[current_fov, :, :].copy()
-                label = label_stack[current_fov, :, :].copy()
-
-                image = []
-                for layer in layer_names:
-                    image.append(self.viewer.layers[layer].data[current_fov])
-                image = np.stack(image,axis=0)
-
-                cell_mask = np.zeros(mask.shape, dtype=np.uint8)
-
-                mask[mask != mask_id] = 0
-                cell_mask[mask != mask_id] = 0
-                cell_mask[mask == mask_id] = 1
+                        meta["manual_segmentation"] = True
+                        self.segLayer.metadata = meta
+                        self.segLayer.mode = "pan_zoom"
+                        self.update_image_folds()
 
-                from napari_bacseg._utils_statistics import get_cell_images
-                from napari_bacseg._utils_colicoords import run_colicoords, process_colicoords
+            if self.segmentation_mode == "refine":
+                layer_names = [
+                    layer.name
+                    for layer in self.viewer.layers
+                    if layer.name
+                    not in ["Segmentations", "Classes", "center_lines"]
+                ]
 
-                colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
+                self.segLayer.mode == "pan_zoom"
+                self.segLayer.brush_size = 1
 
-                cell_images_path = get_cell_images(self,image, mask, cell_mask, mask_id, layer_names, colicoords_dir)
+                data_coordinates = self.segLayer.world_to_data(event.position)
+                coord = np.round(data_coordinates).astype(int)
+                mask_id = self.segLayer.get_value(coord)
 
-                cell_data = {"cell_images_path":cell_images_path}
+                self.segLayer.selected_label = mask_id
 
-                colicoords_data = run_colicoords(self, cell_data=[cell_data],
-                                                 colicoords_channel=channel,
-                                                 multithreaded=True)
+                if mask_id != 0:
+                    current_fov = self.viewer.dims.current_step[0]
 
-                process_colicoords(self, colicoords_data)
+                    channel = self.refine_channel.currentText()
+                    channel = channel.replace("Mask + ", "")
 
-    if self.interface_mode == "classify":
+                    label_stack = self.classLayer.data
+                    mask_stack = self.segLayer.data
 
-        self.segLayer.mode == "pan_zoom"
-        self.segLayer.brush_size = 1
+                    mask = mask_stack[current_fov, :, :].copy()
+                    label = label_stack[current_fov, :, :].copy()
 
-        data_coordinates = self.segLayer.world_to_data(event.position)
-        coord = np.round(data_coordinates).astype(int)
-        mask_val = self.segLayer.get_value(coord).copy()
+                    image = []
+                    for layer in layer_names:
+                        image.append(
+                            self.viewer.layers[layer].data[current_fov]
+                        )
+                    image = np.stack(image, axis=0)
+
+                    cell_mask = np.zeros(mask.shape, dtype=np.uint8)
+
+                    mask[mask != mask_id] = 0
+                    cell_mask[mask != mask_id] = 0
+                    cell_mask[mask == mask_id] = 1
+
+                    from napari_bacseg._utils_colicoords import (
+                        process_colicoords,
+                        run_colicoords,
+                    )
+                    from napari_bacseg._utils_statistics import get_cell_images
+
+                    colicoords_dir = os.path.join(
+                        tempfile.gettempdir(), "colicoords"
+                    )
+
+                    cell_images_path = get_cell_images(
+                        self,
+                        image,
+                        mask,
+                        cell_mask,
+                        mask_id,
+                        layer_names,
+                        colicoords_dir,
+                    )
+
+                    cell_data = {"cell_images_path": cell_images_path}
+
+                    colicoords_data = run_colicoords(
+                        self,
+                        cell_data=[cell_data],
+                        colicoords_channel=channel,
+                        multithreaded=True,
+                    )
 
-        self.segLayer.selected_label = mask_val
+                    process_colicoords(self, colicoords_data)
 
-        if mask_val != 0:
+        if self.interface_mode == "classify":
+            self.segLayer.mode == "pan_zoom"
+            self.segLayer.brush_size = 1
 
-            stored_mask = self.segLayer.data.copy()
-            stored_class = self.classLayer.data.copy()
+            data_coordinates = self.segLayer.world_to_data(event.position)
+            coord = np.round(data_coordinates).astype(int)
+            mask_val = self.segLayer.get_value(coord).copy()
 
-            if len(stored_mask.shape) > 2:
+            self.segLayer.selected_label = mask_val
 
-                current_fov = self.viewer.dims.current_step[0]
+            if mask_val != 0:
+                stored_mask = self.segLayer.data.copy()
+                stored_class = self.classLayer.data.copy()
 
-                seg_mask = stored_mask[current_fov, :, :]
-                class_mask = stored_class[current_fov, :, :]
+                if len(stored_mask.shape) > 2:
+                    current_fov = self.viewer.dims.current_step[0]
 
-                class_mask[seg_mask == mask_val] = self.class_colour
+                    seg_mask = stored_mask[current_fov, :, :]
+                    class_mask = stored_class[current_fov, :, :]
 
-                stored_class[current_fov, :, :] = class_mask
+                    class_mask[seg_mask == mask_val] = self.class_colour
 
-                self.classLayer.data = stored_class
-                self.segLayer.mode = "pan_zoom"
+                    stored_class[current_fov, :, :] = class_mask
 
-            else:
+                    self.classLayer.data = stored_class
+                    self.segLayer.mode = "pan_zoom"
 
-                stored_class[stored_mask == mask_val] = self.class_colour
+                else:
+                    stored_class[stored_mask == mask_val] = self.class_colour
 
-                self.classLayer.data = stored_class
-                self.segLayer.mode = "pan_zoom"
+                    self.classLayer.data = stored_class
+                    self.segLayer.mode = "pan_zoom"
 
-    if self.interface_mode == "panzoom":
+        if self.interface_mode == "panzoom":
+            mouse_button = event.button
 
-        mouse_button = event.button
+            data_coordinates = self.segLayer.world_to_data(event.position)
+            coord = np.round(data_coordinates).astype(int)
 
-        data_coordinates = self.segLayer.world_to_data(event.position)
-        coord = np.round(data_coordinates).astype(int)
+        if self.modify_auto_panzoom.isChecked() == True:
+            self.interface_mode = "panzoom"
+            self.modify_panzoom.setEnabled(False)
+            self.modify_segment.setEnabled(True)
+            self.modify_classify.setEnabled(True)
 
-    if self.modify_auto_panzoom.isChecked() == True:
-        self._modifyMode(mode="panzoom")
+    except:
+        print(traceback.format_exc())
 
 
 def _newSegColour(self):
-
     mask_stack = self.segLayer.data
 
     current_fov = self.viewer.dims.current_step[0]
 
     if len(mask_stack.shape) > 2:
         mask = mask_stack[current_fov, :, :]
     else:
@@ -528,332 +568,200 @@
     colours = np.unique(mask)
     new_colour = max(colours) + 1
 
     self.segLayer.selected_label = new_colour
 
     return new_colour
 
-def _modifyMode(self, mode, viewer=None):
 
+def _modifyMode(self, mode, viewer=None):
     def _event(viewer):
-
         if mode == "panzoom":
             self.segLayer.mode = "pan_zoom"
 
-            self.modify_add.setEnabled(False)
-            self.modify_extend.setEnabled(False)
-            self.modify_join.setEnabled(False)
-            self.modify_split.setEnabled(False)
-            self.modify_delete.setEnabled(False)
-            self.modify_refine.setEnabled(False)
-
-            self.classify_single.setEnabled(False)
-            self.classify_dividing.setEnabled(False)
-            self.classify_divided.setEnabled(False)
-            self.classify_vertical.setEnabled(False)
-            self.classify_broken.setEnabled(False)
-            self.classify_edge.setEnabled(False)
-
             self.interface_mode = "panzoom"
             self.modify_panzoom.setEnabled(False)
             self.modify_panzoom.setEnabled(False)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(True)
 
         if mode == "segment":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(False)
-            self.modify_extend.setEnabled(True)
-            self.modify_join.setEnabled(True)
-            self.modify_split.setEnabled(True)
-            self.modify_delete.setEnabled(True)
-            self.modify_refine.setEnabled(True)
-
-            self.classify_single.setEnabled(True)
-            self.classify_dividing.setEnabled(False)
-            self.classify_divided.setEnabled(False)
-            self.classify_vertical.setEnabled(False)
-            self.classify_broken.setEnabled(False)
-            self.classify_edge.setEnabled(False)
-
-
             self.interface_mode = "segment"
             self.segmentation_mode = "add"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
             self.modify_classify.setEnabled(True)
 
         if mode == "classify":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(False)
-            self.modify_extend.setEnabled(False)
-            self.modify_join.setEnabled(False)
-            self.modify_split.setEnabled(False)
-            self.modify_delete.setEnabled(False)
-            self.modify_refine.setEnabled(False)
-
-            self.classify_single.setEnabled(False)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(True)
-
             self.interface_mode = "classify"
             self.segmentation_mode = "add"
             self.class_mode = 1
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
 
-        if mode == "add":
+        if mode == "clicktozoom":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(False)
-            self.modify_extend.setEnabled(True)
-            self.modify_join.setEnabled(True)
-            self.modify_split.setEnabled(True)
-            self.modify_delete.setEnabled(True)
-            self.modify_refine.setEnabled(True)
-
-            self.classify_single.setEnabled(False)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(True)
+            self.interface_mode = "segment"
+            self.segmentation_mode = "clicktozoom"
+            # self.modify_panzoom.setEnabled(True)
+            # self.modify_segment.setEnabled(True)
+            # self.modify_classify.setEnabled(True)
+
+        if mode == "add":
+            self.viewer.layers.selection.select_only(self.segLayer)
 
             self.interface_mode = "segment"
             self.segmentation_mode = "add"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
+            show_info("Add (click/drag to add)")
 
         if mode == "extend":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(True)
-            self.modify_extend.setEnabled(False)
-            self.modify_join.setEnabled(True)
-            self.modify_split.setEnabled(True)
-            self.modify_delete.setEnabled(True)
-            self.modify_refine.setEnabled(True)
-
             self.interface_mode = "segment"
             self.segmentation_mode = "extend"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
+            show_info("Extend (click/drag to extend)")
 
         if mode == "join":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(True)
-            self.modify_extend.setEnabled(True)
-            self.modify_join.setEnabled(False)
-            self.modify_split.setEnabled(True)
-            self.modify_delete.setEnabled(True)
-            self.modify_refine.setEnabled(True)
-
             self.interface_mode = "segment"
             self.segmentation_mode = "join"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
+            show_info("Join (click/drag to join)")
 
         if mode == "split":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(True)
-            self.modify_extend.setEnabled(True)
-            self.modify_join.setEnabled(True)
-            self.modify_split.setEnabled(False)
-            self.modify_delete.setEnabled(True)
-            self.modify_refine.setEnabled(True)
-
             self.interface_mode = "segment"
             self.segmentation_mode = "split"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
+            show_info("Split (click/drag to split)")
 
         if mode == "delete":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(True)
-            self.modify_extend.setEnabled(True)
-            self.modify_join.setEnabled(True)
-            self.modify_split.setEnabled(True)
-            self.modify_delete.setEnabled(False)
-            self.modify_refine.setEnabled(True)
-
             self.interface_mode = "segment"
             self.segmentation_mode = "delete"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
+            show_info("Delete (click/drag to delete)")
 
         if mode == "edit_vertex":
             self.viewer.layers.selection.select_only(self.shapeLayer)
 
             self.interface_mode = "shapes"
             self.segmentation_mode = "edit_vertex"
 
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
 
         if mode == "refine":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.modify_add.setEnabled(True)
-            self.modify_extend.setEnabled(True)
-            self.modify_join.setEnabled(True)
-            self.modify_split.setEnabled(True)
-            self.modify_delete.setEnabled(True)
-            self.modify_refine.setEnabled(False)
-
             self.interface_mode = "segment"
             self.segmentation_mode = "refine"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(False)
+            show_info("Refine (click to refine)")
 
         if self.interface_mode == "segment":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            if self.segmentation_mode == "add":
-
-                self.classify_single.setEnabled(False)
-                self.classify_dividing.setEnabled(True)
-                self.classify_divided.setEnabled(True)
-                self.classify_vertical.setEnabled(True)
-                self.classify_broken.setEnabled(True)
-                self.classify_edge.setEnabled(True)
-
-            else:
-
-                self.classify_single.setEnabled(False)
-                self.classify_dividing.setEnabled(False)
-                self.classify_divided.setEnabled(False)
-                self.classify_vertical.setEnabled(False)
-                self.classify_broken.setEnabled(False)
-                self.classify_edge.setEnabled(False)
-
         if mode == "single":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.classify_single.setEnabled(False)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(True)
-
             self.class_mode = mode
             self.class_colour = 1
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
+            show_info("Single (click to classify)")
 
         if mode == "dividing":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.classify_single.setEnabled(True)
-            self.classify_dividing.setEnabled(False)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(True)
-
             self.class_mode = mode
             self.class_colour = 2
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
+            show_info("Dividing (click to classify)")
 
         if mode == "divided":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.classify_single.setEnabled(True)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(False)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(True)
-
             self.class_mode = mode
             self.class_colour = 3
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
+            show_info("Divided (click to classify)")
 
         if mode == "vertical":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.classify_single.setEnabled(True)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(False)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(True)
-
             self.class_mode = mode
             self.class_colour = 4
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
+            show_info("Vertical (click to classify)")
 
         if mode == "broken":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.classify_single.setEnabled(True)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(False)
-            self.classify_edge.setEnabled(True)
-
             self.class_mode = mode
             self.class_colour = 5
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
+            show_info("Broken (click to classify)")
 
         if mode == "edge":
             self.viewer.layers.selection.select_only(self.segLayer)
 
-            self.classify_single.setEnabled(True)
-            self.classify_dividing.setEnabled(True)
-            self.classify_divided.setEnabled(True)
-            self.classify_vertical.setEnabled(True)
-            self.classify_broken.setEnabled(True)
-            self.classify_edge.setEnabled(False)
-
             self.class_mode = mode
             self.class_colour = 6
             self.interface_mode = "classify"
             self.modify_panzoom.setEnabled(True)
             self.modify_segment.setEnabled(True)
             self.modify_classify.setEnabled(False)
+            show_info("Edge (click to classify)")
 
     return _event
 
-def autocontrast_values(image, clip_hist_percent=0.001):
 
+def autocontrast_values(image, clip_hist_percent=0.001):
     # calculate histogram
-    hist, bin_edges = np.histogram(image, bins=(2 ** 16) - 1)
+    hist, bin_edges = np.histogram(image, bins=(2**16) - 1)
     hist_size = len(hist)
 
     # calculate cumulative distribution from the histogram
     accumulator = cumsum(hist)
 
     # Locate points to clip
     maximum = accumulator[-1]
-    clip_hist_percent *= (maximum / 100.0)
+    clip_hist_percent *= maximum / 100.0
     clip_hist_percent /= 2.0
 
     # Locate left cut
     minimum_gray = 0
     try:
         while accumulator[minimum_gray] < clip_hist_percent:
             minimum_gray += 1
@@ -882,15 +790,15 @@
         gamma = 2
     if gamma < 0.2:
         gamma = 0.2
 
     if maximum_gray > minimum_gray:
         contrast_limit = [minimum_gray, maximum_gray]
     else:
-        contrast_limit = [np.min(image),np.max(image)]
+        contrast_limit = [np.min(image), np.max(image)]
 
     return contrast_limit, alpha, beta, gamma
 
 
 def get_histogram(image, bins):
     """calculates and returns histogram"""
 
@@ -915,89 +823,98 @@
     b = [next(a)]
     for i in a:
         b.append(b[-1] + i)
     return np.array(b)
 
 
 def _viewerControls(self, key, viewer=None):
-
     def _event(viewer):
-
         if key == "h":
             self.viewer.reset_view()
 
         if key == "o":
-
             current_zoom = self.viewer.camera.zoom
             new_zoom = current_zoom - 2
             if new_zoom <= 0:
                 self.viewer.reset_view()
             else:
                 self.viewer.camera.zoom = new_zoom
 
         if key == "i":
             self.viewer.camera.zoom = self.viewer.camera.zoom + 2
 
         if key == "z":
-
             if self.segLayer.visible == True:
                 self.segLayer.visible = False
                 self.modify_viewmasks.setChecked(False)
             else:
                 self.segLayer.visible = True
                 self.modify_viewmasks.setChecked(True)
 
         if key == "x":
-
             if self.classLayer.visible == True:
                 self.classLayer.visible = False
                 self.modify_viewlabels.setChecked(False)
             else:
                 self.classLayer.visible = True
                 self.modify_viewlabels.setChecked(True)
 
         if key == "viewlabels":
             self.classLayer.visible = self.modify_viewlabels.isChecked()
 
         if key == "viewmasks":
             self.segLayer.visible = self.modify_viewmasks.isChecked()
 
         if key == "c":
-
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes","center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Classes", "center_lines"]
+            ]
 
             if len(layer_names) != 0:
-
                 active_layer = layer_names[-1]
 
-                image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
-
-                image = self.viewer.layers[str(active_layer)].data[image_dims].copy()
-
-                crop = self.viewer.layers[str(active_layer)].corner_pixels[:,-2:]
+                image_dims = tuple(
+                    list(self.viewer.dims.current_step[:-2]) + [...]
+                )
+
+                image = (
+                    self.viewer.layers[str(active_layer)]
+                    .data[image_dims]
+                    .copy()
+                )
+
+                crop = self.viewer.layers[str(active_layer)].corner_pixels[
+                    :, -2:
+                ]
 
                 [[y1, x1], [y2, x2]] = crop
 
                 image_crop = image[y1:y2, x1:x2]
 
-                contrast_limit = [np.min(image_crop),np.max(image_crop)]
+                contrast_limit = [np.min(image_crop), np.max(image_crop)]
 
                 if contrast_limit[1] > contrast_limit[0]:
-                    self.viewer.layers[str(active_layer)].contrast_limits = contrast_limit
+                    self.viewer.layers[
+                        str(active_layer)
+                    ].contrast_limits = contrast_limit
+
     return _event
 
-def _imageControls(self, key, viewer=None):
 
+def _imageControls(self, key, viewer=None):
     def _event(viewer):
+        print(True)
 
         if key == "Upload":
             self._uploadDatabase("active")
 
         if len(self.viewer.dims.current_step) == 3:
-
             current_frame = self.viewer.dims.current_step[0]
             frame_range = int(self.viewer.dims.range[0][1]) - 1
 
             if key == "Right" or "Upload":
                 next_step = current_frame + 1
             if key == "Left":
                 next_step = current_frame - 1
@@ -1007,15 +924,14 @@
             if next_step > frame_range:
                 next_step = frame_range
 
             self.viewer.dims.current_step = (next_step, 0, 0)
             self.viewer.reset_view()
 
         if len(self.viewer.dims.current_step) == 4:
-
             current_frame = self.viewer.dims.current_step[0]
             current_tile = self.viewer.dims.current_step[1]
 
             frame_range = int(self.viewer.dims.range[0][1]) - 1
             tile_range = int(self.viewer.dims.range[1][1]) - 1
 
             next_frame = current_frame
@@ -1039,118 +955,107 @@
 
             self.viewer.dims.current_step = (next_frame, next_tile, 0, 0)
             self.viewer.reset_view()
             self._autoContrast()
 
     return _event
 
-def _clear_images(self):
 
+def _clear_images(self):
     self.segLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
 
     layer_names = [layer.name for layer in self.viewer.layers]
 
     for layer_name in layer_names:
-        if layer_name not in ["Segmentations", "Classes","center_lines"]:
+        if layer_name not in ["Segmentations", "Classes", "center_lines"]:
             self.viewer.layers.remove(self.viewer.layers[layer_name])
 
 
 def _copymasktoall(self):
-
     current_fov = self.viewer.dims.current_step[0]
 
     mask = self.segLayer.data[current_fov]
     label = self.classLayer.data[current_fov]
 
     dim_range = int(self.viewer.dims.range[0][1])
 
     for i in range(dim_range):
-
         self.segLayer.data[i] = mask
         self.classLayer.data[i] = label
 
-def _deleteallmasks(self, viewer=None, mode = "all"):
 
+def _deleteallmasks(self, viewer=None, mode="all"):
     def _event(viewer):
-
         try:
             current_step = self.viewer.dims.current_step
 
             viewer_dims = np.array(self.viewer.dims.range[:-2]).astype(int)
 
             if mode == "active":
-
                 mask = self.segLayer.data[current_step[:-2]].copy()
                 mask_ids = np.unique(mask).tolist()
 
                 if len(viewer_dims) == 2:
-
                     self.update_image_folds(mask_ids=mask_ids)
 
                 else:
-
                     for mask_id in mask_ids:
                         mask[mask == mask_id] = 0
 
                     self.segLayer.data[current_step[:-2]] = mask
                     self.segLayer.refresh()
 
             else:
-
                 for image_index in range(*viewer_dims[0]):
-
                     mask = self.segLayer.data[image_index].copy()
                     mask_ids = np.unique(mask)
 
                     if len(viewer_dims) == 2:
-                        self.update_image_folds(mask_ids=mask_ids, image_index=image_index)
+                        self.update_image_folds(
+                            mask_ids=mask_ids, image_index=image_index
+                        )
 
                     else:
-
                         for mask_id in mask_ids:
-                            mask[mask==mask_id] = 0
+                            mask[mask == mask_id] = 0
 
                         self.segLayer.data[image_index] = mask
                         self.segLayer.refresh()
 
             if self.segLayer.visible == True:
                 self.segLayer.visible = False
                 self.segLayer.visible = True
 
-            if self.classLayer.visible==True:
+            if self.classLayer.visible == True:
                 self.classLayer.visible = False
                 self.classLayer.visible = True
 
         except:
             print(traceback.format_exc())
-            pass
 
     return _event
 
-def _delete_active_image(self, viewer=None, mode="active"):
 
+def _delete_active_image(self, viewer=None, mode="active"):
     def _event(viewer):
-
         try:
             current_fov = self.viewer.dims.current_step[0]
 
             dim_range = int(self.viewer.dims.range[0][1])
 
             if mode == "active":
                 dim_delete_list = [current_fov]
             else:
                 dim_delete_list = np.arange(dim_range).tolist()
                 dim_delete_list.remove(current_fov)
 
             layer_names = [layer.name for layer in self.viewer.layers]
 
             if dim_range > 1:
-
                 for layer_name in layer_names:
-
                     layer = self.viewer.layers[layer_name]
 
                     images = layer.data.copy()
                     metadata = layer.metadata.copy()
 
                     if mode == "active":
                         images = np.delete(images, current_fov, axis=0)
@@ -1177,38 +1082,34 @@
         except:
             pass
 
     return _event
 
 
 def _doubeClickEvents(self, viewer, event):
-
     mouse_button = event.button
 
     data_coordinates = self.segLayer.world_to_data(event.position)
     coord = np.round(data_coordinates).astype(int)
     colour = self.segLayer.get_value(coord)
 
-    if mouse_button == 1 and colour in [0,None]:
-
+    if mouse_button == 1 and colour in [0, None]:
         if self.modify_viewmasks.isChecked() == True:
             self.modify_viewmasks.setChecked(False)
             self.segLayer.visible = False
         else:
             self.modify_viewmasks.setChecked(True)
             self.segLayer.visible = True
 
     if mouse_button == 1 and colour != 0:
-
         meta = self.segLayer.metadata.copy()
 
         self.segLayer.fill(coord, 0)
         self.classLayer.fill(coord, 0)
         self.segLayer.selected_label = 0
 
         # update metadata
 
         meta["manual_segmentation"] = True
         self.segLayer.metadata = meta
         self.segLayer.mode = "pan_zoom"
         self.update_image_folds()
-
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_json.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
         json.dump(annotation, f)
 
     return annotation
 
 
 def import_coco_json(json_path):
 
+    json_path = os.path.splitext(json_path)[0] + ".txt"
+
     with open(json_path, 'r') as f:
         dat = json.load(f)
 
     h = dat["images"][0]["height"]
     w = dat["images"][0]["width"]
 
     mask = np.zeros((h, w), dtype=np.uint16)
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_oufti.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_oufti.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_refine.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_refine.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_statistics.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     contours, hierarchy = cv2.findContours(img, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)
     contours = sorted(contours, key=cv2.contourArea, reverse=True)
     return contours
 
 
 def determine_overlap(cnt_num, contours, image):
+
     try:
 
         # gets current contour of interest
         cnt = contours[cnt_num]
 
         # number of pixels in contour
         cnt_pixels = len(cnt)
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_utils_tiler.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_utils_tiler.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/_widget.py` & `napari-bacseg-1.0.5/src/napari_bacseg/_widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,15 +17,30 @@
 
 import cv2
 import napari
 import numpy as np
 from napari.utils.notifications import show_info
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
 from qtpy.QtCore import QObject, QRunnable, QThreadPool
-from qtpy.QtWidgets import (QCheckBox, QComboBox, QFileDialog, QFormLayout, QHBoxLayout, QLabel, QLineEdit, QProgressBar, QPushButton, QRadioButton, QSlider, QTabWidget, QVBoxLayout, QWidget, )
+from qtpy.QtWidgets import (
+    QCheckBox,
+    QComboBox,
+    QFileDialog,
+    QFormLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QProgressBar,
+    QPushButton,
+    QRadioButton,
+    QSlider,
+    QTabWidget,
+    QVBoxLayout,
+    QWidget,
+)
 
 import napari_bacseg._utils
 from napari_bacseg._utils import align_image_channels, unstack_images
 
 os.environ["QT_AUTO_SCREEN_SCALE_FACTOR"] = "1"
 
 
@@ -91,15 +106,17 @@
         try:
             result = self.fn(*self.args, **self.kwargs)
         except:
             traceback.print_exc()
             exctype, value = sys.exc_info()[:2]
             self.signals.error.emit((exctype, value, traceback.format_exc()))
         else:
-            self.signals.result.emit(result)  # Return the result of the processing
+            self.signals.result.emit(
+                result
+            )  # Return the result of the processing
         finally:
             self.signals.finished.emit()  # Done
 
     def result(self):
         return self.fn(*self.args, **self.kwargs)
 
 
@@ -140,20 +157,52 @@
     def __init__(self, viewer: napari.Viewer):
         """Initialize widget with two layer combo boxes and a run button"""
 
         super().__init__()
 
         # import functions
         from napari_bacseg._utils import _manualImport, stack_images
-        from napari_bacseg._utils_cellpose import (_initialise_cellpose_model, _select_cellpose_save_directory, _select_cellpose_save_path, _select_custom_cellpose_model, train_cellpose_model, )
-        from napari_bacseg._utils_database import (_create_bacseg_database, _load_bacseg_database, _populateUSERMETA, _show_database_controls, populate_upload_combos, update_database_metadata, )
-        from napari_bacseg._utils_interface_events import (_copymasktoall, _delete_active_image, _deleteallmasks, _doubeClickEvents, _imageControls, _modifyMode, _segmentationEvents, _viewerControls, )
-        from napari_bacseg._utils_oufti import (_update_active_midlines, centre_oufti_midlines, generate_midlines, midline_edit_toggle, update_midlines, )
+        from napari_bacseg._utils_cellpose import (
+            _initialise_cellpose_model,
+            _select_cellpose_save_directory,
+            _select_cellpose_save_path,
+            _select_custom_cellpose_model,
+            train_cellpose_model,
+        )
+        from napari_bacseg._utils_database import (
+            _create_bacseg_database,
+            _load_bacseg_database,
+            _populateUSERMETA,
+            _show_database_controls,
+            populate_upload_combos,
+            update_database_metadata,
+        )
+        from napari_bacseg._utils_interface_events import (
+            _copymasktoall,
+            _delete_active_image,
+            _deleteallmasks,
+            _doubeClickEvents,
+            _imageControls,
+            _modifyMode,
+            _segmentationEvents,
+            _viewerControls,
+        )
+        from napari_bacseg._utils_oufti import (
+            _update_active_midlines,
+            centre_oufti_midlines,
+            generate_midlines,
+            midline_edit_toggle,
+            update_midlines,
+        )
         from napari_bacseg._utils_statistics import _compute_simple_cell_stats
-        from napari_bacseg._utils_tiler import (fold_images, unfold_images, update_image_folds, )
+        from napari_bacseg._utils_tiler import (
+            fold_images,
+            unfold_images,
+            update_image_folds,
+        )
         from napari_bacseg.bacseg_ui import Ui_tab_widget
 
         self.populate_upload_combos = self.wrapper(populate_upload_combos)
         self.update_database_metadata = self.wrapper(update_database_metadata)
         self.stack_image = self.wrapper(stack_images)
         self._modifyMode = self.wrapper(_modifyMode)
         self._viewerControls = self.wrapper(_viewerControls)
@@ -161,31 +210,41 @@
         self._deleteallmasks = self.wrapper(_deleteallmasks)
         self._delete_active_image = self.wrapper(_delete_active_image)
         self._populateUSERMETA = self.wrapper(_populateUSERMETA)
         self._imageControls = self.wrapper(_imageControls)
         self._segmentationEvents = self.wrapper(_segmentationEvents)
         self._manualImport = self.wrapper(_manualImport)
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
-        self._initialise_cellpose_model = self.wrapper(_initialise_cellpose_model)
-        self._select_custom_cellpose_model = self.wrapper(_select_custom_cellpose_model)
-        self._select_cellpose_save_directory = self.wrapper(_select_cellpose_save_directory)
-        self._select_cellpose_save_path = self.wrapper(_select_cellpose_save_path)
+        self._initialise_cellpose_model = self.wrapper(
+            _initialise_cellpose_model
+        )
+        self._select_custom_cellpose_model = self.wrapper(
+            _select_custom_cellpose_model
+        )
+        self._select_cellpose_save_directory = self.wrapper(
+            _select_cellpose_save_directory
+        )
+        self._select_cellpose_save_path = self.wrapper(
+            _select_cellpose_save_path
+        )
         self.unfold_images = self.wrapper(unfold_images)
         self.fold_images = self.wrapper(fold_images)
         self.update_image_folds = self.wrapper(update_image_folds)
         self.midline_edit_toggle = self.wrapper(midline_edit_toggle)
         self.centre_oufti_midlines = self.wrapper(centre_oufti_midlines)
         self.generate_midlines = self.wrapper(generate_midlines)
         self.update_midlines = self.wrapper(update_midlines)
         self._update_active_midlines = self.wrapper(_update_active_midlines)
         self._create_bacseg_database = self.wrapper(_create_bacseg_database)
         self._load_bacseg_database = self.wrapper(_load_bacseg_database)
         self._show_database_controls = self.wrapper(_show_database_controls)
         self._doubeClickEvents = self.wrapper(_doubeClickEvents)
-        self._compute_simple_cell_stats = self.wrapper(_compute_simple_cell_stats)
+        self._compute_simple_cell_stats = self.wrapper(
+            _compute_simple_cell_stats
+        )
 
         application_path = os.path.dirname(sys.executable)
         self.viewer = viewer
         self.setLayout(QVBoxLayout())
 
         # ui_path = os.path.abspath(r"C:\napari-bacseg\src\napari_bacseg\bacseg_ui.ui")
         # self.bacseg_ui = uic.loadUi(ui_path)
@@ -206,101 +265,206 @@
         self.active_import_mode = ""
         self.import_mode = self.findChild(QComboBox, "import_mode")
         self.import_filemode = self.findChild(QComboBox, "import_filemode")
         self.import_precision = self.findChild(QComboBox, "import_precision")
         self.import_import = self.findChild(QPushButton, "import_import")
         self.import_limit = self.findChild(QComboBox, "import_limit")
         self.import_limit_label = self.findChild(QLabel, "import_limit_label")
-        self.clear_previous = self.findChild(QCheckBox, "import_clear_previous")
+        self.clear_previous = self.findChild(
+            QCheckBox, "import_clear_previous"
+        )
         self.autocontrast = self.findChild(QCheckBox, "import_auto_contrast")
-        self.import_multiframe_mode = self.findChild(QComboBox, "import_multiframe_mode")
+        self.import_multiframe_mode = self.findChild(
+            QComboBox, "import_multiframe_mode"
+        )
         self.import_crop_mode = self.findChild(QComboBox, "import_crop_mode")
         self.channel_mode = self.findChild(QComboBox, "nim_channel_mode")
-        self.import_progressbar = self.findChild(QProgressBar, "import_progressbar")
+        self.import_progressbar = self.findChild(
+            QProgressBar, "import_progressbar"
+        )
         self.import_align = self.findChild(QCheckBox, "import_align")
         self.label_modality = self.findChild(QComboBox, "label_modality")
         self.label_stain = self.findChild(QComboBox, "label_stain")
-        self.label_stain_target = self.findChild(QComboBox, "label_stain_target")
+        self.label_stain_target = self.findChild(
+            QComboBox, "label_stain_target"
+        )
         self.label_overwrite = self.findChild(QPushButton, "label_overwrite")
-        self.label_light_source = self.findChild(QComboBox, "label_light_source")
+        self.label_light_source = self.findChild(
+            QComboBox, "label_light_source"
+        )
 
         # view tab controls + variables from Qt Desinger References
         self.unfold_tile_size = self.findChild(QComboBox, "unfold_tile_size")
-        self.unfold_tile_overlap = self.findChild(QComboBox, "unfold_tile_overlap")
+        self.unfold_tile_overlap = self.findChild(
+            QComboBox, "unfold_tile_overlap"
+        )
         self.unfold_mode = self.findChild(QComboBox, "unfold_mode")
         self.fold = self.findChild(QPushButton, "fold")
         self.unfold = self.findChild(QPushButton, "unfold")
-        self.unfold_progressbar = self.findChild(QPushButton, "unfold_progressbar")
+        self.unfold_progressbar = self.findChild(
+            QPushButton, "unfold_progressbar"
+        )
+        self.alignment_channel = self.findChild(QComboBox, "alignment_channel")
+        self.align_active_image = self.findChild(
+            QPushButton, "align_active_image"
+        )
+        self.align_all_images = self.findChild(QPushButton, "align_all_images")
+
+        self.overlay_filename = self.findChild(QCheckBox, "overlay_filename")
+        self.overlay_folder = self.findChild(QCheckBox, "overlay_folder")
+        self.overlay_microscope = self.findChild(
+            QCheckBox, "overlay_microscope"
+        )
+        self.overlay_datemodified = self.findChild(
+            QCheckBox, "overlay_datemodified"
+        )
+        self.overlay_content = self.findChild(QCheckBox, "overlay_content")
+        self.overlay_phenotype = self.findChild(QCheckBox, "overlay_phenotype")
+        self.overlay_strain = self.findChild(QCheckBox, "overlay_strain")
+        self.overlay_staintarget = self.findChild(
+            QCheckBox, "overlay_staintarget"
+        )
+        self.overlay_antibiotic = self.findChild(
+            QCheckBox, "overlay_antibiotic"
+        )
+        self.overlay_stain = self.findChild(QCheckBox, "overlay_stain")
+        self.overlay_modality = self.findChild(QCheckBox, "overlay_modality")
+        self.overlay_lightsource = self.findChild(
+            QCheckBox, "overlay_lightsource"
+        )
+        self.overlay_focus = self.findChild(QCheckBox, "overlay_focus")
+        self.overlay_debris = self.findChild(QCheckBox, "overlay_debris")
+        self.overlay_laplacian = self.findChild(QCheckBox, "overlay_laplacian")
+        self.overlay_range = self.findChild(QCheckBox, "overlay_range")
 
         # cellpose controls + variables from Qt Desinger References
         self.cellpose_segmentation = False
         self.cellpose_model = None
         self.cellpose_custom_model_path = ""
         self.cellpose_train_model_path = ""
         self.cellpose_log_file = None
-        self.cellpose_select_custom_model = self.findChild(QPushButton, "cellpose_select_custom_model")
+        self.cellpose_select_custom_model = self.findChild(
+            QPushButton, "cellpose_select_custom_model"
+        )
         self.cellpose_segmodel = self.findChild(QComboBox, "cellpose_segmodel")
-        self.cellpose_trainmodel = self.findChild(QComboBox, "cellpose_trainmodel")
-        self.cellpose_segchannel = self.findChild(QComboBox, "cellpose_segchannel")
-        self.cellpose_flowthresh = self.findChild(QSlider, "cellpose_flowthresh")
-        self.cellpose_flowthresh_label = self.findChild(QLabel, "cellpose_flowthresh_label")
-        self.cellpose_maskthresh = self.findChild(QSlider, "cellpose_maskthresh")
-        self.cellpose_maskthresh_label = self.findChild(QLabel, "cellpose_maskthresh_label")
+        self.cellpose_trainmodel = self.findChild(
+            QComboBox, "cellpose_trainmodel"
+        )
+        self.cellpose_segchannel = self.findChild(
+            QComboBox, "cellpose_segchannel"
+        )
+        self.cellpose_flowthresh = self.findChild(
+            QSlider, "cellpose_flowthresh"
+        )
+        self.cellpose_flowthresh_label = self.findChild(
+            QLabel, "cellpose_flowthresh_label"
+        )
+        self.cellpose_maskthresh = self.findChild(
+            QSlider, "cellpose_maskthresh"
+        )
+        self.cellpose_maskthresh_label = self.findChild(
+            QLabel, "cellpose_maskthresh_label"
+        )
         self.cellpose_minsize = self.findChild(QSlider, "cellpose_minsize")
-        self.cellpose_minsize_label = self.findChild(QLabel, "cellpose_minsize_label")
+        self.cellpose_minsize_label = self.findChild(
+            QLabel, "cellpose_minsize_label"
+        )
         self.cellpose_diameter = self.findChild(QSlider, "cellpose_diameter")
-        self.cellpose_diameter_label = self.findChild(QLabel, "cellpose_diameter_label")
-        self.cellpose_segment_active = self.findChild(QPushButton, "cellpose_segment_active")
-        self.cellpose_segment_all = self.findChild(QPushButton, "cellpose_segment_all")
-        self.cellpose_clear_previous = self.findChild(QCheckBox, "cellpose_clear_previous")
+        self.cellpose_diameter_label = self.findChild(
+            QLabel, "cellpose_diameter_label"
+        )
+        self.cellpose_segment_active = self.findChild(
+            QPushButton, "cellpose_segment_active"
+        )
+        self.cellpose_segment_all = self.findChild(
+            QPushButton, "cellpose_segment_all"
+        )
+        self.cellpose_clear_previous = self.findChild(
+            QCheckBox, "cellpose_clear_previous"
+        )
         self.cellpose_usegpu = self.findChild(QCheckBox, "cellpose_usegpu")
-        self.cellpose_resetimage = self.findChild(QCheckBox, "cellpose_resetimage")
-        self.cellpose_progressbar = self.findChild(QProgressBar, "cellpose_progressbar")
-        self.cellpose_train_model = self.findChild(QPushButton, "cellpose_train_model")
-        self.cellpose_save_dir = self.findChild(QPushButton, "cellpose_save_dir")
-        self.cellpose_trainchannel = self.findChild(QComboBox, "cellpose_trainchannel")
+        self.cellpose_resetimage = self.findChild(
+            QCheckBox, "cellpose_resetimage"
+        )
+        self.cellpose_progressbar = self.findChild(
+            QProgressBar, "cellpose_progressbar"
+        )
+        self.cellpose_train_model = self.findChild(
+            QPushButton, "cellpose_train_model"
+        )
+        self.cellpose_save_dir = self.findChild(
+            QPushButton, "cellpose_save_dir"
+        )
+        self.cellpose_trainchannel = self.findChild(
+            QComboBox, "cellpose_trainchannel"
+        )
         self.cellpose_nepochs = self.findChild(QComboBox, "cellpose_nepochs")
-        self.cellpose_batchsize = self.findChild(QComboBox, "cellpose_batchsize")
+        self.cellpose_batchsize = self.findChild(
+            QComboBox, "cellpose_batchsize"
+        )
 
         # modify tab controls + variables from Qt Desinger References
         self.interface_mode = "panzoom"
         self.segmentation_mode = "add"
         self.class_mode = "single"
         self.class_colour = 1
         self.modify_panzoom = self.findChild(QPushButton, "modify_panzoom")
         self.modify_segment = self.findChild(QPushButton, "modify_segment")
         self.modify_classify = self.findChild(QPushButton, "modify_classify")
         self.modify_refine = self.findChild(QPushButton, "modify_refine")
         self.refine_channel = self.findChild(QComboBox, "refine_channel")
         self.refine_all = self.findChild(QPushButton, "refine_all")
-        self.modify_copymasktoall = self.findChild(QPushButton, "modify_copymasktoall")
-        self.modify_deleteallmasks = self.findChild(QPushButton, "modify_deleteallmasks")
-        self.modify_deleteactivemasks = self.findChild(QPushButton, "modify_deleteactivemasks")
-        self.modify_deleteactiveimage = self.findChild(QPushButton, "modify_deleteactiveimage")
-        self.modify_deleteotherimages = self.findChild(QPushButton, "modify_deleteotherimages")
-        self.modify_progressbar = self.findChild(QProgressBar, "modify_progressbar")
-
-        self.modify_auto_panzoom = self.findChild(QCheckBox, "modify_auto_panzoom")
+        self.modify_copymasktoall = self.findChild(
+            QPushButton, "modify_copymasktoall"
+        )
+        self.modify_deleteallmasks = self.findChild(
+            QPushButton, "modify_deleteallmasks"
+        )
+        self.modify_deleteactivemasks = self.findChild(
+            QPushButton, "modify_deleteactivemasks"
+        )
+        self.modify_deleteactiveimage = self.findChild(
+            QPushButton, "modify_deleteactiveimage"
+        )
+        self.modify_deleteotherimages = self.findChild(
+            QPushButton, "modify_deleteotherimages"
+        )
+        self.modify_progressbar = self.findChild(
+            QProgressBar, "modify_progressbar"
+        )
+
+        self.modify_auto_panzoom = self.findChild(
+            QCheckBox, "modify_auto_panzoom"
+        )
         self.modify_add = self.findChild(QPushButton, "modify_add")
         self.modify_extend = self.findChild(QPushButton, "modify_extend")
         self.modify_split = self.findChild(QPushButton, "modify_split")
         self.modify_join = self.findChild(QPushButton, "modify_join")
         self.modify_delete = self.findChild(QPushButton, "modify_delete")
         self.classify_single = self.findChild(QPushButton, "classify_single")
-        self.classify_dividing = self.findChild(QPushButton, "classify_dividing")
+        self.classify_dividing = self.findChild(
+            QPushButton, "classify_dividing"
+        )
         self.classify_divided = self.findChild(QPushButton, "classify_divided")
-        self.classify_vertical = self.findChild(QPushButton, "classify_vertical")
+        self.classify_vertical = self.findChild(
+            QPushButton, "classify_vertical"
+        )
         self.classify_broken = self.findChild(QPushButton, "classify_broken")
         self.classify_edge = self.findChild(QPushButton, "classify_edge")
         self.modify_viewmasks = self.findChild(QCheckBox, "modify_viewmasks")
         self.modify_viewlabels = self.findChild(QCheckBox, "modify_viewlabels")
         self.find_next = self.findChild(QPushButton, "find_next")
         self.find_previous = self.findChild(QPushButton, "find_previous")
         self.find_criterion = self.findChild(QComboBox, "find_criterion")
         self.find_mode = self.findChild(QComboBox, "find_mode")
+        self.scalebar_show = self.findChild(QCheckBox, "scalebar_show")
+        self.scalebar_resolution = self.findChild(
+            QLineEdit, "scalebar_resolution"
+        )
+        self.scalebar_units = self.findChild(QComboBox, "scalebar_units")
 
         self.set_quality_mode = self.findChild(QComboBox, "set_quality_mode")
         self.set_focus_0 = self.findChild(QPushButton, "set_focus_0")
         self.set_focus_1 = self.findChild(QPushButton, "set_focus_1")
         self.set_focus_2 = self.findChild(QPushButton, "set_focus_2")
         self.set_focus_3 = self.findChild(QPushButton, "set_focus_3")
         self.set_focus_4 = self.findChild(QPushButton, "set_focus_4")
@@ -308,287 +472,730 @@
 
         self.set_debris_1 = self.findChild(QPushButton, "set_debris_1")
         self.set_debris_2 = self.findChild(QPushButton, "set_debris_2")
         self.set_debris_3 = self.findChild(QPushButton, "set_debris_3")
         self.set_debris_4 = self.findChild(QPushButton, "set_debris_4")
         self.set_debris_5 = self.findChild(QPushButton, "set_debris_5")
 
-        self.modify_panzoom.setEnabled(False)
-        self.modify_add.setEnabled(False)
-        self.modify_extend.setEnabled(False)
-        self.modify_join.setEnabled(False)
-        self.modify_split.setEnabled(False)
-        self.modify_delete.setEnabled(False)
-        self.modify_refine.setEnabled(False)
-        self.classify_single.setEnabled(False)
-        self.classify_dividing.setEnabled(False)
-        self.classify_divided.setEnabled(False)
-        self.classify_vertical.setEnabled(False)
-        self.classify_broken.setEnabled(False)
-        self.classify_edge.setEnabled(False)
-
         # upload tab controls from Qt Desinger References
         self.database_path = ""
         self.user_metadata_keys = 6
 
-        self.metadata_columns = ["date_uploaded", "date_created", "date_modified", "file_name", "channel", "file_list", "channel_list", "segmentation_file", "segmentation_channel", "akseg_hash",
-            "user_initial", "content", "microscope", "modality", "source", "stain", "stain_target", "antibiotic", "treatment time (mins)", "antibiotic concentration", "mounting method", "protocol",
-            "folder", "parent_folder", "num_segmentations", "image_laplacian", "image_focus","image_debris","segmented", "labelled", "segmentation_curated", "label_curated", "posX", "posY", "posZ",
-            "image_load_path", "image_save_path", "mask_load_path", "mask_save_path", "label_load_path", "label_save_path"]
+        self.metadata_columns = [
+            "date_uploaded",
+            "date_created",
+            "date_modified",
+            "file_name",
+            "channel",
+            "file_list",
+            "channel_list",
+            "segmentation_file",
+            "segmentation_channel",
+            "akseg_hash",
+            "user_initial",
+            "content",
+            "microscope",
+            "modality",
+            "source",
+            "strain",
+            "phenotype",
+            "stain",
+            "stain_target",
+            "antibiotic",
+            "treatment time (mins)",
+            "antibiotic concentration",
+            "mounting method",
+            "protocol",
+            "folder",
+            "parent_folder",
+            "num_segmentations",
+            "image_laplacian",
+            "image_focus",
+            "image_debris",
+            "segmented",
+            "labelled",
+            "segmentation_curated",
+            "label_curated",
+            "posX",
+            "posY",
+            "posZ",
+            "image_load_path",
+            "image_save_path",
+            "mask_load_path",
+            "mask_save_path",
+            "label_load_path",
+            "label_save_path",
+        ]
 
-        user_key_list = np.arange(1,self.user_metadata_keys+1).tolist()
+        user_key_list = np.arange(1, self.user_metadata_keys + 1).tolist()
         user_key_list.reverse()
 
         for key in user_key_list:
             user_key = f"user_meta{key}"
-            self.metadata_columns.insert(22,str(user_key))
-            setattr(self, f"upload_usermeta{key}", self.findChild(QComboBox, f"upload_usermeta{key}"))
+            self.metadata_columns.insert(22, str(user_key))
+            setattr(
+                self,
+                f"upload_usermeta{key}",
+                self.findChild(QComboBox, f"upload_usermeta{key}"),
+            )
 
         self.upload_initial = self.findChild(QComboBox, "upload_initial")
         self.upload_content = self.findChild(QComboBox, "upload_content")
         self.upload_microscope = self.findChild(QComboBox, "upload_microscope")
         self.upload_antibiotic = self.findChild(QComboBox, "upload_antibiotic")
-        self.upload_abxconcentration = self.findChild(QComboBox, "upload_abxconcentration")
-        self.upload_treatmenttime = self.findChild(QComboBox, "upload_treatmenttime")
+        self.upload_phenotype = self.findChild(QComboBox, "upload_phenotype")
+        self.upload_strain = self.findChild(QComboBox, "upload_strain")
+        self.upload_abxconcentration = self.findChild(
+            QComboBox, "upload_abxconcentration"
+        )
+        self.upload_treatmenttime = self.findChild(
+            QComboBox, "upload_treatmenttime"
+        )
         self.upload_mount = self.findChild(QComboBox, "upload_mount")
         self.upload_protocol = self.findChild(QComboBox, "upload_protocol")
-        self.upload_overwrite_images = self.findChild(QCheckBox, "upload_overwrite_images")
-        self.upload_overwrite_masks = self.findChild(QCheckBox, "upload_overwrite_masks")
-        self.overwrite_selected_metadata = self.findChild(QCheckBox, "overwrite_selected_metadata")
-        self.overwrite_all_metadata = self.findChild(QCheckBox, "overwrite_all_metadata")
+        self.upload_overwrite_images = self.findChild(
+            QCheckBox, "upload_overwrite_images"
+        )
+        self.upload_overwrite_masks = self.findChild(
+            QCheckBox, "upload_overwrite_masks"
+        )
+        self.overwrite_selected_metadata = self.findChild(
+            QCheckBox, "overwrite_selected_metadata"
+        )
+        self.overwrite_all_metadata = self.findChild(
+            QCheckBox, "overwrite_all_metadata"
+        )
         self.upload_all = self.findChild(QPushButton, "upload_all")
         self.upload_active = self.findChild(QPushButton, "upload_active")
-        self.database_download = self.findChild(QPushButton, "database_download")
-        self.database_download_limit = self.findChild(QComboBox, "database_download_limit")
+        self.database_download = self.findChild(
+            QPushButton, "database_download"
+        )
+        self.database_download_limit = self.findChild(
+            QComboBox, "database_download_limit"
+        )
         self.create_database = self.findChild(QPushButton, "create_database")
         self.load_database = self.findChild(QPushButton, "load_database")
-        self.display_database_path = self.findChild(QLineEdit, "display_database_path")
-        self.upload_progressbar = self.findChild(QProgressBar, "upload_progressbar")
+        self.display_database_path = self.findChild(
+            QLineEdit, "display_database_path"
+        )
+        self.upload_progressbar = self.findChild(
+            QProgressBar, "upload_progressbar"
+        )
         self.upload_tab = self.findChild(QWidget, "upload_tab")
-        self.upload_segmentation_combo = self.findChild(QComboBox, "upload_segmentation_combo")
-        self.upload_label_combo = self.findChild(QComboBox, "upload_label_combo")
-        self.download_sort_order = self.findChild(QComboBox, "download_sort_order")
+        self.upload_segmentation_combo = self.findChild(
+            QComboBox, "upload_segmentation_combo"
+        )
+        self.upload_label_combo = self.findChild(
+            QComboBox, "upload_label_combo"
+        )
+        self.download_sort_order_1 = self.findChild(
+            QComboBox, "download_sort_order_1"
+        )
+        self.download_sort_order_2 = self.findChild(
+            QComboBox, "download_sort_order_2"
+        )
+        self.download_sort_direction_1 = self.findChild(
+            QComboBox, "download_sort_direction_1"
+        )
+        self.download_sort_direction_2 = self.findChild(
+            QComboBox, "download_sort_direction_2"
+        )
         self.update_metadata = self.findChild(QPushButton, "update_metadata")
-
-        self.image_metadata_controls = self.findChild(QFormLayout, "image_metadata_controls")
+        self.upload_images_setting = self.findChild(
+            QCheckBox, "upload_images_setting"
+        )
+        self.upload_segmentations_setting = self.findChild(
+            QCheckBox, "upload_segmentations_setting"
+        )
+        self.upload_metadata_setting = self.findChild(
+            QCheckBox, "upload_metadata_setting"
+        )
+
+        self.image_metadata_controls = self.findChild(
+            QFormLayout, "image_metadata_controls"
+        )
 
         self._show_database_controls(False)
 
         # oufti tab controls
-        self.oufti_generate_all_midlines = self.findChild(QPushButton, "oufti_generate_all_midlines")
-        self.oufti_generate_active_midlines = self.findChild(QPushButton, "oufti_generate_active_midlines")
-        self.oufti_panzoom_mode = self.findChild(QRadioButton, "oufti_panzoom_mode")
+        self.oufti_generate_all_midlines = self.findChild(
+            QPushButton, "oufti_generate_all_midlines"
+        )
+        self.oufti_generate_active_midlines = self.findChild(
+            QPushButton, "oufti_generate_active_midlines"
+        )
+        self.oufti_panzoom_mode = self.findChild(
+            QRadioButton, "oufti_panzoom_mode"
+        )
         self.oufti_edit_mode = self.findChild(QRadioButton, "oufti_edit_mode")
-        self.oufti_midline_vertexes = self.findChild(QComboBox, "oufti_midline_vertexes")
-        self.oufti_centre_all_midlines = self.findChild(QPushButton, "oufti_centre_all_midlines")
-        self.oufti_centre_active_midlines = self.findChild(QPushButton, "oufti_centre_active_midlines")
+        self.oufti_midline_vertexes = self.findChild(
+            QComboBox, "oufti_midline_vertexes"
+        )
+        self.oufti_centre_all_midlines = self.findChild(
+            QPushButton, "oufti_centre_all_midlines"
+        )
+        self.oufti_centre_active_midlines = self.findChild(
+            QPushButton, "oufti_centre_active_midlines"
+        )
         self.oufti_mesh_length = self.findChild(QComboBox, "oufti_mesh_length")
-        self.oufti_mesh_dilation = self.findChild(QComboBox, "oufti_mesh_dilation")
+        self.oufti_mesh_dilation = self.findChild(
+            QComboBox, "oufti_mesh_dilation"
+        )
 
         # export tab controls from Qt Desinger References
         self.export_channel = self.findChild(QComboBox, "export_channel")
         self.export_mode = self.findChild(QComboBox, "export_mode")
         self.export_location = self.findChild(QComboBox, "export_location")
         self.export_modifier = self.findChild(QLineEdit, "export_modifier")
         self.export_single = self.findChild(QCheckBox, "export_single")
         self.export_dividing = self.findChild(QCheckBox, "export_dividing")
         self.export_divided = self.findChild(QCheckBox, "export_divided")
         self.export_vertical = self.findChild(QCheckBox, "export_vertical")
         self.export_broken = self.findChild(QCheckBox, "export_broken")
         self.export_edge = self.findChild(QCheckBox, "export_edge")
-        self.export_statistics_multithreaded = self.findChild(QCheckBox, "export_statistics_multithreaded")
+        self.export_statistics_multithreaded = self.findChild(
+            QCheckBox, "export_statistics_multithreaded"
+        )
         self.export_active = self.findChild(QPushButton, "export_active")
         self.export_all = self.findChild(QPushButton, "export_all")
         self.export_normalise = self.findChild(QCheckBox, "export_normalise")
         self.export_invert = self.findChild(QCheckBox, "export_invert")
-        self.export_autocontrast = self.findChild(QCheckBox, "export_autocontrast")
-        self.export_statistics_pixelsize = self.findChild(QLineEdit, "export_statistics_pixelsize")
-        self.export_statistics_active = self.findChild(QPushButton, "export_statistics_active")
-        self.export_statistics_all = self.findChild(QPushButton, "export_statistics_all")
-        self.export_colicoords_mode = self.findChild(QComboBox, "export_colicoords_mode")
-        self.export_progressbar = self.findChild(QProgressBar, "export_progressbar")
-        self.export_image_setting = self.findChild(QCheckBox, "export_image_setting")
-        self.export_overwrite_setting = self.findChild(QCheckBox, "export_overwrite_setting")
+        self.export_scalebar = self.findChild(QCheckBox, "export_scalebar")
+        self.export_scalebar_resolution = self.findChild(
+            QLineEdit, "export_scalebar_resolution"
+        )
+        self.export_scalebar_resolution_units = self.findChild(
+            QComboBox, "export_scalebar_resolution_units"
+        )
+        self.export_scalebar_size = self.findChild(
+            QLineEdit, "export_scalebar_size"
+        )
+        self.export_scalebar_size_units = self.findChild(
+            QComboBox, "export_scalebar_size_units"
+        )
+        self.export_scalebar_colour = self.findChild(
+            QComboBox, "export_scalebar_colour"
+        )
+        self.export_scalebar_thickness = self.findChild(
+            QComboBox, "export_scalebar_thickness"
+        )
+        self.export_cropzoom = self.findChild(QCheckBox, "export_crop_zoom")
+        self.export_mask_background = self.findChild(
+            QCheckBox, "export_mask_background"
+        )
+
+        self.export_autocontrast = self.findChild(
+            QCheckBox, "export_autocontrast"
+        )
+        self.export_statistics_pixelsize = self.findChild(
+            QLineEdit, "export_statistics_pixelsize"
+        )
+        self.export_statistics_active = self.findChild(
+            QPushButton, "export_statistics_active"
+        )
+        self.export_statistics_all = self.findChild(
+            QPushButton, "export_statistics_all"
+        )
+        self.export_colicoords_mode = self.findChild(
+            QComboBox, "export_colicoords_mode"
+        )
+        self.export_progressbar = self.findChild(
+            QProgressBar, "export_progressbar"
+        )
+        self.export_image_setting = self.findChild(
+            QCheckBox, "export_image_setting"
+        )
+        self.export_overwrite_setting = self.findChild(
+            QCheckBox, "export_overwrite_setting"
+        )
         self.export_directory = ""
 
         # import events
         self.autocontrast.stateChanged.connect(self._autoContrast)
         self.import_import.clicked.connect(self._importDialog)
         self.label_overwrite.clicked.connect(self.overwrite_channel_info)
 
         # view events
         self.fold.clicked.connect(self.fold_images)
         self.unfold.clicked.connect(self.unfold_images)
         self.tiler_object = None
         self.tile_dict = {"Segmentations": [], "Classes": []}
         self.unfolded = False
+        self.align_active_image.clicked.connect(
+            partial(self._align_images, mode="active")
+        )
+        self.align_all_images.clicked.connect(
+            partial(self._align_images, mode="all")
+        )
+        self.scalebar_show.stateChanged.connect(self._updateScaleBar)
+        self.scalebar_resolution.textChanged.connect(self._updateScaleBar)
+        self.scalebar_units.currentTextChanged.connect(self._updateScaleBar)
+        self.overlay_filename.stateChanged.connect(self._updateFileName)
+        self.overlay_folder.stateChanged.connect(self._updateFileName)
+        self.overlay_microscope.stateChanged.connect(self._updateFileName)
+        self.overlay_datemodified.stateChanged.connect(self._updateFileName)
+        self.overlay_content.stateChanged.connect(self._updateFileName)
+        self.overlay_phenotype.stateChanged.connect(self._updateFileName)
+        self.overlay_strain.stateChanged.connect(self._updateFileName)
+        self.overlay_antibiotic.stateChanged.connect(self._updateFileName)
+        self.overlay_stain.stateChanged.connect(self._updateFileName)
+        self.overlay_staintarget.stateChanged.connect(self._updateFileName)
+        self.overlay_modality.stateChanged.connect(self._updateFileName)
+        self.overlay_lightsource.stateChanged.connect(self._updateFileName)
+        self.overlay_focus.stateChanged.connect(self._updateFileName)
+        self.overlay_debris.stateChanged.connect(self._updateFileName)
+        self.overlay_laplacian.stateChanged.connect(self._updateFileName)
+        self.overlay_range.stateChanged.connect(self._updateFileName)
 
         # cellpose events
-        self.cellpose_flowthresh.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_flowthresh", "cellpose_flowthresh_label"))
-        self.cellpose_maskthresh.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_maskthresh", "cellpose_maskthresh_label"))
-        self.cellpose_minsize.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_minsize", "cellpose_minsize_label"))
-        self.cellpose_diameter.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_diameter", "cellpose_diameter_label"))
-
-        self.cellpose_select_custom_model.clicked.connect(self._select_custom_cellpose_model)
-        self.cellpose_save_dir.clicked.connect(self._select_cellpose_save_directory)
+        self.cellpose_flowthresh.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_flowthresh", "cellpose_flowthresh_label"
+            )
+        )
+        self.cellpose_maskthresh.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_maskthresh", "cellpose_maskthresh_label"
+            )
+        )
+        self.cellpose_minsize.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_minsize", "cellpose_minsize_label"
+            )
+        )
+        self.cellpose_diameter.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_diameter", "cellpose_diameter_label"
+            )
+        )
+
+        self.cellpose_select_custom_model.clicked.connect(
+            self._select_custom_cellpose_model
+        )
+        self.cellpose_save_dir.clicked.connect(
+            self._select_cellpose_save_directory
+        )
         self.cellpose_segment_all.clicked.connect(self._segmentAll)
         self.cellpose_segment_active.clicked.connect(self._segmentActive)
         self.cellpose_train_model.clicked.connect(self._trainCellpose)
-        self.cellpose_segchannel.currentTextChanged.connect(self._updateSegChannels)
+        self.cellpose_segchannel.currentTextChanged.connect(
+            self._updateSegChannels
+        )
 
         # modify tab events
         self.modify_panzoom.clicked.connect(self._modifyMode(mode="panzoom"))
         self.modify_segment.clicked.connect(self._modifyMode(mode="segment"))
         self.modify_classify.clicked.connect(self._modifyMode(mode="classify"))
         self.modify_refine.clicked.connect(self._modifyMode(mode="refine"))
         self.modify_add.clicked.connect(self._modifyMode(mode="add"))
         self.modify_extend.clicked.connect(self._modifyMode(mode="extend"))
         self.modify_join.clicked.connect(self._modifyMode(mode="join"))
         self.modify_split.clicked.connect(self._modifyMode(mode="split"))
         self.modify_delete.clicked.connect(self._modifyMode(mode="delete"))
         self.classify_single.clicked.connect(self._modifyMode(mode="single"))
-        self.classify_dividing.clicked.connect(self._modifyMode(mode="dividing"))
+        self.classify_dividing.clicked.connect(
+            self._modifyMode(mode="dividing")
+        )
         self.classify_divided.clicked.connect(self._modifyMode(mode="divided"))
-        self.classify_vertical.clicked.connect(self._modifyMode(mode="vertical"))
+        self.classify_vertical.clicked.connect(
+            self._modifyMode(mode="vertical")
+        )
         self.classify_broken.clicked.connect(self._modifyMode(mode="broken"))
         self.classify_edge.clicked.connect(self._modifyMode(mode="edge"))
 
-        self.set_focus_1.clicked.connect(partial(self.set_image_quality, mode = "focus", value=1))
-        self.set_focus_2.clicked.connect(partial(self.set_image_quality, mode = "focus", value=2))
-        self.set_focus_3.clicked.connect(partial(self.set_image_quality, mode = "focus", value=3))
-        self.set_focus_4.clicked.connect(partial(self.set_image_quality, mode = "focus", value=4))
-        self.set_focus_5.clicked.connect(partial(self.set_image_quality, mode = "focus", value=5))
-
-        self.set_debris_1.clicked.connect(partial(self.set_image_quality, mode = "debris", value=1))
-        self.set_debris_2.clicked.connect(partial(self.set_image_quality, mode = "debris", value=2))
-        self.set_debris_3.clicked.connect(partial(self.set_image_quality, mode = "debris", value=3))
-        self.set_debris_4.clicked.connect(partial(self.set_image_quality, mode = "debris", value=4))
-        self.set_debris_5.clicked.connect(partial(self.set_image_quality, mode = "debris", value=5))
-
-        self.modify_viewmasks.stateChanged.connect(self._viewerControls("viewmasks"))
-        self.modify_viewlabels.stateChanged.connect(self._viewerControls("viewlabels"))
+        self.viewer.bind_key(key="b", func=self.set_blurred, overwrite=True)
+        self.set_focus_1.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=1)
+        )
+        self.set_focus_2.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=2)
+        )
+        self.set_focus_3.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=3)
+        )
+        self.set_focus_4.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=4)
+        )
+        self.set_focus_5.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=5)
+        )
+        self.viewer.bind_key(key="f", func=self.set_focused, overwrite=True)
+
+        self.set_debris_1.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=1)
+        )
+        self.set_debris_2.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=2)
+        )
+        self.set_debris_3.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=3)
+        )
+        self.set_debris_4.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=4)
+        )
+        self.set_debris_5.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=5)
+        )
+
+        self.modify_viewmasks.stateChanged.connect(
+            self._viewerControls("viewmasks")
+        )
+        self.modify_viewlabels.stateChanged.connect(
+            self._viewerControls("viewlabels")
+        )
         self.refine_all.clicked.connect(self._refine_bacseg)
         self.modify_copymasktoall.clicked.connect(self._copymasktoall)
-        self.modify_deleteallmasks.clicked.connect(self._deleteallmasks(mode="all"))
-        self.modify_deleteactivemasks.clicked.connect(self._deleteallmasks(mode="active"))
-        self.modify_deleteactiveimage.clicked.connect(self._delete_active_image(mode="active"))
-        self.modify_deleteotherimages.clicked.connect(self._delete_active_image(mode="other"))
+        self.modify_deleteallmasks.clicked.connect(
+            self._deleteallmasks(mode="all")
+        )
+        self.modify_deleteactivemasks.clicked.connect(
+            self._deleteallmasks(mode="active")
+        )
+        self.modify_deleteactiveimage.clicked.connect(
+            self._delete_active_image(mode="active")
+        )
+        self.modify_deleteotherimages.clicked.connect(
+            self._delete_active_image(mode="other")
+        )
         self.find_next.clicked.connect(self._sort_cells("next"))
         self.find_previous.clicked.connect(self._sort_cells("previous"))
 
         # export events
         self.export_active.clicked.connect(self._export("active"))
         self.export_all.clicked.connect(self._export("all"))
-        self.export_statistics_active.clicked.connect(self._export_statistics("active"))
-        self.export_statistics_all.clicked.connect(self._export_statistics("all"))
+        self.export_statistics_active.clicked.connect(
+            self._export_statistics("active")
+        )
+        self.export_statistics_all.clicked.connect(
+            self._export_statistics("all")
+        )
 
         # oufti events
-        self.oufti_generate_all_midlines.clicked.connect(self.generate_midlines(mode="all"))
-        self.oufti_generate_active_midlines.clicked.connect(self.generate_midlines(mode="active"))
-        self.viewer.bind_key(key="m", func=self.midline_edit_toggle, overwrite=True)
+        self.oufti_generate_all_midlines.clicked.connect(
+            self.generate_midlines(mode="all")
+        )
+        self.oufti_generate_active_midlines.clicked.connect(
+            self.generate_midlines(mode="active")
+        )
+        self.viewer.bind_key(
+            key="m", func=self.midline_edit_toggle, overwrite=True
+        )
         self.oufti_edit_mode.clicked.connect(self.midline_edit_toggle)
         self.oufti_panzoom_mode.clicked.connect(self.midline_edit_toggle)
-        self.oufti_centre_all_midlines.clicked.connect(self.centre_oufti_midlines(mode="all"))
-        self.oufti_centre_active_midlines.clicked.connect(self.centre_oufti_midlines(mode="active"))
+        self.oufti_centre_all_midlines.clicked.connect(
+            self.centre_oufti_midlines(mode="all")
+        )
+        self.oufti_centre_active_midlines.clicked.connect(
+            self.centre_oufti_midlines(mode="active")
+        )
 
         # upload tab events
         self.upload_all.clicked.connect(self._uploadDatabase(mode="all"))
         self.upload_active.clicked.connect(self._uploadDatabase(mode="active"))
         self.database_download.clicked.connect(self._downloadDatabase)
         self.create_database.clicked.connect(self._create_bacseg_database)
         self.load_database.clicked.connect(self._load_bacseg_database)
         self.upload_initial.currentTextChanged.connect(self._populateUSERMETA)
 
         self.update_metadata.clicked.connect(self.update_database_metadata)
 
-
-
         # viewer event that call updateFileName when the slider is modified
         self.contours = []
         self.viewer.dims.events.current_step.connect(self._sliderEvent)
 
         # self.segImage = self.viewer.add_image(np.zeros((1,100,100),dtype=np.uint16),name="Image")
-        self.class_colours = {1: (255 / 255, 255 / 255, 255 / 255, 1), 2: (0 / 255, 255 / 255, 0 / 255, 1), 3: (0 / 255, 170 / 255, 255 / 255, 1), 4: (170 / 255, 0 / 255, 255 / 255, 1), 5: (
-        255 / 255, 170 / 255, 0 / 255, 1), 6: (255 / 255, 0 / 255, 0 / 255, 1), }
-
-        self.classLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=0.25, name="Classes", color=self.class_colours, metadata={0: {"image_name": ""}}, visible=False, )
-        self.segLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Segmentations", metadata={0: {"image_name": ""}}, )
-
+        self.class_colours = {
+            1: (255 / 255, 255 / 255, 255 / 255, 1),
+            2: (0 / 255, 255 / 255, 0 / 255, 1),
+            3: (0 / 255, 170 / 255, 255 / 255, 1),
+            4: (170 / 255, 0 / 255, 255 / 255, 1),
+            5: (255 / 255, 170 / 255, 0 / 255, 1),
+            6: (255 / 255, 0 / 255, 0 / 255, 1),
+        }
+
+        self.classLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=0.25,
+            name="Classes",
+            color=self.class_colours,
+            metadata={0: {"image_name": ""}},
+            visible=False,
+        )
+        self.segLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=1,
+            name="Segmentations",
+            metadata={0: {"image_name": ""}},
+        )
 
         self.segLayer.contour = 1
 
         # keyboard events, only triggered when viewer is not empty (an image is loaded/active)
-        self.viewer.bind_key(key="a", func=self._modifyMode(mode="add"), overwrite=True)
-        self.viewer.bind_key(key="e", func=self._modifyMode(mode="extend"), overwrite=True)
-        self.viewer.bind_key(key="j", func=self._modifyMode(mode="join"), overwrite=True)
-        self.viewer.bind_key(key="s", func=self._modifyMode(mode="split"), overwrite=True)
-        self.viewer.bind_key(key="d", func=self._modifyMode(mode="delete"), overwrite=True)
-        self.viewer.bind_key(key="r", func=self._modifyMode(mode="refine"), overwrite=True)
-        self.viewer.bind_key(key="Control-1", func=self._modifyMode(mode="single"), overwrite=True, )
-        self.viewer.bind_key(key="Control-2", func=self._modifyMode(mode="dividing"), overwrite=True, )
-        self.viewer.bind_key(key="Control-3", func=self._modifyMode(mode="divided"), overwrite=True, )
-        self.viewer.bind_key(key="Control-4", func=self._modifyMode(mode="vertical"), overwrite=True, )
-        self.viewer.bind_key(key="Control-5", func=self._modifyMode(mode="broken"), overwrite=True, )
-        self.viewer.bind_key(key="Control-6", func=self._modifyMode(mode="edge"), overwrite=True)
-        self.viewer.bind_key(key="F1", func=self._modifyMode(mode="panzoom"), overwrite=True)
-        self.viewer.bind_key(key="F2", func=self._modifyMode(mode="segment"), overwrite=True)
-        self.viewer.bind_key(key="F3", func=self._modifyMode(mode="classify"), overwrite=True)
-        self.viewer.bind_key(key="h", func=self._viewerControls("h"), overwrite=True)
-        self.viewer.bind_key(key="i", func=self._viewerControls("i"), overwrite=True)
-        self.viewer.bind_key(key="o", func=self._viewerControls("o"), overwrite=True)
-        self.viewer.bind_key(key="x", func=self._viewerControls("x"), overwrite=True)
-        self.viewer.bind_key(key="z", func=self._viewerControls("z"), overwrite=True)
-        self.viewer.bind_key(key="c", func=self._viewerControls("c"), overwrite=True)
-        self.viewer.bind_key(key="Right", func=self._imageControls("Right"), overwrite=True)
-        self.viewer.bind_key(key="Left", func=self._imageControls("Left"), overwrite=True)
-        self.viewer.bind_key(key="u", func=self._imageControls("Upload"), overwrite=True)
-        self.viewer.bind_key(key="Control-d", func=self._deleteallmasks(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-d", func=self._deleteallmasks(mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Control-i", func=self._delete_active_image(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-i", func=self._delete_active_image(mode="other"), overwrite=True, )
+        self.viewer.bind_key(
+            key="a", func=self._modifyMode(mode="add"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="e", func=self._modifyMode(mode="extend"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="j", func=self._modifyMode(mode="join"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="s", func=self._modifyMode(mode="split"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="d", func=self._modifyMode(mode="delete"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="r", func=self._modifyMode(mode="refine"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="k", func=self._modifyMode(mode="clicktozoom"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-1",
+            func=self._modifyMode(mode="single"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-2",
+            func=self._modifyMode(mode="dividing"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-3",
+            func=self._modifyMode(mode="divided"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-4",
+            func=self._modifyMode(mode="vertical"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-5",
+            func=self._modifyMode(mode="broken"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-6", func=self._modifyMode(mode="edge"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F1", func=self._modifyMode(mode="panzoom"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F2", func=self._modifyMode(mode="segment"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F3", func=self._modifyMode(mode="classify"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="h", func=self._viewerControls("h"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="i", func=self._viewerControls("i"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="o", func=self._viewerControls("o"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="x", func=self._viewerControls("x"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="z", func=self._viewerControls("z"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="c", func=self._viewerControls("c"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Right", func=self._imageControls("Right"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Left", func=self._imageControls("Left"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="u", func=self._imageControls("Upload"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-d",
+            func=self._deleteallmasks(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-d",
+            func=self._deleteallmasks(mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-i",
+            func=self._delete_active_image(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-i",
+            func=self._delete_active_image(mode="other"),
+            overwrite=True,
+        )
+
+        self.viewer.bind_key(
+            key="Control-l", func=self._downloadDatabase(), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-u",
+            func=self._uploadDatabase(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-u",
+            func=self._uploadDatabase(mode="all"),
+            overwrite=True,
+        )
         #
-        self.viewer.bind_key(key="Control-l", func=self._downloadDatabase(), overwrite=True)
-        self.viewer.bind_key(key="Control-u", func=self._uploadDatabase(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-u", func=self._uploadDatabase(mode="all"), overwrite=True, )
-        #
-        self.viewer.bind_key(key="Control-Left", func=self._manual_align_channels("left", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Right", func=self._manual_align_channels("right", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Up", func=self._manual_align_channels("up", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Down", func=self._manual_align_channels("down", mode="active"), overwrite=True, )
-
-        self.viewer.bind_key(key="Alt-Left", func=self._manual_align_channels("left", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Right", func=self._manual_align_channels("right", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Up", func=self._manual_align_channels("up", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Down", func=self._manual_align_channels("down", mode="all"), overwrite=True, )
-
-        self.import_filemode.currentIndexChanged.connect(self.update_import_limit)
+        self.viewer.bind_key(
+            key="Control-Left",
+            func=self._manual_align_channels("left", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Right",
+            func=self._manual_align_channels("right", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Up",
+            func=self._manual_align_channels("up", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Down",
+            func=self._manual_align_channels("down", mode="active"),
+            overwrite=True,
+        )
+
+        self.viewer.bind_key(
+            key="Alt-Left",
+            func=self._manual_align_channels("left", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Right",
+            func=self._manual_align_channels("right", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Up",
+            func=self._manual_align_channels("up", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Down",
+            func=self._manual_align_channels("down", mode="all"),
+            overwrite=True,
+        )
+
+        self.import_filemode.currentIndexChanged.connect(
+            self.update_import_limit
+        )
         self.update_import_limit()
 
         # mouse events
         self.segLayer.mouse_drag_callbacks.append(self._segmentationEvents)
-        self.segLayer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+        # self.segLayer.mouse_move_callbac1ks.append(self._zoomEvents)
+        self.segLayer.mouse_double_click_callbacks.append(
+            self._doubeClickEvents
+        )
 
         # viewer events
         self.viewer.layers.events.inserted.connect(self._manualImport)
-        self.viewer.layers.selection.events.changed.connect(self._updateFileName)
+        self.viewer.layers.events.removed.connect(
+            self._updateSegmentationCombo
+        )
+        self.viewer.layers.selection.events.changed.connect(
+            self._updateFileName
+        )
 
         self.threadpool = QThreadPool()  # self.load_dev_data()
 
         self.widget_notifications = True
 
+    def _align_images(self, viewer=None, mode="active"):
+        import scipy
+        from skimage.registration import phase_cross_correlation
 
-    def set_image_quality(self, mode = "", value =""):
+        try:
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Classes", "center_lines"]
+            ]
+
+            if len(layer_names) > 2:
+                num_images = self.viewer.layers[layer_names[0]].data.shape[0]
+
+                if mode == "active":
+                    fov_list = [self.viewer.dims.current_step[0]]
+                else:
+                    fov_list = range(num_images)
+
+                alignment_channel = self.alignment_channel.currentText()
+                current_fov = self.viewer.dims.current_step[0]
+
+                target_channels = [
+                    layer
+                    for layer in layer_names
+                    if layer != alignment_channel
+                ]
+
+                for channel in target_channels:
+                    image_stack = self.viewer.layers[channel].data.copy()
+                    target_image_stack = self.viewer.layers[
+                        alignment_channel
+                    ].data.copy()
+
+                    for fov in fov_list:
+                        target_image = image_stack[fov, :, :]
+                        alignment_image = target_image_stack[fov, :, :]
+
+                        shift, error, diffphase = phase_cross_correlation(
+                            alignment_image, target_image, upsample_factor=100
+                        )
+
+                        shifted_img = scipy.ndimage.shift(target_image, shift)
+
+                        image_stack[fov, :, :] = shifted_img
+
+                    self.viewer.layers[channel].data = image_stack
+
+                show_info(
+                    f"{len(fov_list)} Image(s) aligned to channel: "
+                    + alignment_channel
+                )
+
+        except:
+            pass
 
+    def set_blurred(self, viewer=None):
+        self.set_image_quality(mode="focus", value=1)
+
+    def set_focused(self, viewer=None):
+        self.set_image_quality(mode="focus", value=5)
+
+    def set_image_quality(self, mode="", value=""):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Classes", "center_lines"]
+            ]
 
             update_mode = self.set_quality_mode.currentIndex()
 
             if len(layer_names) > 0:
-
                 current_fov = self.viewer.dims.current_step[0]
                 n_frames = self.viewer.dims.nsteps[0]
                 active_layer = self.viewer.layers.selection.active.name
 
                 if update_mode == 0:
                     frames = [current_fov]
                     layers = [active_layer]
@@ -600,27 +1207,24 @@
                     layers = [active_layer]
                 if update_mode == 3:
                     frames = np.arange(n_frames)
                     layers = layer_names
 
                 for layer in layers:
                     for frame in frames:
-
                         meta = self.viewer.layers[layer].metadata.copy()
 
                         meta[frame][f"image_{mode}"] = value
 
                         self.viewer.layers[layer].metadata = meta
 
             self._updateFileName()
 
         except:
             print(traceback.format_exc())
-            pass
-
 
     def wrapper(self, func, *args, **kwargs):
         try:
             func_name = func.__name__
 
             func = partial(func, self, *args, **kwargs)
             func.__name__ = func_name
@@ -630,21 +1234,27 @@
         except:
             pass
 
         return func
 
     def overwrite_channel_info(self):
         all_layers = [layer.name for layer in self.viewer.layers]
-        selected_layers = [layer.name for layer in self.viewer.layers.selection]
+        selected_layers = [
+            layer.name for layer in self.viewer.layers.selection
+        ]
 
         if len(selected_layers) == 1:
             selected_layer = selected_layers[0]
             all_layers.pop(all_layers.index(selected_layer))
 
-            if selected_layer not in ["Segmentations", "Classes", "center_lines", ]:
+            if selected_layer not in [
+                "Segmentations",
+                "Classes",
+                "center_lines",
+            ]:
                 metadata = self.viewer.layers[selected_layer].metadata.copy()
 
                 label_modality = self.label_modality.currentText()
                 label_light_source = self.label_light_source.currentText()
                 label_stain = self.label_stain.currentText()
                 label_stain_target = self.label_stain_target.currentText()
 
@@ -684,47 +1294,74 @@
             colicoords_channel = colicoords_channel.replace("Mask + ", "")
 
             if pixel_size <= 0:
                 pixel_size = 1
 
             desktop = os.path.expanduser("~/Desktop")
 
-            path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+            path = QFileDialog.getExistingDirectory(
+                self, "Select Directory", desktop
+            )
 
             colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
 
             if os.path.isdir(colicoords_dir) != True:
                 os.mkdir(colicoords_dir)
             else:
                 shutil.rmtree(colicoords_dir)
                 os.mkdir(colicoords_dir)
 
             if os.path.isdir(path):
                 path = os.path.abspath(path)
 
-                from napari_bacseg._utils_statistics import (get_cell_statistics, process_cell_statistics, )
+                from napari_bacseg._utils_statistics import (
+                    get_cell_statistics,
+                    process_cell_statistics,
+                )
 
                 self.get_cell_statistics = self.wrapper(get_cell_statistics)
-                self.process_cell_statistics = self.wrapper(process_cell_statistics)
-
-                worker = Worker(self.get_cell_statistics, mode=mode, pixel_size=pixel_size, colicoords_dir=colicoords_dir, )
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
-                worker.signals.result.connect(self.process_cell_statistics(path=path))
+                self.process_cell_statistics = self.wrapper(
+                    process_cell_statistics
+                )
+
+                worker = Worker(
+                    self.get_cell_statistics,
+                    mode=mode,
+                    pixel_size=pixel_size,
+                    colicoords_dir=colicoords_dir,
+                )
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
+                worker.signals.result.connect(
+                    self.process_cell_statistics(path=path)
+                )
                 self.threadpool.start(worker)
                 cell_data = worker.result()
 
                 if self.export_colicoords_mode.currentIndex() != 0:
                     from napari_bacseg._utils_colicoords import run_colicoords
 
                     self.run_colicoords = self.wrapper(run_colicoords)
 
-                    worker = Worker(self.run_colicoords, cell_data=cell_data, colicoords_channel=colicoords_channel, pixel_size=pixel_size, statistics=True, multithreaded=multithreaded, )
-
-                    worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
-                    worker.signals.result.connect(self.process_cell_statistics(path=path))
+                    worker = Worker(
+                        self.run_colicoords,
+                        cell_data=cell_data,
+                        colicoords_channel=colicoords_channel,
+                        pixel_size=pixel_size,
+                        statistics=True,
+                        multithreaded=multithreaded,
+                    )
+
+                    worker.signals.progress.connect(
+                        partial(self._Progresbar, progressbar="export")
+                    )
+                    worker.signals.result.connect(
+                        self.process_cell_statistics(path=path)
+                    )
                     self.threadpool.start(worker)
 
         return _event
 
     def update_import_limit(self):
         if self.import_filemode.currentIndex() == 0:
             self.import_limit.setEnabled(False)
@@ -759,34 +1396,49 @@
                     criterion = meta["simple_cell_stats"]["cell_area"]
                 if find_criterion == "Cell Solidity":
                     criterion = meta["simple_cell_stats"]["cell_solidity"]
                 if find_criterion == "Cell Aspect Ratio":
                     criterion = meta["simple_cell_stats"]["cell_aspect_ratio"]
 
                 if find_mode == "Ascending":
-                    criterion, cell_centre, cell_zoom = zip(*sorted(zip(criterion, cell_centre, cell_zoom), key=lambda x: x[0], ))
+                    criterion, cell_centre, cell_zoom = zip(
+                        *sorted(
+                            zip(criterion, cell_centre, cell_zoom),
+                            key=lambda x: x[0],
+                        )
+                    )
                 else:
-                    criterion, cell_centre, cell_zoom = zip(*sorted(zip(criterion, cell_centre, cell_zoom), key=lambda x: x[0], reverse=True, ))
-
-                current_position = tuple(np.array(self.viewer.camera.center).round())
+                    criterion, cell_centre, cell_zoom = zip(
+                        *sorted(
+                            zip(criterion, cell_centre, cell_zoom),
+                            key=lambda x: x[0],
+                            reverse=True,
+                        )
+                    )
+
+                current_position = tuple(
+                    np.array(self.viewer.camera.center).round()
+                )
 
                 if current_position not in cell_centre:
                     self.viewer.camera.center = cell_centre[0]
                     self.viewer.camera.zoom = cell_zoom[0]
 
                 else:
                     current_index = cell_centre.index(current_position)
 
                     if order == "next":
                         new_index = current_index + 1
 
                     if order == "previous":
                         new_index = current_index - 1
 
-                    new_index = max(current_fov, min(new_index, len(cell_centre) - 1))
+                    new_index = max(
+                        current_fov, min(new_index, len(cell_centre) - 1)
+                    )
 
                     self.viewer.camera.center = cell_centre[new_index]
                     self.viewer.camera.zoom = cell_zoom[new_index]
 
             except:
                 pass
 
@@ -811,15 +1463,19 @@
             elif key == "right":
                 shift_vector = [0.0, 1.0]
             else:
                 shift_vector = [0.0, 0.0]
 
             shift_image = False
             if active_layer != None:
-                if active_layer.name not in ["Segmentations", "Classes", "center_lines", ]:
+                if active_layer.name not in [
+                    "Segmentations",
+                    "Classes",
+                    "center_lines",
+                ]:
                     shift_image = True
 
             if shift_image is True:
                 if mode == "active":
                     image_stack = active_layer.data.copy()
                     image = image_stack[current_fov, :, :]
                     image = shift(image, shift=shift_vector)
@@ -867,84 +1523,145 @@
 
         channel = self.refine_channel.currentText()
         colicoords_channel = channel.replace("Mask + ", "")
 
         mask_stack = self.segLayer.data
         mask = mask_stack[current_fov, :, :].copy()
 
-        from napari_bacseg._utils_colicoords import (process_colicoords, run_colicoords, )
+        from napari_bacseg._utils_colicoords import (
+            process_colicoords,
+            run_colicoords,
+        )
         from napari_bacseg._utils_statistics import get_cell_statistics
 
         self.get_cell_statistics = self.wrapper(get_cell_statistics)
         self.run_colicoords = self.wrapper(run_colicoords)
         self.process_colicoords = self.wrapper(process_colicoords)
 
         colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
 
-        worker = Worker(self.get_cell_statistics, mode="active", pixel_size=pixel_size, colicoords_dir=colicoords_dir, )
+        worker = Worker(
+            self.get_cell_statistics,
+            mode="active",
+            pixel_size=pixel_size,
+            colicoords_dir=colicoords_dir,
+        )
 
         self.threadpool.start(worker)
         cell_data = worker.result()
 
-        worker = Worker(self.run_colicoords, cell_data=cell_data, colicoords_channel=colicoords_channel, pixel_size=pixel_size, multithreaded=True, )
-
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="modify"))
+        worker = Worker(
+            self.run_colicoords,
+            cell_data=cell_data,
+            colicoords_channel=colicoords_channel,
+            pixel_size=pixel_size,
+            multithreaded=True,
+        )
+
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="modify")
+        )
         worker.signals.result.connect(self.process_colicoords)
         self.threadpool.start(worker)
 
     def _uploadDatabase(self, viewer=None, mode=""):
         def _event(viewer):
             try:
-                if (self.database_path != "" and os.path.exists(self.database_path) == True):
+                if (
+                    self.database_path != ""
+                    and os.path.exists(self.database_path) == True
+                ):
                     if self.unfolded == True:
                         self.fold_images()
 
-                    from napari_bacseg._utils_database_IO import (_upload_bacseg_database, )
-
-                    self._upload_bacseg_database = self.wrapper(_upload_bacseg_database)
-
-                    worker = Worker(self._upload_bacseg_database, mode=mode)
-                    worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
-                    self.threadpool.start(worker)
-
+                    if self.upload_initial.currentText() in [
+                        "",
+                        "Required for upload",
+                    ]:
+                        show_info("Please select the user initial.")
+                    else:
+                        from napari_bacseg._utils_database_IO import (
+                            _upload_bacseg_database,
+                        )
+
+                        self._upload_bacseg_database = self.wrapper(
+                            _upload_bacseg_database
+                        )
+
+                        worker = Worker(
+                            self._upload_bacseg_database, mode=mode
+                        )
+                        worker.signals.progress.connect(
+                            partial(self._Progresbar, progressbar="database")
+                        )
+                        self.threadpool.start(worker)
             except:
                 pass
 
         return _event
 
     def _downloadDatabase(self, viewer=None):
         try:
-            if (self.database_path != "" and os.path.exists(self.database_path) == True):
+            if (
+                self.database_path != ""
+                and os.path.exists(self.database_path) == True
+            ):
                 if self.unfolded == True:
                     self.fold_images()
 
-                from napari_bacseg._utils_database_IO import (get_filtered_database_metadata, read_bacseg_images, )
-
-                self.get_filtered_database_metadata = self.wrapper(get_filtered_database_metadata)
-                self.read_bacseg_images = self.wrapper(read_bacseg_images)
-
-                self.active_import_mode = "BacSeg"
-
-                (measurements, file_paths, channels,) = self.get_filtered_database_metadata()
-
-                if len(file_paths) == 0:
-                    if self.widget_notifications:
-                        show_info("no matching database files found")
+                if self.upload_initial.currentText() in [
+                    "",
+                    "Required for upload",
+                ]:
+                    show_info("Please select the user initial.")
 
                 else:
-                    worker = Worker(self.read_bacseg_images, measurements=measurements, channels=channels, )
-                    worker.signals.result.connect(self._process_import)
-                    worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
-                    self.threadpool.start(worker)
+                    from napari_bacseg._utils_database_IO import (
+                        get_filtered_database_metadata,
+                        read_bacseg_images,
+                    )
+
+                    self.get_filtered_database_metadata = self.wrapper(
+                        get_filtered_database_metadata
+                    )
+                    self.read_bacseg_images = self.wrapper(read_bacseg_images)
+
+                    self.active_import_mode = "BacSeg"
+
+                    (
+                        measurements,
+                        file_paths,
+                        channels,
+                    ) = self.get_filtered_database_metadata()
+
+                    if len(file_paths) == 0:
+                        if self.widget_notifications:
+                            show_info("no matching database files found")
+
+                    else:
+                        worker = Worker(
+                            self.read_bacseg_images,
+                            measurements=measurements,
+                            channels=channels,
+                        )
+                        worker.signals.result.connect(self._process_import)
+                        worker.signals.progress.connect(
+                            partial(self._Progresbar, progressbar="database")
+                        )
+                        self.threadpool.start(worker)
 
         except:
             print(traceback.format_exc())
 
     def _updateSegChannels(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name not in ["Segmentations", "Classes", "center_lines"]
+        ]
 
         segChannel = self.cellpose_segchannel.currentText()
 
         self.export_channel.setCurrentText(segChannel)
 
     def _Progresbar(self, progress, progressbar):
         if progressbar == "import":
@@ -984,394 +1701,669 @@
         if import_mode == "JSON (.txt) Segmentation(s)":
             file_extension = "*.txt"
 
         desktop = os.path.expanduser("~/Desktop")
 
         if type(paths) is not list:
             if import_filemode == "Import File(s)":
-                paths, _ = QFileDialog.getOpenFileNames(self, "Open Files", desktop, f"Files ({file_extension})")
+                paths, _ = QFileDialog.getOpenFileNames(
+                    self, "Open Files", desktop, f"Files ({file_extension})"
+                )
 
             if import_filemode == "Import Directory":
-                path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                path = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 paths = [path]
 
         if "" in paths or paths == [] or type(paths) is not list:
             if self.widget_notifications:
                 show_info("No file/folder selected")
 
         else:
             if import_mode == "Images":
-                self.import_images = self.wrapper(napari_bacseg._utils.import_images)
+                self.import_images = self.wrapper(
+                    napari_bacseg._utils.import_images
+                )
 
                 worker = Worker(self.import_images, file_paths=paths)
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "NanoImager Data":
-                self.read_nim_directory = self.wrapper(napari_bacseg._utils.read_nim_directory)
-                self.read_nim_images = self.wrapper(napari_bacseg._utils.read_nim_images)
-
-                measurements, file_paths, channels = self.read_nim_directory(paths)
-
-                worker = Worker(self.read_nim_images, measurements=measurements, channels=channels, )
+                self.read_nim_directory = self.wrapper(
+                    napari_bacseg._utils.read_nim_directory
+                )
+                self.read_nim_images = self.wrapper(
+                    napari_bacseg._utils.read_nim_images
+                )
+
+                measurements, file_paths, channels = self.read_nim_directory(
+                    paths
+                )
+
+                worker = Worker(
+                    self.read_nim_images,
+                    measurements=measurements,
+                    channels=channels,
+                )
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "Mask (.tif) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".tif")
                 self._autoClassify()
 
             if import_mode == "Cellpose (.npy) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".npy")
                 self._autoClassify()
 
             if import_mode == "Oufti (.mat) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".mat")
                 self._autoClassify()
 
             if import_mode == "JSON (.txt) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".txt")
                 self._autoClassify()
 
             if import_mode == "ImageJ files(s)":
-                self.import_imagej = self.wrapper(napari_bacseg._utils.import_imagej)
+                self.import_imagej = self.wrapper(
+                    napari_bacseg._utils.import_imagej
+                )
 
                 worker = Worker(self.import_imagej, paths=paths)
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "ScanR Data":
-                from napari_bacseg._utils import (read_scanr_directory, read_scanr_images, )
+                from napari_bacseg._utils import (
+                    read_scanr_directory,
+                    read_scanr_images,
+                )
 
                 self.read_scanr_images = self.wrapper(read_scanr_images)
 
-                measurements, file_paths, channels = read_scanr_directory(self, paths)
-
-                worker = Worker(self.read_scanr_images, measurements=measurements, channels=channels, )
+                measurements, file_paths, channels = read_scanr_directory(
+                    self, paths
+                )
+
+                worker = Worker(
+                    self.read_scanr_images,
+                    measurements=measurements,
+                    channels=channels,
+                )
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
-    def _export(self, mode):
+    def _export(self, mode, viewer=None):
         def _event(viewer):
             # if self.unfolded == True:
             #     self.fold_images()
 
             execute_export = True
 
             if self.export_location.currentIndex() == 1:
                 desktop = os.path.expanduser("~/Desktop")
-                self.export_directory = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                self.export_directory = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 if self.export_directory == "":
                     execute_export = False
 
             if execute_export == True:
-                self.export_files = self.wrapper(napari_bacseg._utils.export_files)
+                self.export_files = self.wrapper(
+                    napari_bacseg._utils.export_files
+                )
 
                 worker = Worker(self.export_files, mode=mode)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
                 self.threadpool.start(worker)
 
         return _event
 
     def _trainCellpose(self):
         if self.unfolded == True:
             self.fold_images()
 
         from napari_bacseg._utils_cellpose import train_cellpose_model
 
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
 
         worker = Worker(self.train_cellpose_model)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose_train"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose_train")
+        )
         self.threadpool.start(worker)
 
     def _segmentActive(self):
         if self.unfolded == True:
             self.fold_images()
 
-        from napari_bacseg._utils_cellpose import (_process_cellpose, _run_cellpose, )
+        from napari_bacseg._utils_cellpose import (
+            _process_cellpose,
+            _run_cellpose,
+        )
 
         self._run_cellpose = self.wrapper(_run_cellpose)
         self._process_cellpose = self.wrapper(_process_cellpose)
 
         current_fov = self.viewer.dims.current_step[0]
         chanel = self.cellpose_segchannel.currentText()
 
         images = self.viewer.layers[chanel].data
 
         image = [images[current_fov, :, :]]
 
         worker = Worker(self._run_cellpose, images=image)
         worker.signals.result.connect(self._process_cellpose)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose")
+        )
         self.threadpool.start(worker)
 
     def _segmentAll(self):
         if self.unfolded == True:
             self.fold_images()
 
-        from napari_bacseg._utils_cellpose import (_process_cellpose, _run_cellpose, )
+        from napari_bacseg._utils_cellpose import (
+            _process_cellpose,
+            _run_cellpose,
+        )
 
         self._run_cellpose = self.wrapper(_run_cellpose)
         self._process_cellpose = self.wrapper(_process_cellpose)
 
         channel = self.cellpose_segchannel.currentText()
 
         images = self.viewer.layers[channel].data
 
         images = unstack_images(images)
 
         worker = Worker(self._run_cellpose, images=images)
         worker.signals.result.connect(self._process_cellpose)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose")
+        )
         self.threadpool.start(worker)
 
     def _updateSliderLabel(self, slider_name, label_name):
         self.slider = self.findChild(QSlider, slider_name)
         self.label = self.findChild(QLabel, label_name)
 
         slider_value = self.slider.value()
 
-        if (slider_name == "cellpose_flowthresh" or slider_name == "cellpose_maskthresh"):
+        if (
+            slider_name == "cellpose_flowthresh"
+            or slider_name == "cellpose_maskthresh"
+        ):
             self.label.setText(str(slider_value / 100))
         else:
             self.label.setText(str(slider_value))
 
     def _updateSegmentationCombo(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name not in ["Segmentations", "Classes", "center_lines"]
+        ]
 
         self.cellpose_segchannel.clear()
         self.cellpose_segchannel.addItems(layer_names)
 
         self.cellpose_trainchannel.clear()
         self.cellpose_trainchannel.addItems(layer_names)
 
         self.cellpose_trainchannel.clear()
         self.cellpose_trainchannel.addItems(layer_names)
 
+        self.alignment_channel.clear()
+        self.alignment_channel.addItems(layer_names)
+
         self.export_channel.clear()
         export_layers = layer_names
-        export_layers.extend(["All Channels (Stack)", "First Three Channels (RGB)"])
+        export_layers.extend(
+            ["All Channels (Stack)", "First Three Channels (RGB)"]
+        )
         self.export_channel.addItems(export_layers)
 
         self.refine_channel.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
         self.refine_channel.addItems(["Mask"] + refine_layers)
 
         self.export_colicoords_mode.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
-        self.export_colicoords_mode.addItems(["None (OpenCV Stats)", "Mask"] + refine_layers)
+        self.export_colicoords_mode.addItems(
+            ["None (OpenCV Stats)", "Mask"] + refine_layers
+        )
 
     def _sliderEvent(self, current_step):
+        try:
+            active_layer = self.viewer.layers.selection.active
+
+            crop = active_layer.corner_pixels.T
+
+            y_range = crop[-2]
+            x_range = crop[-1]
+        except:
+            pass
+
         self._updateFileName()
         self._autoContrast()
+        self._updateScaleBar()
         self._update_active_midlines()
 
+    def _updateScaleBar(self):
+        layer_names = [layer.name for layer in self.viewer.layers]
+
+        try:
+            if self.scalebar_show.isChecked() and len(layer_names) > 0:
+                pixel_resolution = float(self.scalebar_resolution.text())
+                scalebar_units = self.scalebar_units.currentText()
+
+                if pixel_resolution > 0:
+                    for layer in layer_names:
+                        self.viewer.layers[layer].scale = [
+                            1,
+                            pixel_resolution,
+                            pixel_resolution,
+                        ]
+
+                        self.viewer.scale_bar.visible = True
+                        self.viewer.scale_bar.unit = scalebar_units
+                        self.viewer.reset_view()
+
+            else:
+                self.viewer.scale_bar.visible = False
+
+        except:
+            self.viewer.scale_bar.visible = False
+
     def _autoContrast(self):
         try:
             if self.autocontrast.isChecked():
-                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+                layer_names = [
+                    layer.name
+                    for layer in self.viewer.layers
+                    if layer.name
+                    not in ["Segmentations", "Classes", "center_lines"]
+                ]
 
                 if len(layer_names) != 0:
                     active_layer = layer_names[-1]
 
-                    image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
-
-                    image = (self.viewer.layers[str(active_layer)].data[image_dims].copy())
-
-                    crop = self.viewer.layers[str(active_layer)].corner_pixels[:, -2:]
+                    image_dims = tuple(
+                        list(self.viewer.dims.current_step[:-2]) + [...]
+                    )
+
+                    image = (
+                        self.viewer.layers[str(active_layer)]
+                        .data[image_dims]
+                        .copy()
+                    )
+
+                    crop = self.viewer.layers[str(active_layer)].corner_pixels[
+                        :, -2:
+                    ]
 
                     [[y1, x1], [y2, x2]] = crop
 
                     image_crop = image[y1:y2, x1:x2]
 
-                    contrast_limit = [np.min(image_crop), np.max(image_crop)]
+                    contrast_limit = np.percentile(
+                        image_crop[image_crop != 0], (1, 99)
+                    )
+                    contrast_limit = [
+                        int(contrast_limit[0] * 0.5),
+                        int(contrast_limit[1] * 2),
+                    ]
 
                     if contrast_limit[1] > contrast_limit[0]:
-                        self.viewer.layers[str(active_layer)].contrast_limits = contrast_limit
+                        self.viewer.layers[
+                            str(active_layer)
+                        ].contrast_limits = contrast_limit
 
         except:
             pass
 
     def _updateFileName(self):
         try:
             current_fov = self.viewer.dims.current_step[0]
             active_layer = self.viewer.layers.selection.active
 
-            metadata = self.viewer.layers[str(active_layer)].metadata[current_fov]
-
-            file_name = metadata["image_name"]
-            channel = metadata["channel"]
-
-            viewer_text = f"File Name: {file_name}"
-
-            if "modality" in metadata.keys():
-                modality = metadata["modality"]
-                viewer_text = viewer_text + f"\nModality: {modality}"
+            image = self.viewer.layers[str(active_layer)].data[current_fov]
+            metadata = self.viewer.layers[str(active_layer)].metadata[
+                current_fov
+            ]
+
+            viewer_text = ""
+
+            if (
+                self.overlay_filename.isChecked()
+                and "image_name" in metadata.keys()
+            ):
+                viewer_text = f"File Name: {metadata['image_name']}"
+            if self.overlay_folder.isChecked() and "folder" in metadata.keys():
+                viewer_text = viewer_text + f"\nFolder: {metadata['folder']}"
+            if (
+                self.overlay_microscope.isChecked()
+                and "microscope" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nMicroscope: {metadata['microscope']}"
+                )
+            if (
+                self.overlay_datemodified.isChecked()
+                and "date_modified" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text
+                    + f"\nDate Modified: {metadata['date_modified']}"
+                )
+            if (
+                self.overlay_content.isChecked()
+                and "content" in metadata.keys()
+            ):
+                viewer_text = viewer_text + f"\nContent: {metadata['content']}"
+            if self.overlay_strain.isChecked() and "strain" in metadata.keys():
+                viewer_text = viewer_text + f"\nStrain: {metadata['strain']}"
+            if (
+                self.overlay_phenotype.isChecked()
+                and "phenotype" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nPhenotype: {metadata['phenotype']}"
+                )
+            if (
+                self.overlay_antibiotic.isChecked()
+                and "antibiotic" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nAntibiotic: {metadata['antibiotic']}"
+                )
+            if self.overlay_stain.isChecked() and "stain" in metadata.keys():
+                viewer_text = viewer_text + f"\nStain: {metadata['stain']}"
+            if (
+                self.overlay_staintarget.isChecked()
+                and "stain_target" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nStain Target: {metadata['stain_target']}"
+                )
+            if (
+                self.overlay_modality.isChecked()
+                and "modality" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nModality: {metadata['modality']}"
+                )
+            if (
+                self.overlay_lightsource.isChecked()
+                and "source" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nLight Source: {metadata['source']}"
+                )
+            if (
+                self.overlay_focus.isChecked()
+                and "image_focus" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nImage Focus: {metadata['image_focus']}"
+                )
+            if (
+                self.overlay_debris.isChecked()
+                and "image_debris" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nImage Debris: {metadata['image_debris']}"
+                )
+            if self.overlay_laplacian.isChecked():
+                image_laplacian = np.mean(cv2.Laplacian(image, cv2.CV_64F))
+                viewer_text = viewer_text + f"\nLaplacian: {image_laplacian}"
+            if self.overlay_range.isChecked():
+                image_range = np.max(image) - np.min(image)
+                viewer_text = viewer_text + f"\nRange: {image_range}"
+
+            if viewer_text != "":
+                self.viewer.text_overlay.visible = True
+                self.viewer.text_overlay.text = viewer_text.lstrip("\n")
             else:
-                viewer_text = viewer_text + f"\nModality: None"
-
-            if "light_source" in metadata.keys():
-                light_source = metadata["light_source"]
-                viewer_text = viewer_text + f"\nLight Source: {light_source}"
-            else:
-                viewer_text = viewer_text + f"\nLight Source: None"
-
-            if "stain" in metadata.keys():
-                stain = metadata["stain"]
-                viewer_text = viewer_text + f"\nStain: {stain}"
-            else:
-                viewer_text = viewer_text + f"\nStain: None"
-
-            if "stain_target" in metadata.keys():
-                stain_target = metadata["stain_target"]
-                viewer_text = viewer_text + f"\nStain Target: {stain_target}"
-            else:
-                viewer_text = viewer_text + f"\nStain Target: None"
-
-            if "image_focus" in metadata.keys():
-                image_focus = metadata["image_focus"]
-                viewer_text = viewer_text + f"\nImage Focus: {image_focus}"
-            else:
-                viewer_text = viewer_text + f"\nImage Focus: None"
-
-            if "image_debris" in metadata.keys():
-                image_debris = metadata["image_debris"]
-                viewer_text = viewer_text + f"\nImage Debris: {image_debris}"
-            else:
-                viewer_text = viewer_text + f"\nImage Debris: None"
-
-            self.viewer.text_overlay.visible = True
-
-            self.viewer.text_overlay.text = viewer_text
+                self.viewer.text_overlay.visible = False
 
         except:
             pass
 
     def _process_import(self, imported_data, rearrange=True):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name not in ["Segmentations", "Classes", "center_lines"]
+        ]
 
         if self.clear_previous.isChecked() == True:
             # removes all layers (except segmentation layer)
             for layer_name in layer_names:
                 self.viewer.layers.remove(self.viewer.layers[layer_name])
             # reset segmentation and class layers
             self.segLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
             self.classLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
 
         imported_images = imported_data["imported_images"]
 
+        self.viewer.dims.set_current_step(0, 0)
+
         for layer_name, layer_data in imported_images.items():
             images = layer_data["images"]
             masks = layer_data["masks"]
             classes = layer_data["classes"]
             metadata = layer_data["metadata"]
 
             from napari_bacseg._utils import stack_images
 
             new_image_stack, new_metadata = stack_images(images, metadata)
             new_mask_stack, new_metadata = stack_images(masks, metadata)
             new_class_stack, new_metadata = stack_images(classes, metadata)
 
             if len(new_mask_stack) == 0:
-                new_mask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_mask_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             if len(new_class_stack) == 0:
-                new_class_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_class_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             colormap = "gray"
 
             if layer_name == "405":
                 colormap = "green"
             if layer_name == "532":
                 colormap = "red"
             if layer_name == "Cy3":
                 colormap = "red"
             if layer_name == "DAPI":
                 colormap = "green"
 
-            if (self.clear_previous.isChecked() == False and layer_name in layer_names):
+            if (
+                self.clear_previous.isChecked() == False
+                and layer_name in layer_names
+            ):
                 current_image_stack = self.viewer.layers[layer_name].data
                 current_metadata = self.viewer.layers[layer_name].metadata
                 current_mask_stack = self.segLayer.data
                 current_class_stack = self.classLayer.data
 
                 if len(current_image_stack) == 0:
-                    setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
+                    setattr(
+                        self,
+                        layer_name,
+                        self.viewer.add_image(
+                            new_image_stack,
+                            name=layer_name,
+                            colormap=colormap,
+                            gamma=0.8,
+                            metadata=new_metadata,
+                        ),
+                    )
 
                     image_layer = getattr(self, layer_name)
-                    image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                    image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                    image_layer.mouse_drag_callbacks.append(
+                        self._segmentationEvents
+                    )
+                    image_layer.mouse_double_click_callbacks.append(
+                        self._doubeClickEvents
+                    )
 
                     self.segLayer.data = new_mask_stack
                     self.classLayer.data = new_class_stack
                     self.segLayer.metadata = new_metadata
 
                 else:
                     from napari_bacseg._utils import append_image_stacks
 
-                    (appended_image_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_image_stack, new_image_stack, )
-
-                    (appended_mask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_mask_stack, new_mask_stack, )
-
-                    (appended_class_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_class_stack, new_class_stack, )
+                    (
+                        appended_image_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_image_stack,
+                        new_image_stack,
+                    )
+
+                    (
+                        appended_mask_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_mask_stack,
+                        new_mask_stack,
+                    )
+
+                    (
+                        appended_class_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_class_stack,
+                        new_class_stack,
+                    )
 
                     self.viewer.layers.remove(self.viewer.layers[layer_name])
 
-                    setattr(self, layer_name, self.viewer.add_image(appended_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=appended_metadata, ), )
+                    setattr(
+                        self,
+                        layer_name,
+                        self.viewer.add_image(
+                            appended_image_stack,
+                            name=layer_name,
+                            colormap=colormap,
+                            gamma=0.8,
+                            metadata=appended_metadata,
+                        ),
+                    )
 
                     image_layer = getattr(self, layer_name)
-                    image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                    image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                    image_layer.mouse_drag_callbacks.append(
+                        self._segmentationEvents
+                    )
+                    image_layer.mouse_double_click_callbacks.append(
+                        self._doubeClickEvents
+                    )
 
                     self.segLayer.data = appended_mask_stack
                     self.classLayer.data = appended_class_stack
                     self.segLayer.metadata = appended_metadata
 
             else:
-                setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
+                setattr(
+                    self,
+                    layer_name,
+                    self.viewer.add_image(
+                        new_image_stack,
+                        name=layer_name,
+                        colormap=colormap,
+                        gamma=0.8,
+                        metadata=new_metadata,
+                    ),
+                )
 
                 image_layer = getattr(self, layer_name)
-                image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                image_layer.mouse_drag_callbacks.append(
+                    self._segmentationEvents
+                )
+                image_layer.mouse_double_click_callbacks.append(
+                    self._doubeClickEvents
+                )
 
                 self.segLayer.data = new_mask_stack
                 self.classLayer.data = new_class_stack
                 self.segLayer.metadata = new_metadata
 
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Classes", "center_lines"]]
-
-        # ensures segmentation and classes is in correct order in the viewer
-        for layer in layer_names:
-            self.viewer.layers[layer].selected = False
-            layer_index = self.viewer.layers.index(layer)
-            self.viewer.layers.move(layer_index, 0)
-
         # sets labels such that only label contours are shown
         self.segLayer.contour = 1
         self.segLayer.opacity = 1
 
+        self._reorderLayers()
         self._updateFileName()
         self._updateSegmentationCombo()
         self._updateSegChannels()
         self.import_progressbar.reset()
         self.viewer.reset_view()
         self._autoClassify()
         align_image_channels(self)
         self._autoContrast()
+        self._updateScaleBar()
+
+    def _reorderLayers(self):
+        try:
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name in ["Segmentations", "Classes", "center_lines"]
+            ]
+
+            for layer in ["center_lines", "Classes", "Segmentations"]:
+                if layer in layer_names:
+                    layer_index = self.viewer.layers.index(layer)
+                    self.viewer.layers.move(layer_index, -1)
+
+        except:
+            pass
 
     def _autoClassify(self, reset=False):
         mask_stack = self.segLayer.data.copy()
         label_stack = self.classLayer.data.copy()
 
         for i in range(len(mask_stack)):
             mask = mask_stack[i, :, :]
@@ -1384,21 +2376,30 @@
                 label = np.zeros(label.shape, dtype=np.uint16)
 
                 for mask_id in mask_ids:
                     if mask_id != 0:
                         cnt_mask = np.zeros(label.shape, dtype=np.uint8)
                         cnt_mask[mask == mask_id] = 255
 
-                        cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
+                        cnt, _ = cv2.findContours(
+                            cnt_mask.astype(np.uint8),
+                            cv2.RETR_EXTERNAL,
+                            cv2.CHAIN_APPROX_NONE,
+                        )
 
                         x, y, w, h = cv2.boundingRect(cnt[0])
                         y1, y2, x1, x2 = y, (y + h), x, (x + w)
 
                         # appends contour to list if the bounding coordinates are along the edge of the image
-                        if (y1 > 0 and y2 < cnt_mask.shape[0] and x1 > 0 and x2 < cnt_mask.shape[1]):
+                        if (
+                            y1 > 0
+                            and y2 < cnt_mask.shape[0]
+                            and x1 > 0
+                            and x2 < cnt_mask.shape[1]
+                        ):
                             label[mask == mask_id] = 1
 
                         else:
                             label[mask == mask_id] = 6
 
             label_stack[i, :, :] = label
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/bacseg_ui.py` & `napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_tab_widget(object):
     def setupUi(self, tab_widget):
         tab_widget.setObjectName("tab_widget")
         tab_widget.setEnabled(True)
-        tab_widget.resize(681, 1011)
+        tab_widget.resize(681, 1133)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(100)
         sizePolicy.setHeightForWidth(tab_widget.sizePolicy().hasHeightForWidth())
         tab_widget.setSizePolicy(sizePolicy)
         tab_widget.setMinimumSize(QtCore.QSize(200, 0))
         tab_widget.setMaximumSize(QtCore.QSize(1000, 16777215))
@@ -44,28 +44,14 @@
         font.setBold(True)
         font.setWeight(75)
         self.label_37.setFont(font)
         self.label_37.setObjectName("label_37")
         self.verticalLayout.addWidget(self.label_37)
         self.formLayout_8 = QtWidgets.QFormLayout()
         self.formLayout_8.setObjectName("formLayout_8")
-        self.label_27 = QtWidgets.QLabel(self.import_tab)
-        self.label_27.setObjectName("label_27")
-        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_27)
-        self.import_mode = QtWidgets.QComboBox(self.import_tab)
-        self.import_mode.setObjectName("import_mode")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.import_mode.addItem("")
-        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.import_mode)
         spacerItem = QtWidgets.QSpacerItem(334, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.formLayout_8.setItem(2, QtWidgets.QFormLayout.FieldRole, spacerItem)
         self.label_51 = QtWidgets.QLabel(self.import_tab)
         self.label_51.setObjectName("label_51")
         self.formLayout_8.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_51)
         self.import_filemode = QtWidgets.QComboBox(self.import_tab)
         self.import_filemode.setObjectName("import_filemode")
@@ -113,14 +99,28 @@
         self.import_precision = QtWidgets.QComboBox(self.import_tab)
         self.import_precision.setObjectName("import_precision")
         self.import_precision.addItem("")
         self.import_precision.addItem("")
         self.import_precision.addItem("")
         self.import_precision.addItem("")
         self.formLayout_8.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.import_precision)
+        self.import_mode = QtWidgets.QComboBox(self.import_tab)
+        self.import_mode.setObjectName("import_mode")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.import_mode.addItem("")
+        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_mode)
+        self.label_27 = QtWidgets.QLabel(self.import_tab)
+        self.label_27.setObjectName("label_27")
+        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_27)
         self.verticalLayout.addLayout(self.formLayout_8)
         spacerItem2 = QtWidgets.QSpacerItem(334, 5, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.verticalLayout.addItem(spacerItem2)
         self.gridLayout_9 = QtWidgets.QGridLayout()
         self.gridLayout_9.setObjectName("gridLayout_9")
         self.import_clear_previous = QtWidgets.QCheckBox(self.import_tab)
         self.import_clear_previous.setChecked(True)
@@ -149,166 +149,263 @@
         spacerItem4 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout.addItem(spacerItem4)
         tab_widget.addTab(self.import_tab, "")
         self.tab = QtWidgets.QWidget()
         self.tab.setObjectName("tab")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.tab)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
-        self.line_27 = QtWidgets.QFrame(self.tab)
-        self.line_27.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line_27.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_27.setObjectName("line_27")
-        self.verticalLayout_5.addWidget(self.line_27)
-        self.label_60 = QtWidgets.QLabel(self.tab)
+        self.tabWidget = QtWidgets.QTabWidget(self.tab)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.tabWidget.sizePolicy().hasHeightForWidth())
+        self.tabWidget.setSizePolicy(sizePolicy)
+        self.tabWidget.setObjectName("tabWidget")
+        self.tab_16 = QtWidgets.QWidget()
+        self.tab_16.setObjectName("tab_16")
+        self.verticalLayout_23 = QtWidgets.QVBoxLayout(self.tab_16)
+        self.verticalLayout_23.setObjectName("verticalLayout_23")
+        self.label_60 = QtWidgets.QLabel(self.tab_16)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_60.setFont(font)
         self.label_60.setObjectName("label_60")
-        self.verticalLayout_5.addWidget(self.label_60)
-        self.import_auto_contrast = QtWidgets.QCheckBox(self.tab)
+        self.verticalLayout_23.addWidget(self.label_60)
+        self.import_auto_contrast = QtWidgets.QCheckBox(self.tab_16)
         self.import_auto_contrast.setChecked(True)
         self.import_auto_contrast.setObjectName("import_auto_contrast")
-        self.verticalLayout_5.addWidget(self.import_auto_contrast)
-        spacerItem5 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_5.addItem(spacerItem5)
-        self.line_26 = QtWidgets.QFrame(self.tab)
-        self.line_26.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line_26.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_26.setObjectName("line_26")
-        self.verticalLayout_5.addWidget(self.line_26)
-        self.label_38 = QtWidgets.QLabel(self.tab)
+        self.verticalLayout_23.addWidget(self.import_auto_contrast)
+        spacerItem5 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_23.addItem(spacerItem5)
+        self.line_29 = QtWidgets.QFrame(self.tab_16)
+        self.line_29.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_29.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_29.setObjectName("line_29")
+        self.verticalLayout_23.addWidget(self.line_29)
+        self.label_38 = QtWidgets.QLabel(self.tab_16)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_38.setFont(font)
         self.label_38.setObjectName("label_38")
-        self.verticalLayout_5.addWidget(self.label_38)
+        self.verticalLayout_23.addWidget(self.label_38)
         self.gridLayout_6 = QtWidgets.QGridLayout()
         self.gridLayout_6.setObjectName("gridLayout_6")
-        self.modify_viewlabels = QtWidgets.QCheckBox(self.tab)
+        self.modify_viewlabels = QtWidgets.QCheckBox(self.tab_16)
         self.modify_viewlabels.setObjectName("modify_viewlabels")
         self.gridLayout_6.addWidget(self.modify_viewlabels, 1, 1, 1, 1)
-        self.modify_viewmasks = QtWidgets.QCheckBox(self.tab)
+        self.modify_viewmasks = QtWidgets.QCheckBox(self.tab_16)
         self.modify_viewmasks.setObjectName("modify_viewmasks")
         self.gridLayout_6.addWidget(self.modify_viewmasks, 1, 0, 1, 1)
-        self.verticalLayout_5.addLayout(self.gridLayout_6)
-        spacerItem6 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_5.addItem(spacerItem6)
-        self.line_17 = QtWidgets.QFrame(self.tab)
-        self.line_17.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line_17.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_17.setObjectName("line_17")
-        self.verticalLayout_5.addWidget(self.line_17)
-        self.label_56 = QtWidgets.QLabel(self.tab)
+        self.verticalLayout_23.addLayout(self.gridLayout_6)
+        spacerItem6 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_23.addItem(spacerItem6)
+        self.tabWidget.addTab(self.tab_16, "")
+        self.tab_7 = QtWidgets.QWidget()
+        self.tab_7.setObjectName("tab_7")
+        self.verticalLayout_21 = QtWidgets.QVBoxLayout(self.tab_7)
+        self.verticalLayout_21.setObjectName("verticalLayout_21")
+        self.line_26 = QtWidgets.QFrame(self.tab_7)
+        self.line_26.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_26.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_26.setObjectName("line_26")
+        self.verticalLayout_21.addWidget(self.line_26)
+        self.label_47 = QtWidgets.QLabel(self.tab_7)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
-        self.label_56.setFont(font)
-        self.label_56.setObjectName("label_56")
-        self.verticalLayout_5.addWidget(self.label_56)
-        self.gridLayout_7 = QtWidgets.QGridLayout()
-        self.gridLayout_7.setObjectName("gridLayout_7")
-        self.find_previous = QtWidgets.QPushButton(self.tab)
-        self.find_previous.setObjectName("find_previous")
-        self.gridLayout_7.addWidget(self.find_previous, 1, 1, 1, 1)
-        self.find_mode = QtWidgets.QComboBox(self.tab)
-        self.find_mode.setObjectName("find_mode")
-        self.find_mode.addItem("")
-        self.find_mode.addItem("")
-        self.gridLayout_7.addWidget(self.find_mode, 0, 1, 1, 1)
-        self.find_next = QtWidgets.QPushButton(self.tab)
-        self.find_next.setObjectName("find_next")
-        self.gridLayout_7.addWidget(self.find_next, 1, 0, 1, 1)
-        self.find_criterion = QtWidgets.QComboBox(self.tab)
-        self.find_criterion.setObjectName("find_criterion")
-        self.find_criterion.addItem("")
-        self.find_criterion.addItem("")
-        self.find_criterion.addItem("")
-        self.gridLayout_7.addWidget(self.find_criterion, 0, 0, 1, 1)
-        self.verticalLayout_5.addLayout(self.gridLayout_7)
-        spacerItem7 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_5.addItem(spacerItem7)
-        self.line_25 = QtWidgets.QFrame(self.tab)
-        self.line_25.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line_25.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_25.setObjectName("line_25")
-        self.verticalLayout_5.addWidget(self.line_25)
-        self.label_57 = QtWidgets.QLabel(self.tab)
+        self.label_47.setFont(font)
+        self.label_47.setObjectName("label_47")
+        self.verticalLayout_21.addWidget(self.label_47)
+        self.scalebar_show = QtWidgets.QCheckBox(self.tab_7)
+        self.scalebar_show.setObjectName("scalebar_show")
+        self.verticalLayout_21.addWidget(self.scalebar_show)
+        self.gridLayout_20 = QtWidgets.QGridLayout()
+        self.gridLayout_20.setObjectName("gridLayout_20")
+        self.scalebar_resolution = QtWidgets.QLineEdit(self.tab_7)
+        self.scalebar_resolution.setMaximumSize(QtCore.QSize(200, 16777215))
+        self.scalebar_resolution.setObjectName("scalebar_resolution")
+        self.gridLayout_20.addWidget(self.scalebar_resolution, 0, 1, 1, 1)
+        self.scalebar_units = QtWidgets.QComboBox(self.tab_7)
+        self.scalebar_units.setMaximumSize(QtCore.QSize(200, 100))
+        self.scalebar_units.setObjectName("scalebar_units")
+        self.scalebar_units.addItem("")
+        self.scalebar_units.addItem("")
+        self.gridLayout_20.addWidget(self.scalebar_units, 0, 2, 1, 1)
+        self.label_48 = QtWidgets.QLabel(self.tab_7)
+        self.label_48.setObjectName("label_48")
+        self.gridLayout_20.addWidget(self.label_48, 0, 0, 1, 1)
+        self.verticalLayout_21.addLayout(self.gridLayout_20)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_21.addItem(spacerItem7)
+        self.tabWidget.addTab(self.tab_7, "")
+        self.tab_15 = QtWidgets.QWidget()
+        self.tab_15.setObjectName("tab_15")
+        self.verticalLayout_22 = QtWidgets.QVBoxLayout(self.tab_15)
+        self.verticalLayout_22.setObjectName("verticalLayout_22")
+        self.line_27 = QtWidgets.QFrame(self.tab_15)
+        self.line_27.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_27.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_27.setObjectName("line_27")
+        self.verticalLayout_22.addWidget(self.line_27)
+        self.label_73 = QtWidgets.QLabel(self.tab_15)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_73.setFont(font)
+        self.label_73.setObjectName("label_73")
+        self.verticalLayout_22.addWidget(self.label_73)
+        self.gridLayout_28 = QtWidgets.QGridLayout()
+        self.gridLayout_28.setObjectName("gridLayout_28")
+        self.overlay_filename = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_filename.setChecked(True)
+        self.overlay_filename.setObjectName("overlay_filename")
+        self.gridLayout_28.addWidget(self.overlay_filename, 0, 0, 1, 1)
+        self.overlay_folder = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_folder.setObjectName("overlay_folder")
+        self.gridLayout_28.addWidget(self.overlay_folder, 0, 1, 1, 1)
+        self.overlay_antibiotic = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_antibiotic.setObjectName("overlay_antibiotic")
+        self.gridLayout_28.addWidget(self.overlay_antibiotic, 2, 4, 1, 1)
+        self.overlay_phenotype = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_phenotype.setObjectName("overlay_phenotype")
+        self.gridLayout_28.addWidget(self.overlay_phenotype, 2, 3, 1, 1)
+        self.overlay_strain = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_strain.setObjectName("overlay_strain")
+        self.gridLayout_28.addWidget(self.overlay_strain, 2, 1, 1, 1)
+        self.overlay_content = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_content.setObjectName("overlay_content")
+        self.gridLayout_28.addWidget(self.overlay_content, 2, 0, 1, 1)
+        self.overlay_microscope = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_microscope.setObjectName("overlay_microscope")
+        self.gridLayout_28.addWidget(self.overlay_microscope, 0, 3, 1, 1)
+        self.overlay_datemodified = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_datemodified.setObjectName("overlay_datemodified")
+        self.gridLayout_28.addWidget(self.overlay_datemodified, 0, 4, 1, 1)
+        self.verticalLayout_22.addLayout(self.gridLayout_28)
+        self.gridLayout_29 = QtWidgets.QGridLayout()
+        self.gridLayout_29.setObjectName("gridLayout_29")
+        self.overlay_lightsource = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_lightsource.setObjectName("overlay_lightsource")
+        self.gridLayout_29.addWidget(self.overlay_lightsource, 0, 3, 1, 1)
+        self.overlay_staintarget = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_staintarget.setObjectName("overlay_staintarget")
+        self.gridLayout_29.addWidget(self.overlay_staintarget, 0, 1, 1, 1)
+        self.overlay_modality = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_modality.setObjectName("overlay_modality")
+        self.gridLayout_29.addWidget(self.overlay_modality, 0, 2, 1, 1)
+        self.overlay_stain = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_stain.setObjectName("overlay_stain")
+        self.gridLayout_29.addWidget(self.overlay_stain, 0, 0, 1, 1)
+        self.verticalLayout_22.addLayout(self.gridLayout_29)
+        self.gridLayout_30 = QtWidgets.QGridLayout()
+        self.gridLayout_30.setObjectName("gridLayout_30")
+        self.overlay_focus = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_focus.setObjectName("overlay_focus")
+        self.gridLayout_30.addWidget(self.overlay_focus, 0, 0, 1, 1)
+        self.overlay_laplacian = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_laplacian.setObjectName("overlay_laplacian")
+        self.gridLayout_30.addWidget(self.overlay_laplacian, 0, 2, 1, 1)
+        self.overlay_debris = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_debris.setObjectName("overlay_debris")
+        self.gridLayout_30.addWidget(self.overlay_debris, 0, 1, 1, 1)
+        self.overlay_range = QtWidgets.QCheckBox(self.tab_15)
+        self.overlay_range.setObjectName("overlay_range")
+        self.gridLayout_30.addWidget(self.overlay_range, 0, 3, 1, 1)
+        self.verticalLayout_22.addLayout(self.gridLayout_30)
+        spacerItem8 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_22.addItem(spacerItem8)
+        self.tabWidget.addTab(self.tab_15, "")
+        self.tab_17 = QtWidgets.QWidget()
+        self.tab_17.setObjectName("tab_17")
+        self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.tab_17)
+        self.verticalLayout_24.setObjectName("verticalLayout_24")
+        self.line_28 = QtWidgets.QFrame(self.tab_17)
+        self.line_28.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_28.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_28.setObjectName("line_28")
+        self.verticalLayout_24.addWidget(self.line_28)
+        self.label_57 = QtWidgets.QLabel(self.tab_17)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_57.setFont(font)
         self.label_57.setObjectName("label_57")
-        self.verticalLayout_5.addWidget(self.label_57)
+        self.verticalLayout_24.addWidget(self.label_57)
         self.gridLayout_8 = QtWidgets.QGridLayout()
         self.gridLayout_8.setObjectName("gridLayout_8")
-        self.unfold = QtWidgets.QPushButton(self.tab)
+        self.unfold = QtWidgets.QPushButton(self.tab_17)
         self.unfold.setObjectName("unfold")
         self.gridLayout_8.addWidget(self.unfold, 0, 0, 1, 1)
-        self.fold = QtWidgets.QPushButton(self.tab)
+        self.fold = QtWidgets.QPushButton(self.tab_17)
         self.fold.setObjectName("fold")
         self.gridLayout_8.addWidget(self.fold, 0, 1, 1, 1)
-        self.verticalLayout_5.addLayout(self.gridLayout_8)
+        self.verticalLayout_24.addLayout(self.gridLayout_8)
         self.formLayout_3 = QtWidgets.QFormLayout()
         self.formLayout_3.setObjectName("formLayout_3")
-        self.label_58 = QtWidgets.QLabel(self.tab)
+        self.label_58 = QtWidgets.QLabel(self.tab_17)
         self.label_58.setObjectName("label_58")
         self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_58)
-        self.unfold_tile_size = QtWidgets.QComboBox(self.tab)
+        self.unfold_tile_size = QtWidgets.QComboBox(self.tab_17)
         self.unfold_tile_size.setEditable(True)
         self.unfold_tile_size.setObjectName("unfold_tile_size")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.unfold_tile_size.addItem("")
         self.formLayout_3.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.unfold_tile_size)
-        self.label_59 = QtWidgets.QLabel(self.tab)
+        self.label_59 = QtWidgets.QLabel(self.tab_17)
         self.label_59.setObjectName("label_59")
         self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_59)
-        self.unfold_tile_overlap = QtWidgets.QComboBox(self.tab)
+        self.unfold_tile_overlap = QtWidgets.QComboBox(self.tab_17)
         self.unfold_tile_overlap.setEditable(True)
         self.unfold_tile_overlap.setObjectName("unfold_tile_overlap")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.unfold_tile_overlap.addItem("")
         self.formLayout_3.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.unfold_tile_overlap)
-        self.label_62 = QtWidgets.QLabel(self.tab)
+        self.label_62 = QtWidgets.QLabel(self.tab_17)
         self.label_62.setObjectName("label_62")
         self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_62)
-        self.unfold_mode = QtWidgets.QComboBox(self.tab)
+        self.unfold_mode = QtWidgets.QComboBox(self.tab_17)
         self.unfold_mode.setObjectName("unfold_mode")
         self.unfold_mode.addItem("")
         self.unfold_mode.addItem("")
         self.formLayout_3.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.unfold_mode)
-        self.verticalLayout_5.addLayout(self.formLayout_3)
-        spacerItem8 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_5.addItem(spacerItem8)
+        self.verticalLayout_24.addLayout(self.formLayout_3)
+        spacerItem9 = QtWidgets.QSpacerItem(20, 1, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_24.addItem(spacerItem9)
+        self.tabWidget.addTab(self.tab_17, "")
+        self.verticalLayout_5.addWidget(self.tabWidget)
+        spacerItem10 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem10)
         tab_widget.addTab(self.tab, "")
         self.segement_tab = QtWidgets.QWidget()
         self.segement_tab.setObjectName("segement_tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.segement_tab)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.line_12 = QtWidgets.QFrame(self.segement_tab)
         self.line_12.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_12.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_12.setObjectName("line_12")
         self.verticalLayout_2.addWidget(self.line_12)
         self.cellpose_select_custom_model = QtWidgets.QPushButton(self.segement_tab)
         self.cellpose_select_custom_model.setObjectName("cellpose_select_custom_model")
         self.verticalLayout_2.addWidget(self.cellpose_select_custom_model)
-        spacerItem9 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_2.addItem(spacerItem9)
+        spacerItem11 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_2.addItem(spacerItem11)
         self.tabWidget_3 = QtWidgets.QTabWidget(self.segement_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabWidget_3.sizePolicy().hasHeightForWidth())
         self.tabWidget_3.setSizePolicy(sizePolicy)
         self.tabWidget_3.setObjectName("tabWidget_3")
@@ -334,24 +431,24 @@
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.cellpose_segmodel.addItem("")
         self.formLayout_12.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_segmodel)
         self.verticalLayout_10.addLayout(self.formLayout_12)
-        spacerItem10 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_10.addItem(spacerItem10)
+        spacerItem12 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_10.addItem(spacerItem12)
         self.cellpose_segment_active = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_active.setObjectName("cellpose_segment_active")
         self.verticalLayout_10.addWidget(self.cellpose_segment_active)
         self.cellpose_segment_all = QtWidgets.QPushButton(self.tab_6)
         self.cellpose_segment_all.setObjectName("cellpose_segment_all")
         self.verticalLayout_10.addWidget(self.cellpose_segment_all)
-        spacerItem11 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_10.addItem(spacerItem11)
+        spacerItem13 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_10.addItem(spacerItem13)
         self.formLayout_13 = QtWidgets.QFormLayout()
         self.formLayout_13.setObjectName("formLayout_13")
         self.cellpose_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.cellpose_progressbar.setMaximumSize(QtCore.QSize(16777215, 20))
         self.cellpose_progressbar.setProperty("value", 0)
         self.cellpose_progressbar.setObjectName("cellpose_progressbar")
         self.formLayout_13.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.cellpose_progressbar)
@@ -409,16 +506,16 @@
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.cellpose_trainmodel.addItem("")
         self.formLayout_15.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.cellpose_trainmodel)
         self.verticalLayout_13.addLayout(self.formLayout_15)
-        spacerItem12 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_13.addItem(spacerItem12)
+        spacerItem14 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_13.addItem(spacerItem14)
         self.cellpose_save_dir = QtWidgets.QPushButton(self.tab_11)
         self.cellpose_save_dir.setObjectName("cellpose_save_dir")
         self.verticalLayout_13.addWidget(self.cellpose_save_dir)
         self.cellpose_train_model = QtWidgets.QPushButton(self.tab_11)
         self.cellpose_train_model.setObjectName("cellpose_train_model")
         self.verticalLayout_13.addWidget(self.cellpose_train_model)
         self.tabWidget_3.addTab(self.tab_11, "")
@@ -484,16 +581,16 @@
         self.label_4 = QtWidgets.QLabel(self.tab_12)
         self.label_4.setObjectName("label_4")
         self.gridLayout_2.addWidget(self.label_4, 3, 0, 1, 1)
         self.cellpose_diameter_label = QtWidgets.QLabel(self.tab_12)
         self.cellpose_diameter_label.setObjectName("cellpose_diameter_label")
         self.gridLayout_2.addWidget(self.cellpose_diameter_label, 3, 2, 1, 1)
         self.verticalLayout_14.addLayout(self.gridLayout_2)
-        spacerItem13 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_14.addItem(spacerItem13)
+        spacerItem15 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_14.addItem(spacerItem15)
         self.cellpose_clear_previous = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_clear_previous.setChecked(True)
         self.cellpose_clear_previous.setObjectName("cellpose_clear_previous")
         self.verticalLayout_14.addWidget(self.cellpose_clear_previous)
         self.cellpose_usegpu = QtWidgets.QCheckBox(self.tab_12)
         self.cellpose_usegpu.setChecked(True)
         self.cellpose_usegpu.setObjectName("cellpose_usegpu")
@@ -505,16 +602,16 @@
         self.tabWidget_3.addTab(self.tab_12, "")
         self.verticalLayout_2.addWidget(self.tabWidget_3)
         self.line_6 = QtWidgets.QFrame(self.segement_tab)
         self.line_6.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_6.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_6.setObjectName("line_6")
         self.verticalLayout_2.addWidget(self.line_6)
-        spacerItem14 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_2.addItem(spacerItem14)
+        spacerItem16 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_2.addItem(spacerItem16)
         tab_widget.addTab(self.segement_tab, "")
         self.tab_3 = QtWidgets.QWidget()
         self.tab_3.setEnabled(True)
         self.tab_3.setObjectName("tab_3")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_3)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.line_4 = QtWidgets.QFrame(self.tab_3)
@@ -542,16 +639,16 @@
         self.modify_segment.setObjectName("modify_segment")
         self.gridLayout_3.addWidget(self.modify_segment, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_3)
         self.modify_auto_panzoom = QtWidgets.QCheckBox(self.tab_3)
         self.modify_auto_panzoom.setChecked(True)
         self.modify_auto_panzoom.setObjectName("modify_auto_panzoom")
         self.verticalLayout_3.addWidget(self.modify_auto_panzoom)
-        spacerItem15 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem15)
+        spacerItem17 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem17)
         self.line_18 = QtWidgets.QFrame(self.tab_3)
         self.line_18.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_18.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_18.setObjectName("line_18")
         self.verticalLayout_3.addWidget(self.line_18)
         self.label_16 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -578,16 +675,16 @@
         self.modify_split = QtWidgets.QPushButton(self.tab_3)
         self.modify_split.setObjectName("modify_split")
         self.gridLayout_4.addWidget(self.modify_split, 1, 0, 1, 1)
         self.modify_extend = QtWidgets.QPushButton(self.tab_3)
         self.modify_extend.setObjectName("modify_extend")
         self.gridLayout_4.addWidget(self.modify_extend, 0, 1, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_4)
-        spacerItem16 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem16)
+        spacerItem18 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem18)
         self.line_19 = QtWidgets.QFrame(self.tab_3)
         self.line_19.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_19.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_19.setObjectName("line_19")
         self.verticalLayout_3.addWidget(self.line_19)
         self.label_28 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -621,16 +718,16 @@
         self.classify_broken.setObjectName("classify_broken")
         self.gridLayout_5.addWidget(self.classify_broken, 1, 1, 1, 1)
         self.classify_single = QtWidgets.QPushButton(self.tab_3)
         self.classify_single.setStyleSheet("color: rgb(255, 255, 255);")
         self.classify_single.setObjectName("classify_single")
         self.gridLayout_5.addWidget(self.classify_single, 0, 0, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_5)
-        spacerItem17 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_3.addItem(spacerItem17)
+        spacerItem19 = QtWidgets.QSpacerItem(334, 14, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_3.addItem(spacerItem19)
         self.line_21 = QtWidgets.QFrame(self.tab_3)
         self.line_21.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_21.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_21.setObjectName("line_21")
         self.verticalLayout_3.addWidget(self.line_21)
         self.label_14 = QtWidgets.QLabel(self.tab_3)
         font = QtGui.QFont()
@@ -713,16 +810,16 @@
         self.set_debris_4 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_4.setObjectName("set_debris_4")
         self.gridLayout_22.addWidget(self.set_debris_4, 0, 4, 1, 1)
         self.set_debris_5 = QtWidgets.QPushButton(self.tab_3)
         self.set_debris_5.setObjectName("set_debris_5")
         self.gridLayout_22.addWidget(self.set_debris_5, 0, 5, 1, 1)
         self.verticalLayout_3.addLayout(self.gridLayout_22)
-        spacerItem18 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem18)
+        spacerItem20 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem20)
         tab_widget.addTab(self.tab_3, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.label_29 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
@@ -737,16 +834,16 @@
         self.oufti_panzoom_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_panzoom_mode.setObjectName("oufti_panzoom_mode")
         self.gridLayout_10.addWidget(self.oufti_panzoom_mode, 0, 0, 1, 1)
         self.oufti_edit_mode = QtWidgets.QRadioButton(self.tab_2)
         self.oufti_edit_mode.setObjectName("oufti_edit_mode")
         self.gridLayout_10.addWidget(self.oufti_edit_mode, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_10)
-        spacerItem19 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem19)
+        spacerItem21 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem21)
         self.label_20 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_20.setFont(font)
         self.label_20.setObjectName("label_20")
@@ -774,16 +871,16 @@
         self.gridLayout_17 = QtWidgets.QGridLayout()
         self.gridLayout_17.setObjectName("gridLayout_17")
         self.oufti_generate_all_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_generate_all_midlines.setObjectName("oufti_generate_all_midlines")
         self.gridLayout_17.addWidget(self.oufti_generate_all_midlines, 0, 0, 1, 1)
         self.gridLayout_16.addLayout(self.gridLayout_17, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_16)
-        spacerItem20 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem20)
+        spacerItem22 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem22)
         self.label_63 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_63.setFont(font)
         self.label_63.setObjectName("label_63")
@@ -793,16 +890,16 @@
         self.oufti_centre_active_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_centre_active_midlines.setObjectName("oufti_centre_active_midlines")
         self.gridLayout_15.addWidget(self.oufti_centre_active_midlines, 0, 0, 1, 1)
         self.oufti_centre_all_midlines = QtWidgets.QPushButton(self.tab_2)
         self.oufti_centre_all_midlines.setObjectName("oufti_centre_all_midlines")
         self.gridLayout_15.addWidget(self.oufti_centre_all_midlines, 0, 1, 1, 1)
         self.verticalLayout_7.addLayout(self.gridLayout_15)
-        spacerItem21 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_7.addItem(spacerItem21)
+        spacerItem23 = QtWidgets.QSpacerItem(360, 13, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem23)
         self.label_61 = QtWidgets.QLabel(self.tab_2)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_61.setFont(font)
         self.label_61.setObjectName("label_61")
@@ -838,16 +935,16 @@
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.oufti_mesh_dilation.addItem("")
         self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.oufti_mesh_dilation)
         self.verticalLayout_7.addLayout(self.formLayout_7)
-        spacerItem22 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_7.addItem(spacerItem22)
+        spacerItem24 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_7.addItem(spacerItem24)
         tab_widget.addTab(self.tab_2, "")
         self.upload_tab = QtWidgets.QWidget()
         self.upload_tab.setEnabled(True)
         self.upload_tab.setObjectName("upload_tab")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.upload_tab)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.line_24 = QtWidgets.QFrame(self.upload_tab)
@@ -880,16 +977,16 @@
         self.display_database_path = QtWidgets.QLineEdit(self.upload_tab)
         self.display_database_path.setAlignment(QtCore.Qt.AlignCenter)
         self.display_database_path.setReadOnly(True)
         self.display_database_path.setClearButtonEnabled(False)
         self.display_database_path.setObjectName("display_database_path")
         self.formLayout_9.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.display_database_path)
         self.verticalLayout_4.addLayout(self.formLayout_9)
-        spacerItem23 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem23)
+        spacerItem25 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem25)
         self.metadata_controls = QtWidgets.QTabWidget(self.upload_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.metadata_controls.sizePolicy().hasHeightForWidth())
         self.metadata_controls.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
@@ -932,60 +1029,83 @@
         self.upload_microscope.setStyleSheet("background-color: rgb(191, 0, 0);")
         self.upload_microscope.setEditable(True)
         self.upload_microscope.setObjectName("upload_microscope")
         self.upload_microscope.addItem("")
         self.image_metadata_controls.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.upload_microscope)
         self.label_76 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_76.setObjectName("label_76")
-        self.image_metadata_controls.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_76)
+        self.image_metadata_controls.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_76)
         self.upload_antibiotic = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_antibiotic.setEnabled(True)
         self.upload_antibiotic.setEditable(True)
         self.upload_antibiotic.setObjectName("upload_antibiotic")
-        self.image_metadata_controls.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.upload_antibiotic)
+        self.image_metadata_controls.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_antibiotic)
         self.label_77 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_77.setObjectName("label_77")
-        self.image_metadata_controls.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_77)
+        self.image_metadata_controls.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_77)
         self.upload_treatmenttime = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_treatmenttime.setEnabled(True)
         self.upload_treatmenttime.setEditable(True)
         self.upload_treatmenttime.setObjectName("upload_treatmenttime")
         self.upload_treatmenttime.addItem("")
         self.upload_treatmenttime.setItemText(0, "")
-        self.image_metadata_controls.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_treatmenttime)
+        self.image_metadata_controls.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.upload_treatmenttime)
         self.label_78 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_78.setObjectName("label_78")
-        self.image_metadata_controls.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_78)
+        self.image_metadata_controls.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_78)
         self.upload_abxconcentration = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_abxconcentration.setEnabled(True)
         self.upload_abxconcentration.setEditable(True)
         self.upload_abxconcentration.setObjectName("upload_abxconcentration")
-        self.image_metadata_controls.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.upload_abxconcentration)
+        self.image_metadata_controls.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.upload_abxconcentration)
         self.label_79 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_79.setObjectName("label_79")
-        self.image_metadata_controls.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_79)
+        self.image_metadata_controls.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_79)
         self.upload_mount = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_mount.setEnabled(True)
         self.upload_mount.setEditable(True)
         self.upload_mount.setObjectName("upload_mount")
         self.upload_mount.addItem("")
         self.upload_mount.setItemText(0, "")
         self.upload_mount.addItem("")
         self.upload_mount.addItem("")
-        self.image_metadata_controls.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.upload_mount)
+        self.image_metadata_controls.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.upload_mount)
         self.label_80 = QtWidgets.QLabel(self.experiment_metadata)
         self.label_80.setObjectName("label_80")
-        self.image_metadata_controls.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_80)
+        self.image_metadata_controls.setWidget(9, QtWidgets.QFormLayout.LabelRole, self.label_80)
         self.upload_protocol = QtWidgets.QComboBox(self.experiment_metadata)
         self.upload_protocol.setEnabled(True)
         self.upload_protocol.setEditable(True)
         self.upload_protocol.setObjectName("upload_protocol")
         self.upload_protocol.addItem("")
         self.upload_protocol.setItemText(0, "")
-        self.image_metadata_controls.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.upload_protocol)
+        self.image_metadata_controls.setWidget(9, QtWidgets.QFormLayout.FieldRole, self.upload_protocol)
+        self.upload_phenotype = QtWidgets.QComboBox(self.experiment_metadata)
+        self.upload_phenotype.setEditable(True)
+        self.upload_phenotype.setObjectName("upload_phenotype")
+        self.upload_phenotype.addItem("")
+        self.upload_phenotype.setItemText(0, "")
+        self.upload_phenotype.addItem("")
+        self.upload_phenotype.addItem("")
+        self.upload_phenotype.addItem("")
+        self.upload_phenotype.addItem("")
+        self.image_metadata_controls.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.upload_phenotype)
+        self.label_41 = QtWidgets.QLabel(self.experiment_metadata)
+        self.label_41.setObjectName("label_41")
+        self.image_metadata_controls.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_41)
+        self.label_42 = QtWidgets.QLabel(self.experiment_metadata)
+        self.label_42.setObjectName("label_42")
+        self.image_metadata_controls.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_42)
+        self.upload_strain = QtWidgets.QComboBox(self.experiment_metadata)
+        self.upload_strain.setEditable(True)
+        self.upload_strain.setObjectName("upload_strain")
+        self.upload_strain.addItem("")
+        self.upload_strain.setItemText(0, "")
+        self.upload_strain.addItem("")
+        self.image_metadata_controls.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.upload_strain)
         self.verticalLayout_9.addLayout(self.image_metadata_controls)
         self.metadata_controls.addTab(self.experiment_metadata, "")
         self.image_metadata = QtWidgets.QWidget()
         self.image_metadata.setObjectName("image_metadata")
         self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.image_metadata)
         self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.formLayout_10 = QtWidgets.QFormLayout()
@@ -1202,16 +1322,16 @@
         self.label_stain_target.addItem("")
         self.label_stain_target.addItem("")
         self.formLayout_10.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.label_stain_target)
         self.verticalLayout_8.addLayout(self.formLayout_10)
         self.label_overwrite = QtWidgets.QPushButton(self.image_metadata)
         self.label_overwrite.setObjectName("label_overwrite")
         self.verticalLayout_8.addWidget(self.label_overwrite)
-        spacerItem24 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_8.addItem(spacerItem24)
+        spacerItem26 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_8.addItem(spacerItem26)
         self.metadata_controls.addTab(self.image_metadata, "")
         self.user_metadata = QtWidgets.QWidget()
         self.user_metadata.setObjectName("user_metadata")
         self.verticalLayout_19 = QtWidgets.QVBoxLayout(self.user_metadata)
         self.verticalLayout_19.setObjectName("verticalLayout_19")
         self.formLayout_2 = QtWidgets.QFormLayout()
         self.formLayout_2.setObjectName("formLayout_2")
@@ -1260,23 +1380,23 @@
         self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_92)
         self.upload_usermeta6 = QtWidgets.QComboBox(self.user_metadata)
         self.upload_usermeta6.setEnabled(True)
         self.upload_usermeta6.setEditable(True)
         self.upload_usermeta6.setObjectName("upload_usermeta6")
         self.formLayout_2.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.upload_usermeta6)
         self.verticalLayout_19.addLayout(self.formLayout_2)
-        spacerItem25 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_19.addItem(spacerItem25)
+        spacerItem27 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_19.addItem(spacerItem27)
         self.metadata_controls.addTab(self.user_metadata, "")
         self.verticalLayout_4.addWidget(self.metadata_controls)
         self.update_metadata = QtWidgets.QPushButton(self.upload_tab)
         self.update_metadata.setObjectName("update_metadata")
         self.verticalLayout_4.addWidget(self.update_metadata)
-        spacerItem26 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem26)
+        spacerItem28 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem28)
         self.label_87 = QtWidgets.QLabel(self.upload_tab)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_87.setFont(font)
         self.label_87.setObjectName("label_87")
@@ -1302,113 +1422,181 @@
         self.upload_label_combo.addItem("")
         self.upload_label_combo.setItemText(0, "")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.upload_label_combo.addItem("")
         self.formLayout_16.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.upload_label_combo)
         self.verticalLayout_4.addLayout(self.formLayout_16)
-        spacerItem27 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem27)
+        spacerItem29 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_4.addItem(spacerItem29)
         self.tabWidget_2 = QtWidgets.QTabWidget(self.upload_tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabWidget_2.sizePolicy().hasHeightForWidth())
         self.tabWidget_2.setSizePolicy(sizePolicy)
-        self.tabWidget_2.setMaximumSize(QtCore.QSize(16777215, 150))
+        self.tabWidget_2.setMaximumSize(QtCore.QSize(16777215, 500))
         self.tabWidget_2.setObjectName("tabWidget_2")
         self.tab_10 = QtWidgets.QWidget()
         self.tab_10.setObjectName("tab_10")
         self.verticalLayout_12 = QtWidgets.QVBoxLayout(self.tab_10)
         self.verticalLayout_12.setObjectName("verticalLayout_12")
         self.database_download_buttons_2 = QtWidgets.QGridLayout()
         self.database_download_buttons_2.setObjectName("database_download_buttons_2")
-        self.download_sort_order = QtWidgets.QComboBox(self.tab_10)
-        self.download_sort_order.setObjectName("download_sort_order")
-        self.download_sort_order.addItem("")
-        self.download_sort_order.addItem("")
-        self.download_sort_order.addItem("")
-        self.download_sort_order.addItem("")
-        self.download_sort_order.addItem("")
-        self.database_download_buttons_2.addWidget(self.download_sort_order, 0, 1, 1, 1)
+        self.download_sort_order_2 = QtWidgets.QComboBox(self.tab_10)
+        self.download_sort_order_2.setObjectName("download_sort_order_2")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.setItemText(0, "")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.addItem("")
+        self.download_sort_order_2.addItem("")
+        self.database_download_buttons_2.addWidget(self.download_sort_order_2, 1, 1, 1, 1)
         self.label_15 = QtWidgets.QLabel(self.tab_10)
         self.label_15.setObjectName("label_15")
         self.database_download_buttons_2.addWidget(self.label_15, 0, 0, 1, 1)
+        self.download_sort_direction_1 = QtWidgets.QComboBox(self.tab_10)
+        self.download_sort_direction_1.setObjectName("download_sort_direction_1")
+        self.download_sort_direction_1.addItem("")
+        self.download_sort_direction_1.setItemText(0, "")
+        self.download_sort_direction_1.addItem("")
+        self.download_sort_direction_1.addItem("")
+        self.database_download_buttons_2.addWidget(self.download_sort_direction_1, 0, 2, 1, 1)
+        self.download_sort_order_1 = QtWidgets.QComboBox(self.tab_10)
+        self.download_sort_order_1.setObjectName("download_sort_order_1")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.setItemText(0, "")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.addItem("")
+        self.download_sort_order_1.addItem("")
+        self.database_download_buttons_2.addWidget(self.download_sort_order_1, 0, 1, 1, 1)
+        self.label_23 = QtWidgets.QLabel(self.tab_10)
+        self.label_23.setObjectName("label_23")
+        self.database_download_buttons_2.addWidget(self.label_23, 1, 0, 1, 1)
+        self.download_sort_direction_2 = QtWidgets.QComboBox(self.tab_10)
+        self.download_sort_direction_2.setObjectName("download_sort_direction_2")
+        self.download_sort_direction_2.addItem("")
+        self.download_sort_direction_2.setItemText(0, "")
+        self.download_sort_direction_2.addItem("")
+        self.download_sort_direction_2.addItem("")
+        self.database_download_buttons_2.addWidget(self.download_sort_direction_2, 1, 2, 1, 1)
+        self.verticalLayout_12.addLayout(self.database_download_buttons_2)
+        self.gridLayout_23 = QtWidgets.QGridLayout()
+        self.gridLayout_23.setObjectName("gridLayout_23")
         self.label_88 = QtWidgets.QLabel(self.tab_10)
         self.label_88.setObjectName("label_88")
-        self.database_download_buttons_2.addWidget(self.label_88, 1, 0, 1, 1)
+        self.gridLayout_23.addWidget(self.label_88, 0, 0, 1, 1)
         self.database_download_limit = QtWidgets.QComboBox(self.tab_10)
         self.database_download_limit.setEnabled(True)
+        self.database_download_limit.setEditable(True)
         self.database_download_limit.setFrame(True)
         self.database_download_limit.setObjectName("database_download_limit")
         self.database_download_limit.addItem("")
         self.database_download_limit.addItem("")
         self.database_download_limit.addItem("")
         self.database_download_limit.addItem("")
         self.database_download_limit.addItem("")
         self.database_download_limit.addItem("")
         self.database_download_limit.addItem("")
-        self.database_download_buttons_2.addWidget(self.database_download_limit, 1, 1, 1, 1)
-        self.verticalLayout_12.addLayout(self.database_download_buttons_2)
+        self.gridLayout_23.addWidget(self.database_download_limit, 0, 1, 1, 1)
+        self.verticalLayout_12.addLayout(self.gridLayout_23)
         self.database_download = QtWidgets.QPushButton(self.tab_10)
         self.database_download.setEnabled(True)
         self.database_download.setObjectName("database_download")
         self.verticalLayout_12.addWidget(self.database_download)
         self.tabWidget_2.addTab(self.tab_10, "")
         self.tab_4 = QtWidgets.QWidget()
         self.tab_4.setObjectName("tab_4")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.tab_4)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
-        self.database_upload_options_2 = QtWidgets.QGridLayout()
-        self.database_upload_options_2.setObjectName("database_upload_options_2")
-        self.overwrite_all_metadata = QtWidgets.QCheckBox(self.tab_4)
-        self.overwrite_all_metadata.setEnabled(True)
-        self.overwrite_all_metadata.setObjectName("overwrite_all_metadata")
-        self.database_upload_options_2.addWidget(self.overwrite_all_metadata, 1, 1, 1, 1)
-        self.upload_overwrite_images = QtWidgets.QCheckBox(self.tab_4)
-        self.upload_overwrite_images.setEnabled(True)
-        self.upload_overwrite_images.setObjectName("upload_overwrite_images")
-        self.database_upload_options_2.addWidget(self.upload_overwrite_images, 0, 0, 1, 1)
+        self.label_24 = QtWidgets.QLabel(self.tab_4)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_24.setFont(font)
+        self.label_24.setObjectName("label_24")
+        self.verticalLayout_11.addWidget(self.label_24)
+        self.gridLayout_24 = QtWidgets.QGridLayout()
+        self.gridLayout_24.setObjectName("gridLayout_24")
+        self.upload_segmentations_setting = QtWidgets.QCheckBox(self.tab_4)
+        self.upload_segmentations_setting.setChecked(True)
+        self.upload_segmentations_setting.setObjectName("upload_segmentations_setting")
+        self.gridLayout_24.addWidget(self.upload_segmentations_setting, 0, 1, 1, 1)
+        self.upload_images_setting = QtWidgets.QCheckBox(self.tab_4)
+        self.upload_images_setting.setChecked(True)
+        self.upload_images_setting.setObjectName("upload_images_setting")
+        self.gridLayout_24.addWidget(self.upload_images_setting, 0, 0, 1, 1)
+        self.upload_metadata_setting = QtWidgets.QCheckBox(self.tab_4)
+        self.upload_metadata_setting.setChecked(True)
+        self.upload_metadata_setting.setObjectName("upload_metadata_setting")
+        self.gridLayout_24.addWidget(self.upload_metadata_setting, 0, 2, 1, 1)
+        self.verticalLayout_11.addLayout(self.gridLayout_24)
+        self.label_32 = QtWidgets.QLabel(self.tab_4)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_32.setFont(font)
+        self.label_32.setObjectName("label_32")
+        self.verticalLayout_11.addWidget(self.label_32)
+        self.gridLayout_25 = QtWidgets.QGridLayout()
+        self.gridLayout_25.setObjectName("gridLayout_25")
         self.upload_overwrite_masks = QtWidgets.QCheckBox(self.tab_4)
         self.upload_overwrite_masks.setEnabled(True)
         self.upload_overwrite_masks.setObjectName("upload_overwrite_masks")
-        self.database_upload_options_2.addWidget(self.upload_overwrite_masks, 0, 1, 1, 1)
+        self.gridLayout_25.addWidget(self.upload_overwrite_masks, 0, 1, 1, 1)
+        self.upload_overwrite_images = QtWidgets.QCheckBox(self.tab_4)
+        self.upload_overwrite_images.setEnabled(True)
+        self.upload_overwrite_images.setObjectName("upload_overwrite_images")
+        self.gridLayout_25.addWidget(self.upload_overwrite_images, 0, 0, 1, 1)
+        self.overwrite_all_metadata = QtWidgets.QCheckBox(self.tab_4)
+        self.overwrite_all_metadata.setEnabled(True)
+        self.overwrite_all_metadata.setObjectName("overwrite_all_metadata")
+        self.gridLayout_25.addWidget(self.overwrite_all_metadata, 1, 0, 1, 1)
         self.overwrite_selected_metadata = QtWidgets.QCheckBox(self.tab_4)
         self.overwrite_selected_metadata.setEnabled(True)
         self.overwrite_selected_metadata.setObjectName("overwrite_selected_metadata")
-        self.database_upload_options_2.addWidget(self.overwrite_selected_metadata, 1, 0, 1, 1)
-        self.verticalLayout_11.addLayout(self.database_upload_options_2)
+        self.gridLayout_25.addWidget(self.overwrite_selected_metadata, 1, 1, 1, 1)
+        self.verticalLayout_11.addLayout(self.gridLayout_25)
+        spacerItem30 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_11.addItem(spacerItem30)
         self.database_upload_buttons_2 = QtWidgets.QGridLayout()
         self.database_upload_buttons_2.setObjectName("database_upload_buttons_2")
         self.upload_all = QtWidgets.QPushButton(self.tab_4)
         self.upload_all.setEnabled(True)
         self.upload_all.setObjectName("upload_all")
         self.database_upload_buttons_2.addWidget(self.upload_all, 0, 1, 1, 1)
         self.upload_active = QtWidgets.QPushButton(self.tab_4)
         self.upload_active.setEnabled(True)
         self.upload_active.setObjectName("upload_active")
         self.database_upload_buttons_2.addWidget(self.upload_active, 0, 0, 1, 1)
         self.verticalLayout_11.addLayout(self.database_upload_buttons_2)
         self.tabWidget_2.addTab(self.tab_4, "")
         self.verticalLayout_4.addWidget(self.tabWidget_2)
-        spacerItem28 = QtWidgets.QSpacerItem(435, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_4.addItem(spacerItem28)
         self.gridLayout_18 = QtWidgets.QGridLayout()
         self.gridLayout_18.setObjectName("gridLayout_18")
         self.label_89 = QtWidgets.QLabel(self.upload_tab)
         self.label_89.setObjectName("label_89")
         self.gridLayout_18.addWidget(self.label_89, 0, 0, 1, 1)
         self.upload_progressbar = QtWidgets.QProgressBar(self.upload_tab)
         self.upload_progressbar.setEnabled(True)
         self.upload_progressbar.setProperty("value", 0)
         self.upload_progressbar.setObjectName("upload_progressbar")
         self.gridLayout_18.addWidget(self.upload_progressbar, 0, 1, 1, 1)
         self.verticalLayout_4.addLayout(self.gridLayout_18)
-        spacerItem29 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_4.addItem(spacerItem29)
+        spacerItem31 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_4.addItem(spacerItem31)
         tab_widget.addTab(self.upload_tab, "")
         self.export_tab = QtWidgets.QWidget()
         self.export_tab.setEnabled(True)
         self.export_tab.setObjectName("export_tab")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.export_tab)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.tabWidget_4 = QtWidgets.QTabWidget(self.export_tab)
@@ -1470,38 +1658,47 @@
         self.export_overwrite_setting.setObjectName("export_overwrite_setting")
         self.gridLayout_14.addWidget(self.export_overwrite_setting, 1, 1, 1, 1)
         self.export_image_setting = QtWidgets.QCheckBox(self.tab_8)
         self.export_image_setting.setChecked(True)
         self.export_image_setting.setObjectName("export_image_setting")
         self.gridLayout_14.addWidget(self.export_image_setting, 1, 0, 1, 1)
         self.verticalLayout_15.addLayout(self.gridLayout_14)
-        spacerItem30 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_15.addItem(spacerItem30)
+        spacerItem32 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_15.addItem(spacerItem32)
         self.label_12 = QtWidgets.QLabel(self.tab_8)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_12.setFont(font)
         self.label_12.setObjectName("label_12")
         self.verticalLayout_15.addWidget(self.label_12)
         self.gridLayout_19 = QtWidgets.QGridLayout()
         self.gridLayout_19.setObjectName("gridLayout_19")
         self.export_autocontrast = QtWidgets.QCheckBox(self.tab_8)
         self.export_autocontrast.setObjectName("export_autocontrast")
         self.gridLayout_19.addWidget(self.export_autocontrast, 1, 0, 1, 1)
-        self.export_invert = QtWidgets.QCheckBox(self.tab_8)
-        self.export_invert.setObjectName("export_invert")
-        self.gridLayout_19.addWidget(self.export_invert, 1, 2, 1, 1)
         self.export_normalise = QtWidgets.QCheckBox(self.tab_8)
         self.export_normalise.setObjectName("export_normalise")
         self.gridLayout_19.addWidget(self.export_normalise, 1, 1, 1, 1)
+        self.export_scalebar = QtWidgets.QCheckBox(self.tab_8)
+        self.export_scalebar.setObjectName("export_scalebar")
+        self.gridLayout_19.addWidget(self.export_scalebar, 2, 0, 1, 1)
+        self.export_invert = QtWidgets.QCheckBox(self.tab_8)
+        self.export_invert.setObjectName("export_invert")
+        self.gridLayout_19.addWidget(self.export_invert, 1, 2, 1, 1)
+        self.export_mask_background = QtWidgets.QCheckBox(self.tab_8)
+        self.export_mask_background.setObjectName("export_mask_background")
+        self.gridLayout_19.addWidget(self.export_mask_background, 2, 1, 1, 1)
+        self.export_crop_zoom = QtWidgets.QCheckBox(self.tab_8)
+        self.export_crop_zoom.setObjectName("export_crop_zoom")
+        self.gridLayout_19.addWidget(self.export_crop_zoom, 2, 2, 1, 1)
         self.verticalLayout_15.addLayout(self.gridLayout_19)
-        spacerItem31 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_15.addItem(spacerItem31)
+        spacerItem33 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_15.addItem(spacerItem33)
         self.export_active = QtWidgets.QPushButton(self.tab_8)
         self.export_active.setObjectName("export_active")
         self.verticalLayout_15.addWidget(self.export_active)
         self.export_all = QtWidgets.QPushButton(self.tab_8)
         self.export_all.setObjectName("export_all")
         self.verticalLayout_15.addWidget(self.export_all)
         self.tabWidget_4.addTab(self.tab_8, "")
@@ -1535,16 +1732,16 @@
         self.export_colicoords_mode.addItem("")
         self.export_colicoords_mode.addItem("")
         self.gridLayout_11.addWidget(self.export_colicoords_mode, 1, 1, 1, 1)
         self.label_52 = QtWidgets.QLabel(self.tab_9)
         self.label_52.setObjectName("label_52")
         self.gridLayout_11.addWidget(self.label_52, 0, 0, 1, 1)
         self.verticalLayout_17.addLayout(self.gridLayout_11)
-        spacerItem32 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_17.addItem(spacerItem32)
+        spacerItem34 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_17.addItem(spacerItem34)
         self.export_statistics_multithreaded = QtWidgets.QCheckBox(self.tab_9)
         self.export_statistics_multithreaded.setChecked(True)
         self.export_statistics_multithreaded.setObjectName("export_statistics_multithreaded")
         self.verticalLayout_17.addWidget(self.export_statistics_multithreaded)
         self.export_statistics_active = QtWidgets.QPushButton(self.tab_9)
         self.export_statistics_active.setObjectName("export_statistics_active")
         self.verticalLayout_17.addWidget(self.export_statistics_active)
@@ -1587,63 +1784,124 @@
         self.export_edge.setObjectName("export_edge")
         self.gridLayout.addWidget(self.export_edge, 1, 2, 1, 1)
         self.export_broken = QtWidgets.QCheckBox(self.tab_13)
         self.export_broken.setChecked(True)
         self.export_broken.setObjectName("export_broken")
         self.gridLayout.addWidget(self.export_broken, 1, 1, 1, 1)
         self.verticalLayout_16.addLayout(self.gridLayout)
-        spacerItem33 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_16.addItem(spacerItem33)
+        spacerItem35 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_16.addItem(spacerItem35)
+        self.label_49 = QtWidgets.QLabel(self.tab_13)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_49.setFont(font)
+        self.label_49.setObjectName("label_49")
+        self.verticalLayout_16.addWidget(self.label_49)
+        self.gridLayout_27 = QtWidgets.QGridLayout()
+        self.gridLayout_27.setObjectName("gridLayout_27")
+        self.export_scalebar_resolution_units = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_resolution_units.setMaximumSize(QtCore.QSize(200, 100))
+        self.export_scalebar_resolution_units.setObjectName("export_scalebar_resolution_units")
+        self.export_scalebar_resolution_units.addItem("")
+        self.export_scalebar_resolution_units.addItem("")
+        self.gridLayout_27.addWidget(self.export_scalebar_resolution_units, 0, 2, 1, 1)
+        self.label_50 = QtWidgets.QLabel(self.tab_13)
+        self.label_50.setObjectName("label_50")
+        self.gridLayout_27.addWidget(self.label_50, 0, 0, 1, 1)
+        self.export_scalebar_resolution = QtWidgets.QLineEdit(self.tab_13)
+        self.export_scalebar_resolution.setMaximumSize(QtCore.QSize(200, 16777215))
+        self.export_scalebar_resolution.setObjectName("export_scalebar_resolution")
+        self.gridLayout_27.addWidget(self.export_scalebar_resolution, 0, 1, 1, 1)
+        self.label_55 = QtWidgets.QLabel(self.tab_13)
+        self.label_55.setObjectName("label_55")
+        self.gridLayout_27.addWidget(self.label_55, 1, 0, 1, 1)
+        self.export_scalebar_size = QtWidgets.QLineEdit(self.tab_13)
+        self.export_scalebar_size.setMaximumSize(QtCore.QSize(200, 16777215))
+        self.export_scalebar_size.setObjectName("export_scalebar_size")
+        self.gridLayout_27.addWidget(self.export_scalebar_size, 1, 1, 1, 1)
+        self.export_scalebar_size_units = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_size_units.setMaximumSize(QtCore.QSize(200, 100))
+        self.export_scalebar_size_units.setObjectName("export_scalebar_size_units")
+        self.export_scalebar_size_units.addItem("")
+        self.export_scalebar_size_units.addItem("")
+        self.gridLayout_27.addWidget(self.export_scalebar_size_units, 1, 2, 1, 1)
+        self.verticalLayout_16.addLayout(self.gridLayout_27)
+        self.formLayout_19 = QtWidgets.QFormLayout()
+        self.formLayout_19.setObjectName("formLayout_19")
+        self.label_71 = QtWidgets.QLabel(self.tab_13)
+        self.label_71.setObjectName("label_71")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_71)
+        self.export_scalebar_colour = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_colour.setObjectName("export_scalebar_colour")
+        self.export_scalebar_colour.addItem("")
+        self.export_scalebar_colour.addItem("")
+        self.formLayout_19.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_colour)
+        self.label_72 = QtWidgets.QLabel(self.tab_13)
+        self.label_72.setObjectName("label_72")
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_72)
+        self.export_scalebar_thickness = QtWidgets.QComboBox(self.tab_13)
+        self.export_scalebar_thickness.setObjectName("export_scalebar_thickness")
+        self.export_scalebar_thickness.addItem("")
+        self.export_scalebar_thickness.addItem("")
+        self.export_scalebar_thickness.addItem("")
+        self.export_scalebar_thickness.addItem("")
+        self.export_scalebar_thickness.addItem("")
+        self.export_scalebar_thickness.addItem("")
+        self.formLayout_19.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.export_scalebar_thickness)
+        self.verticalLayout_16.addLayout(self.formLayout_19)
+        spacerItem36 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_16.addItem(spacerItem36)
         self.tabWidget_4.addTab(self.tab_13, "")
         self.verticalLayout_6.addWidget(self.tabWidget_4)
         self.formLayout_11 = QtWidgets.QFormLayout()
         self.formLayout_11.setObjectName("formLayout_11")
         self.label_33 = QtWidgets.QLabel(self.export_tab)
         self.label_33.setObjectName("label_33")
         self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_33)
         self.export_progressbar = QtWidgets.QProgressBar(self.export_tab)
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
         self.formLayout_11.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.export_progressbar)
         self.verticalLayout_6.addLayout(self.formLayout_11)
-        spacerItem34 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_6.addItem(spacerItem34)
+        spacerItem37 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_6.addItem(spacerItem37)
         tab_widget.addTab(self.export_tab, "")
         self.tab_14 = QtWidgets.QWidget()
         self.tab_14.setObjectName("tab_14")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.tab_14)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.line_20 = QtWidgets.QFrame(self.tab_14)
         self.line_20.setFrameShape(QtWidgets.QFrame.HLine)
         self.line_20.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_20.setObjectName("line_20")
         self.verticalLayout_18.addWidget(self.line_20)
-        spacerItem35 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem35)
         self.modify_copymasktoall = QtWidgets.QPushButton(self.tab_14)
         self.modify_copymasktoall.setObjectName("modify_copymasktoall")
         self.verticalLayout_18.addWidget(self.modify_copymasktoall)
-        spacerItem36 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem36)
         self.modify_deleteactiveimage = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteactiveimage.setObjectName("modify_deleteactiveimage")
         self.verticalLayout_18.addWidget(self.modify_deleteactiveimage)
         self.modify_deleteotherimages = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteotherimages.setObjectName("modify_deleteotherimages")
         self.verticalLayout_18.addWidget(self.modify_deleteotherimages)
-        spacerItem37 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
-        self.verticalLayout_18.addItem(spacerItem37)
         self.modify_deleteactivemasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteactivemasks.setObjectName("modify_deleteactivemasks")
         self.verticalLayout_18.addWidget(self.modify_deleteactivemasks)
         self.modify_deleteallmasks = QtWidgets.QPushButton(self.tab_14)
         self.modify_deleteallmasks.setObjectName("modify_deleteallmasks")
         self.verticalLayout_18.addWidget(self.modify_deleteallmasks)
         spacerItem38 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.verticalLayout_18.addItem(spacerItem38)
+        self.line_22 = QtWidgets.QFrame(self.tab_14)
+        self.line_22.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_22.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_22.setObjectName("line_22")
+        self.verticalLayout_18.addWidget(self.line_22)
         self.label_31 = QtWidgets.QLabel(self.tab_14)
         font = QtGui.QFont()
         font.setPointSize(10)
         font.setBold(True)
         font.setWeight(75)
         self.label_31.setFont(font)
         self.label_31.setObjectName("label_31")
@@ -1668,49 +1926,108 @@
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_17)
         self.modify_progressbar = QtWidgets.QProgressBar(self.tab_14)
         self.modify_progressbar.setProperty("value", 0)
         self.modify_progressbar.setTextVisible(True)
         self.modify_progressbar.setObjectName("modify_progressbar")
         self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.modify_progressbar)
         self.verticalLayout_18.addLayout(self.formLayout)
-        spacerItem39 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem39 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
         self.verticalLayout_18.addItem(spacerItem39)
+        self.line_23 = QtWidgets.QFrame(self.tab_14)
+        self.line_23.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_23.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_23.setObjectName("line_23")
+        self.verticalLayout_18.addWidget(self.line_23)
+        self.label_56 = QtWidgets.QLabel(self.tab_14)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_56.setFont(font)
+        self.label_56.setObjectName("label_56")
+        self.verticalLayout_18.addWidget(self.label_56)
+        self.gridLayout_7 = QtWidgets.QGridLayout()
+        self.gridLayout_7.setObjectName("gridLayout_7")
+        self.find_previous = QtWidgets.QPushButton(self.tab_14)
+        self.find_previous.setObjectName("find_previous")
+        self.gridLayout_7.addWidget(self.find_previous, 1, 1, 1, 1)
+        self.find_mode = QtWidgets.QComboBox(self.tab_14)
+        self.find_mode.setObjectName("find_mode")
+        self.find_mode.addItem("")
+        self.find_mode.addItem("")
+        self.gridLayout_7.addWidget(self.find_mode, 0, 1, 1, 1)
+        self.find_next = QtWidgets.QPushButton(self.tab_14)
+        self.find_next.setObjectName("find_next")
+        self.gridLayout_7.addWidget(self.find_next, 1, 0, 1, 1)
+        self.find_criterion = QtWidgets.QComboBox(self.tab_14)
+        self.find_criterion.setObjectName("find_criterion")
+        self.find_criterion.addItem("")
+        self.find_criterion.addItem("")
+        self.find_criterion.addItem("")
+        self.gridLayout_7.addWidget(self.find_criterion, 0, 0, 1, 1)
+        self.verticalLayout_18.addLayout(self.gridLayout_7)
+        spacerItem40 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_18.addItem(spacerItem40)
+        self.label_70 = QtWidgets.QLabel(self.tab_14)
+        font = QtGui.QFont()
+        font.setPointSize(10)
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_70.setFont(font)
+        self.label_70.setObjectName("label_70")
+        self.verticalLayout_18.addWidget(self.label_70)
+        self.formLayout_18 = QtWidgets.QFormLayout()
+        self.formLayout_18.setObjectName("formLayout_18")
+        self.alignment_channel = QtWidgets.QComboBox(self.tab_14)
+        self.alignment_channel.setObjectName("alignment_channel")
+        self.formLayout_18.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.alignment_channel)
+        self.label_40 = QtWidgets.QLabel(self.tab_14)
+        self.label_40.setObjectName("label_40")
+        self.formLayout_18.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_40)
+        self.verticalLayout_18.addLayout(self.formLayout_18)
+        self.gridLayout_26 = QtWidgets.QGridLayout()
+        self.gridLayout_26.setObjectName("gridLayout_26")
+        self.align_active_image = QtWidgets.QPushButton(self.tab_14)
+        self.align_active_image.setObjectName("align_active_image")
+        self.gridLayout_26.addWidget(self.align_active_image, 0, 0, 1, 1)
+        self.align_all_images = QtWidgets.QPushButton(self.tab_14)
+        self.align_all_images.setObjectName("align_all_images")
+        self.gridLayout_26.addWidget(self.align_all_images, 0, 1, 1, 1)
+        self.verticalLayout_18.addLayout(self.gridLayout_26)
+        spacerItem41 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_18.addItem(spacerItem41)
         tab_widget.addTab(self.tab_14, "")
 
         self.retranslateUi(tab_widget)
         tab_widget.setCurrentIndex(0)
         self.import_limit.setCurrentIndex(6)
         self.import_precision.setCurrentIndex(1)
+        self.tabWidget.setCurrentIndex(0)
         self.unfold_tile_size.setCurrentIndex(3)
         self.unfold_tile_overlap.setCurrentIndex(3)
         self.tabWidget_3.setCurrentIndex(0)
         self.cellpose_nepochs.setCurrentIndex(3)
         self.cellpose_batchsize.setCurrentIndex(1)
         self.oufti_midline_vertexes.setCurrentIndex(0)
         self.oufti_mesh_length.setCurrentIndex(4)
         self.oufti_mesh_dilation.setCurrentIndex(6)
         self.metadata_controls.setCurrentIndex(0)
         self.tabWidget_2.setCurrentIndex(0)
-        self.download_sort_order.setCurrentIndex(0)
+        self.download_sort_order_2.setCurrentIndex(0)
+        self.download_sort_order_1.setCurrentIndex(0)
         self.tabWidget_4.setCurrentIndex(0)
+        self.export_location.setCurrentIndex(1)
+        self.export_scalebar_size_units.setCurrentIndex(1)
+        self.export_scalebar_thickness.setCurrentIndex(3)
         QtCore.QMetaObject.connectSlotsByName(tab_widget)
 
     def retranslateUi(self, tab_widget):
         _translate = QtCore.QCoreApplication.translate
         tab_widget.setWindowTitle(_translate("tab_widget", "TabWidget"))
         self.label_37.setText(_translate("tab_widget", "General Import Settings"))
-        self.label_27.setText(_translate("tab_widget", "Import Mode"))
-        self.import_mode.setItemText(0, _translate("tab_widget", "Images"))
-        self.import_mode.setItemText(1, _translate("tab_widget", "NanoImager Data"))
-        self.import_mode.setItemText(2, _translate("tab_widget", "ScanR Data"))
-        self.import_mode.setItemText(3, _translate("tab_widget", "ImageJ files(s)"))
-        self.import_mode.setItemText(4, _translate("tab_widget", "Mask (.tif) Segmentation(s)"))
-        self.import_mode.setItemText(5, _translate("tab_widget", "Cellpose (.npy) Segmentation(s)"))
-        self.import_mode.setItemText(6, _translate("tab_widget", "Oufti (.mat) Segmentation(s)"))
-        self.import_mode.setItemText(7, _translate("tab_widget", "JSON (.txt) Segmentation(s)"))
         self.label_51.setText(_translate("tab_widget", "Import File Mode"))
         self.import_filemode.setItemText(0, _translate("tab_widget", "Import File(s)"))
         self.import_filemode.setItemText(1, _translate("tab_widget", "Import Directory"))
         self.import_limit_label.setText(_translate("tab_widget", "Import File Limit"))
         self.import_limit.setItemText(0, _translate("tab_widget", "1"))
         self.import_limit.setItemText(1, _translate("tab_widget", "5"))
         self.import_limit.setItemText(2, _translate("tab_widget", "10"))
@@ -1729,32 +2046,58 @@
         self.import_crop_mode.setItemText(2, _translate("tab_widget", "Crop Right Half"))
         self.import_crop_mode.setItemText(3, _translate("tab_widget", "Crop Brightest Half"))
         self.label_21.setText(_translate("tab_widget", "Import Precision"))
         self.import_precision.setItemText(0, _translate("tab_widget", "int8"))
         self.import_precision.setItemText(1, _translate("tab_widget", "int16"))
         self.import_precision.setItemText(2, _translate("tab_widget", "int32"))
         self.import_precision.setItemText(3, _translate("tab_widget", "native"))
+        self.import_mode.setItemText(0, _translate("tab_widget", "Images"))
+        self.import_mode.setItemText(1, _translate("tab_widget", "NanoImager Data"))
+        self.import_mode.setItemText(2, _translate("tab_widget", "ScanR Data"))
+        self.import_mode.setItemText(3, _translate("tab_widget", "ImageJ files(s)"))
+        self.import_mode.setItemText(4, _translate("tab_widget", "Mask (.tif) Segmentation(s)"))
+        self.import_mode.setItemText(5, _translate("tab_widget", "Cellpose (.npy) Segmentation(s)"))
+        self.import_mode.setItemText(6, _translate("tab_widget", "Oufti (.mat) Segmentation(s)"))
+        self.import_mode.setItemText(7, _translate("tab_widget", "JSON (.txt) Segmentation(s)"))
+        self.label_27.setText(_translate("tab_widget", "Import Mode"))
         self.import_clear_previous.setText(_translate("tab_widget", "Clear previous images"))
         self.import_align.setText(_translate("tab_widget", "Align Image Channels (Slow)"))
         self.import_import.setText(_translate("tab_widget", "Import"))
         self.label_36.setText(_translate("tab_widget", "Progress"))
         tab_widget.setTabText(tab_widget.indexOf(self.import_tab), _translate("tab_widget", "Import"))
         self.label_60.setText(_translate("tab_widget", "Auto Contrast Adjustment"))
         self.import_auto_contrast.setText(_translate("tab_widget", "Auto Contrast Adjustment"))
         self.label_38.setText(_translate("tab_widget", "View Mask/Class Labels"))
         self.modify_viewlabels.setText(_translate("tab_widget", "View Class Labels [x]"))
         self.modify_viewmasks.setText(_translate("tab_widget", "View Masks [Z]"))
-        self.label_56.setText(_translate("tab_widget", "Find/Sort Cells"))
-        self.find_previous.setText(_translate("tab_widget", "Find Previous"))
-        self.find_mode.setItemText(0, _translate("tab_widget", "Ascending"))
-        self.find_mode.setItemText(1, _translate("tab_widget", "Descending"))
-        self.find_next.setText(_translate("tab_widget", "Find Next"))
-        self.find_criterion.setItemText(0, _translate("tab_widget", "Cell Area"))
-        self.find_criterion.setItemText(1, _translate("tab_widget", "Cell Solidity"))
-        self.find_criterion.setItemText(2, _translate("tab_widget", "Cell Aspect Ratio"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_16), _translate("tab_widget", "General"))
+        self.label_47.setText(_translate("tab_widget", "Scale Bar Settings"))
+        self.scalebar_show.setText(_translate("tab_widget", "Show Scale Bar"))
+        self.scalebar_units.setItemText(0, _translate("tab_widget", "um"))
+        self.scalebar_units.setItemText(1, _translate("tab_widget", "nm"))
+        self.label_48.setText(_translate("tab_widget", "Pixel Resolution (um)"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_7), _translate("tab_widget", "Scale Bar"))
+        self.label_73.setText(_translate("tab_widget", "Information Overlay Settings"))
+        self.overlay_filename.setText(_translate("tab_widget", "File Name"))
+        self.overlay_folder.setText(_translate("tab_widget", "Folder"))
+        self.overlay_antibiotic.setText(_translate("tab_widget", "Antibiotic"))
+        self.overlay_phenotype.setText(_translate("tab_widget", "Phenotype"))
+        self.overlay_strain.setText(_translate("tab_widget", "Strain"))
+        self.overlay_content.setText(_translate("tab_widget", "Content"))
+        self.overlay_microscope.setText(_translate("tab_widget", "Microscope"))
+        self.overlay_datemodified.setText(_translate("tab_widget", "Date Modified"))
+        self.overlay_lightsource.setText(_translate("tab_widget", "Light Source"))
+        self.overlay_staintarget.setText(_translate("tab_widget", "Stain Target"))
+        self.overlay_modality.setText(_translate("tab_widget", "Modality"))
+        self.overlay_stain.setText(_translate("tab_widget", "Stain"))
+        self.overlay_focus.setText(_translate("tab_widget", "Image Focus"))
+        self.overlay_laplacian.setText(_translate("tab_widget", "Image Laplacian"))
+        self.overlay_debris.setText(_translate("tab_widget", "Image Debris"))
+        self.overlay_range.setText(_translate("tab_widget", "Image Range"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_15), _translate("tab_widget", "Overlay"))
         self.label_57.setText(_translate("tab_widget", "Unfold/Fold into Tiles"))
         self.unfold.setText(_translate("tab_widget", "Unfold"))
         self.fold.setText(_translate("tab_widget", "Fold"))
         self.label_58.setText(_translate("tab_widget", "Tile Size (Pixels)"))
         self.unfold_tile_size.setItemText(0, _translate("tab_widget", "100"))
         self.unfold_tile_size.setItemText(1, _translate("tab_widget", "200"))
         self.unfold_tile_size.setItemText(2, _translate("tab_widget", "300"))
@@ -1765,14 +2108,15 @@
         self.unfold_tile_overlap.setItemText(1, _translate("tab_widget", "20"))
         self.unfold_tile_overlap.setItemText(2, _translate("tab_widget", "30"))
         self.unfold_tile_overlap.setItemText(3, _translate("tab_widget", "50"))
         self.unfold_tile_overlap.setItemText(4, _translate("tab_widget", "100"))
         self.label_62.setText(_translate("tab_widget", "Mode"))
         self.unfold_mode.setItemText(0, _translate("tab_widget", "Nested Tiles"))
         self.unfold_mode.setItemText(1, _translate("tab_widget", "Smaller Images (Extra FOVs)"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_17), _translate("tab_widget", "Fold/Unfold"))
         tab_widget.setTabText(tab_widget.indexOf(self.tab), _translate("tab_widget", "View"))
         self.cellpose_select_custom_model.setText(_translate("tab_widget", "Select Custom Cellpose Model"))
         self.label_2.setText(_translate("tab_widget", "Segmentation Channel"))
         self.label.setText(_translate("tab_widget", "Cellpose Model"))
         self.cellpose_segmodel.setItemText(0, _translate("tab_widget", "cyto"))
         self.cellpose_segmodel.setItemText(1, _translate("tab_widget", "nuclei"))
         self.cellpose_segmodel.setItemText(2, _translate("tab_widget", "tissuenet"))
@@ -1917,14 +2261,21 @@
         self.label_76.setText(_translate("tab_widget", "Antibiotic"))
         self.label_77.setText(_translate("tab_widget", "Treatment Time (mins)"))
         self.label_78.setText(_translate("tab_widget", "Antibiotic Concentration"))
         self.label_79.setText(_translate("tab_widget", "Mounting Method"))
         self.upload_mount.setItemText(1, _translate("tab_widget", "Agarose"))
         self.upload_mount.setItemText(2, _translate("tab_widget", "Chitosan"))
         self.label_80.setText(_translate("tab_widget", "Protocol"))
+        self.upload_phenotype.setItemText(1, _translate("tab_widget", "Untreated"))
+        self.upload_phenotype.setItemText(2, _translate("tab_widget", "Treated"))
+        self.upload_phenotype.setItemText(3, _translate("tab_widget", "Treated Sensitive"))
+        self.upload_phenotype.setItemText(4, _translate("tab_widget", "Treated Resistant"))
+        self.label_41.setText(_translate("tab_widget", "Phenotype"))
+        self.label_42.setText(_translate("tab_widget", "Strain"))
+        self.upload_strain.setItemText(1, _translate("tab_widget", "MG1655"))
         self.metadata_controls.setTabText(self.metadata_controls.indexOf(self.experiment_metadata), _translate("tab_widget", "Experiment Metadata"))
         self.label_67.setText(_translate("tab_widget", "Modality"))
         self.label_modality.setItemText(0, _translate("tab_widget", "Required for upload"))
         self.label_modality.setItemText(1, _translate("tab_widget", "Bright Field"))
         self.label_modality.setItemText(2, _translate("tab_widget", "Dark Field"))
         self.label_modality.setItemText(3, _translate("tab_widget", "Phase Contrast"))
         self.label_modality.setItemText(4, _translate("tab_widget", "Fake Phase Contrast"))
@@ -1969,33 +2320,52 @@
         self.upload_segmentation_combo.setItemText(1, _translate("tab_widget", "Not Segmented"))
         self.upload_segmentation_combo.setItemText(2, _translate("tab_widget", "Segmented"))
         self.upload_segmentation_combo.setItemText(3, _translate("tab_widget", "Curated Segmentations"))
         self.label_84.setText(_translate("tab_widget", "Labelled"))
         self.upload_label_combo.setItemText(1, _translate("tab_widget", "Not Labelled"))
         self.upload_label_combo.setItemText(2, _translate("tab_widget", "Labelled"))
         self.upload_label_combo.setItemText(3, _translate("tab_widget", "Curated Labels"))
-        self.download_sort_order.setItemText(0, _translate("tab_widget", "Random"))
-        self.download_sort_order.setItemText(1, _translate("tab_widget", "Date Uploaded (Ascending)"))
-        self.download_sort_order.setItemText(2, _translate("tab_widget", "Date Uploaded (Descending)"))
-        self.download_sort_order.setItemText(3, _translate("tab_widget", "Date Modifed (Ascending)"))
-        self.download_sort_order.setItemText(4, _translate("tab_widget", "Date Modifed (Descending)"))
-        self.label_15.setText(_translate("tab_widget", "Sort Order"))
+        self.download_sort_order_2.setItemText(1, _translate("tab_widget", "Random"))
+        self.download_sort_order_2.setItemText(2, _translate("tab_widget", "Date Uploaded"))
+        self.download_sort_order_2.setItemText(3, _translate("tab_widget", "Date Modifed"))
+        self.download_sort_order_2.setItemText(4, _translate("tab_widget", "Image Laplacian"))
+        self.download_sort_order_2.setItemText(5, _translate("tab_widget", "Num Segmentations"))
+        self.download_sort_order_2.setItemText(6, _translate("tab_widget", "Image Focus"))
+        self.download_sort_order_2.setItemText(7, _translate("tab_widget", "Image Debris"))
+        self.label_15.setText(_translate("tab_widget", "Primary Sort Order"))
+        self.download_sort_direction_1.setItemText(1, _translate("tab_widget", "Ascending"))
+        self.download_sort_direction_1.setItemText(2, _translate("tab_widget", "Descending"))
+        self.download_sort_order_1.setItemText(1, _translate("tab_widget", "Random"))
+        self.download_sort_order_1.setItemText(2, _translate("tab_widget", "Date Uploaded"))
+        self.download_sort_order_1.setItemText(3, _translate("tab_widget", "Date Modifed"))
+        self.download_sort_order_1.setItemText(4, _translate("tab_widget", "Image Laplacian"))
+        self.download_sort_order_1.setItemText(5, _translate("tab_widget", "Num Segmentations"))
+        self.download_sort_order_1.setItemText(6, _translate("tab_widget", "Image Focus"))
+        self.download_sort_order_1.setItemText(7, _translate("tab_widget", "Image Debris"))
+        self.label_23.setText(_translate("tab_widget", "Secondary Sort Order"))
+        self.download_sort_direction_2.setItemText(1, _translate("tab_widget", "Ascending"))
+        self.download_sort_direction_2.setItemText(2, _translate("tab_widget", "Descending"))
         self.label_88.setText(_translate("tab_widget", "Download Limit"))
         self.database_download_limit.setItemText(0, _translate("tab_widget", "1"))
         self.database_download_limit.setItemText(1, _translate("tab_widget", "5"))
         self.database_download_limit.setItemText(2, _translate("tab_widget", "10"))
         self.database_download_limit.setItemText(3, _translate("tab_widget", "20"))
         self.database_download_limit.setItemText(4, _translate("tab_widget", "50"))
         self.database_download_limit.setItemText(5, _translate("tab_widget", "100"))
         self.database_download_limit.setItemText(6, _translate("tab_widget", "All"))
         self.database_download.setText(_translate("tab_widget", "Download [Control-L]"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_10), _translate("tab_widget", "Database Download"))
-        self.overwrite_all_metadata.setText(_translate("tab_widget", "Overwrite All Metadata"))
-        self.upload_overwrite_images.setText(_translate("tab_widget", "Overwrite Images"))
+        self.label_24.setText(_translate("tab_widget", "Upload Data"))
+        self.upload_segmentations_setting.setText(_translate("tab_widget", "Segmentations/labels"))
+        self.upload_images_setting.setText(_translate("tab_widget", "Images"))
+        self.upload_metadata_setting.setText(_translate("tab_widget", "Metadata"))
+        self.label_32.setText(_translate("tab_widget", "Upload Settings"))
         self.upload_overwrite_masks.setText(_translate("tab_widget", "Overwrite Masks/Labels"))
+        self.upload_overwrite_images.setText(_translate("tab_widget", "Overwrite Images"))
+        self.overwrite_all_metadata.setText(_translate("tab_widget", "Overwrite All Metadata"))
         self.overwrite_selected_metadata.setText(_translate("tab_widget", "Overwrite Selected Metadata"))
         self.upload_all.setText(_translate("tab_widget", "Upload All Images [Control-Shift-U]"))
         self.upload_active.setText(_translate("tab_widget", "Upload Active Image [Control-U]"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_4), _translate("tab_widget", "Database Upload"))
         self.label_89.setText(_translate("tab_widget", "Progress"))
         tab_widget.setTabText(tab_widget.indexOf(self.upload_tab), _translate("tab_widget", "Database"))
         self.export_mode.setItemText(0, _translate("tab_widget", "Export .tif Images"))
@@ -2015,16 +2385,19 @@
         self.label_45.setText(_translate("tab_widget", "Image Channel"))
         self.label_26.setText(_translate("tab_widget", "File Name Modifier"))
         self.export_modifier.setText(_translate("tab_widget", "_BacSeg"))
         self.export_overwrite_setting.setText(_translate("tab_widget", "Overwrite Files"))
         self.export_image_setting.setText(_translate("tab_widget", "Export Image Files"))
         self.label_12.setText(_translate("tab_widget", "Image Modifications"))
         self.export_autocontrast.setText(_translate("tab_widget", "Auto Contrast"))
-        self.export_invert.setText(_translate("tab_widget", "Invert "))
         self.export_normalise.setText(_translate("tab_widget", "Normalise"))
+        self.export_scalebar.setText(_translate("tab_widget", "Show Scale Bar"))
+        self.export_invert.setText(_translate("tab_widget", "Invert "))
+        self.export_mask_background.setText(_translate("tab_widget", "Mask Background"))
+        self.export_crop_zoom.setText(_translate("tab_widget", "Crop to Current Zoom"))
         self.export_active.setText(_translate("tab_widget", "Export Data From Active Image"))
         self.export_all.setText(_translate("tab_widget", "Export Data From All Images"))
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_8), _translate("tab_widget", "Export Data"))
         self.label_46.setText(_translate("tab_widget", "Export Cell Statistics"))
         self.label_54.setText(_translate("tab_widget", "ColiCoords Fit Mode"))
         self.export_statistics_pixelsize.setText(_translate("tab_widget", "0.116999998688698"))
         self.export_colicoords_mode.setItemText(0, _translate("tab_widget", "None (OpenCV Stats)"))
@@ -2037,21 +2410,52 @@
         self.label_43.setText(_translate("tab_widget", "Export Cell Settings"))
         self.export_single.setText(_translate("tab_widget", "Single"))
         self.export_vertical.setText(_translate("tab_widget", "Vertical"))
         self.export_divided.setText(_translate("tab_widget", "Divided"))
         self.export_dividing.setText(_translate("tab_widget", "Dividing"))
         self.export_edge.setText(_translate("tab_widget", "Edge"))
         self.export_broken.setText(_translate("tab_widget", "Broken"))
+        self.label_49.setText(_translate("tab_widget", "Scale Bar Settings"))
+        self.export_scalebar_resolution_units.setItemText(0, _translate("tab_widget", "nm"))
+        self.export_scalebar_resolution_units.setItemText(1, _translate("tab_widget", "um"))
+        self.label_50.setText(_translate("tab_widget", "Pixel Resolution"))
+        self.export_scalebar_resolution.setText(_translate("tab_widget", "100"))
+        self.label_55.setText(_translate("tab_widget", "Scale Bar Size"))
+        self.export_scalebar_size.setText(_translate("tab_widget", "20"))
+        self.export_scalebar_size_units.setItemText(0, _translate("tab_widget", "nm"))
+        self.export_scalebar_size_units.setItemText(1, _translate("tab_widget", "um"))
+        self.label_71.setText(_translate("tab_widget", "Scale Bar Colour"))
+        self.export_scalebar_colour.setItemText(0, _translate("tab_widget", "Black"))
+        self.export_scalebar_colour.setItemText(1, _translate("tab_widget", "White"))
+        self.label_72.setText(_translate("tab_widget", "Scale Bar Thickness (pixels)"))
+        self.export_scalebar_thickness.setItemText(0, _translate("tab_widget", "1"))
+        self.export_scalebar_thickness.setItemText(1, _translate("tab_widget", "2"))
+        self.export_scalebar_thickness.setItemText(2, _translate("tab_widget", "5"))
+        self.export_scalebar_thickness.setItemText(3, _translate("tab_widget", "10"))
+        self.export_scalebar_thickness.setItemText(4, _translate("tab_widget", "15"))
+        self.export_scalebar_thickness.setItemText(5, _translate("tab_widget", "20"))
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_13), _translate("tab_widget", "Export Settings"))
         self.label_33.setText(_translate("tab_widget", "Progress "))
         tab_widget.setTabText(tab_widget.indexOf(self.export_tab), _translate("tab_widget", "Export"))
         self.modify_copymasktoall.setText(_translate("tab_widget", "Copy Mask From Active Image to All Images"))
         self.modify_deleteactiveimage.setText(_translate("tab_widget", "Delete Active Image [Control-I]"))
         self.modify_deleteotherimages.setText(_translate("tab_widget", "Delete All Images Except Active Image [Control-Shift-I]"))
         self.modify_deleteactivemasks.setText(_translate("tab_widget", "Delete All Masks, Active Image [Control-D]"))
         self.modify_deleteallmasks.setText(_translate("tab_widget", "Delete All Masks, All Images [Control-Shift-D]"))
         self.label_31.setText(_translate("tab_widget", "Refine Settings (ColiCoords):"))
         self.label_53.setText(_translate("tab_widget", "Refine Channel"))
         self.refine_channel.setItemText(0, _translate("tab_widget", "Mask"))
         self.refine_all.setText(_translate("tab_widget", "Refine All Segmentations In Active Image"))
         self.label_17.setText(_translate("tab_widget", "Progress"))
-        tab_widget.setTabText(tab_widget.indexOf(self.tab_14), _translate("tab_widget", "Misc"))
+        self.label_56.setText(_translate("tab_widget", "Find/Sort Cells"))
+        self.find_previous.setText(_translate("tab_widget", "Find Previous"))
+        self.find_mode.setItemText(0, _translate("tab_widget", "Ascending"))
+        self.find_mode.setItemText(1, _translate("tab_widget", "Descending"))
+        self.find_next.setText(_translate("tab_widget", "Find Next"))
+        self.find_criterion.setItemText(0, _translate("tab_widget", "Cell Area"))
+        self.find_criterion.setItemText(1, _translate("tab_widget", "Cell Solidity"))
+        self.find_criterion.setItemText(2, _translate("tab_widget", "Cell Aspect Ratio"))
+        self.label_70.setText(_translate("tab_widget", "Automatic Channel Alignment/Registration"))
+        self.label_40.setText(_translate("tab_widget", "Reference Channel"))
+        self.align_active_image.setText(_translate("tab_widget", "Align Active Image"))
+        self.align_all_images.setText(_translate("tab_widget", "Align All Images"))
+        tab_widget.setTabText(tab_widget.indexOf(self.tab_14), _translate("tab_widget", "Utilities"))
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.ui`

 * *Files 4% similar despite different names*

#### Comparing `napari-bacseg-1.0.4/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.5/src/napari_bacseg/bacseg_ui.ui`

```diff
@@ -6,15 +6,15 @@
       <bool>true</bool>
     </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>681</width>
-        <height>1011</height>
+        <height>1133</height>
       </rect>
     </property>
     <property name="sizePolicy">
       <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
         <horstretch>0</horstretch>
         <verstretch>100</verstretch>
       </sizepolicy>
@@ -75,65 +75,14 @@
             <property name="text">
               <string>General Import Settings</string>
             </property>
           </widget>
         </item>
         <item>
           <layout class="QFormLayout" name="formLayout_8">
-            <item row="1" column="0">
-              <widget class="QLabel" name="label_27">
-                <property name="text">
-                  <string>Import Mode</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="1">
-              <widget class="QComboBox" name="import_mode">
-                <item>
-                  <property name="text">
-                    <string>Images</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>NanoImager Data</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>ScanR Data</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>ImageJ files(s)</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>Mask (.tif) Segmentation(s)</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>Cellpose (.npy) Segmentation(s)</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>Oufti (.mat) Segmentation(s)</string>
-                  </property>
-                </item>
-                <item>
-                  <property name="text">
-                    <string>JSON (.txt) Segmentation(s)</string>
-                  </property>
-                </item>
-              </widget>
-            </item>
             <item row="2" column="1">
               <spacer name="verticalSpacer_16">
                 <property name="orientation">
                   <enum>Qt::Vertical</enum>
                 </property>
                 <property name="sizeType">
                   <enum>QSizePolicy::Minimum</enum>
@@ -324,14 +273,65 @@
                 <item>
                   <property name="text">
                     <string>native</string>
                   </property>
                 </item>
               </widget>
             </item>
+            <item row="0" column="1">
+              <widget class="QComboBox" name="import_mode">
+                <item>
+                  <property name="text">
+                    <string>Images</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>NanoImager Data</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>ScanR Data</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>ImageJ files(s)</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Mask (.tif) Segmentation(s)</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Cellpose (.npy) Segmentation(s)</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Oufti (.mat) Segmentation(s)</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>JSON (.txt) Segmentation(s)</string>
+                  </property>
+                </item>
+              </widget>
+            </item>
+            <item row="1" column="0">
+              <widget class="QLabel" name="label_27">
+                <property name="text">
+                  <string>Import Mode</string>
+                </property>
+              </widget>
+            </item>
           </layout>
         </item>
         <item>
           <spacer name="verticalSpacer_15">
             <property name="orientation">
               <enum>Qt::Vertical</enum>
             </property>
@@ -428,350 +428,549 @@
     </widget>
     <widget class="QWidget" name="tab">
       <attribute name="title">
         <string>View</string>
       </attribute>
       <layout class="QVBoxLayout" name="verticalLayout_5">
         <item>
-          <widget class="Line" name="line_27">
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <widget class="QLabel" name="label_60">
-            <property name="font">
-              <font>
-                <pointsize>10</pointsize>
-                <weight>75</weight>
-                <bold>true</bold>
-              </font>
-            </property>
-            <property name="text">
-              <string>Auto Contrast Adjustment</string>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <widget class="QCheckBox" name="import_auto_contrast">
-            <property name="text">
-              <string>Auto Contrast Adjustment</string>
-            </property>
-            <property name="checked">
-              <bool>true</bool>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <spacer name="verticalSpacer_18">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>20</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
-          <widget class="Line" name="line_26">
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <widget class="QLabel" name="label_38">
-            <property name="font">
-              <font>
-                <pointsize>10</pointsize>
-                <weight>75</weight>
-                <bold>true</bold>
-              </font>
-            </property>
-            <property name="text">
-              <string>View Mask/Class Labels</string>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <layout class="QGridLayout" name="gridLayout_6">
-            <item row="1" column="1">
-              <widget class="QCheckBox" name="modify_viewlabels">
-                <property name="text">
-                  <string>View Class Labels [x]</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QCheckBox" name="modify_viewmasks">
-                <property name="text">
-                  <string>View Masks [Z]</string>
-                </property>
-              </widget>
-            </item>
-          </layout>
-        </item>
-        <item>
-          <spacer name="verticalSpacer_8">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>20</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
-          <widget class="Line" name="line_17">
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <widget class="QLabel" name="label_56">
-            <property name="font">
-              <font>
-                <pointsize>10</pointsize>
-                <weight>75</weight>
-                <bold>true</bold>
-              </font>
+          <widget class="QTabWidget" name="tabWidget">
+            <property name="sizePolicy">
+              <sizepolicy hsizetype="Expanding" vsizetype="Preferred">
+                <horstretch>0</horstretch>
+                <verstretch>0</verstretch>
+              </sizepolicy>
             </property>
-            <property name="text">
-              <string>Find/Sort Cells</string>
+            <property name="currentIndex">
+              <number>0</number>
             </property>
-          </widget>
-        </item>
-        <item>
-          <layout class="QGridLayout" name="gridLayout_7">
-            <item row="1" column="1">
-              <widget class="QPushButton" name="find_previous">
-                <property name="text">
-                  <string>Find Previous</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QComboBox" name="find_mode">
+            <widget class="QWidget" name="tab_16">
+              <attribute name="title">
+                <string>General</string>
+              </attribute>
+              <layout class="QVBoxLayout" name="verticalLayout_23">
                 <item>
-                  <property name="text">
-                    <string>Ascending</string>
-                  </property>
+                  <widget class="QLabel" name="label_60">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Auto Contrast Adjustment</string>
+                    </property>
+                  </widget>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>Descending</string>
-                  </property>
+                  <widget class="QCheckBox" name="import_auto_contrast">
+                    <property name="text">
+                      <string>Auto Contrast Adjustment</string>
+                    </property>
+                    <property name="checked">
+                      <bool>true</bool>
+                    </property>
+                  </widget>
                 </item>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="QPushButton" name="find_next">
-                <property name="text">
-                  <string>Find Next</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="0">
-              <widget class="QComboBox" name="find_criterion">
                 <item>
-                  <property name="text">
-                    <string>Cell Area</string>
-                  </property>
+                  <spacer name="verticalSpacer_43">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>1</height>
+                      </size>
+                    </property>
+                  </spacer>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>Cell Solidity</string>
-                  </property>
+                  <widget class="Line" name="line_29">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>Cell Aspect Ratio</string>
-                  </property>
+                  <widget class="QLabel" name="label_38">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>View Mask/Class Labels</string>
+                    </property>
+                  </widget>
                 </item>
-              </widget>
-            </item>
-          </layout>
-        </item>
-        <item>
-          <spacer name="verticalSpacer_7">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>20</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
-          <widget class="Line" name="line_25">
-            <property name="orientation">
-              <enum>Qt::Horizontal</enum>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <widget class="QLabel" name="label_57">
-            <property name="font">
-              <font>
-                <pointsize>10</pointsize>
-                <weight>75</weight>
-                <bold>true</bold>
-              </font>
-            </property>
-            <property name="text">
-              <string>Unfold/Fold into Tiles</string>
-            </property>
-          </widget>
-        </item>
-        <item>
-          <layout class="QGridLayout" name="gridLayout_8">
-            <item row="0" column="0">
-              <widget class="QPushButton" name="unfold">
-                <property name="text">
-                  <string>Unfold</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QPushButton" name="fold">
-                <property name="text">
-                  <string>Fold</string>
-                </property>
-              </widget>
-            </item>
-          </layout>
-        </item>
-        <item>
-          <layout class="QFormLayout" name="formLayout_3">
-            <item row="1" column="0">
-              <widget class="QLabel" name="label_58">
-                <property name="text">
-                  <string>Tile Size (Pixels)</string>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="1">
-              <widget class="QComboBox" name="unfold_tile_size">
-                <property name="editable">
-                  <bool>true</bool>
-                </property>
-                <property name="currentIndex">
-                  <number>3</number>
-                </property>
                 <item>
-                  <property name="text">
-                    <string>100</string>
-                  </property>
+                  <layout class="QGridLayout" name="gridLayout_6">
+                    <item row="1" column="1">
+                      <widget class="QCheckBox" name="modify_viewlabels">
+                        <property name="text">
+                          <string>View Class Labels [x]</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QCheckBox" name="modify_viewmasks">
+                        <property name="text">
+                          <string>View Masks [Z]</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>200</string>
-                  </property>
+                  <spacer name="verticalSpacer_37">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>1</height>
+                      </size>
+                    </property>
+                  </spacer>
                 </item>
+              </layout>
+            </widget>
+            <widget class="QWidget" name="tab_7">
+              <attribute name="title">
+                <string>Scale Bar</string>
+              </attribute>
+              <layout class="QVBoxLayout" name="verticalLayout_21">
                 <item>
-                  <property name="text">
-                    <string>300</string>
-                  </property>
+                  <widget class="Line" name="line_26">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>500</string>
-                  </property>
+                  <widget class="QLabel" name="label_47">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Scale Bar Settings</string>
+                    </property>
+                  </widget>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>1000</string>
-                  </property>
+                  <widget class="QCheckBox" name="scalebar_show">
+                    <property name="text">
+                      <string>Show Scale Bar</string>
+                    </property>
+                  </widget>
                 </item>
-              </widget>
-            </item>
-            <item row="2" column="0">
-              <widget class="QLabel" name="label_59">
-                <property name="text">
-                  <string>Tile Overlap (Pixels)</string>
-                </property>
-              </widget>
-            </item>
-            <item row="2" column="1">
-              <widget class="QComboBox" name="unfold_tile_overlap">
-                <property name="editable">
-                  <bool>true</bool>
-                </property>
-                <property name="currentIndex">
-                  <number>3</number>
-                </property>
                 <item>
-                  <property name="text">
-                    <string>10</string>
-                  </property>
+                  <layout class="QGridLayout" name="gridLayout_20">
+                    <item row="0" column="1">
+                      <widget class="QLineEdit" name="scalebar_resolution">
+                        <property name="maximumSize">
+                          <size>
+                            <width>200</width>
+                            <height>16777215</height>
+                          </size>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <widget class="QComboBox" name="scalebar_units">
+                        <property name="maximumSize">
+                          <size>
+                            <width>200</width>
+                            <height>100</height>
+                          </size>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>um</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>nm</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_48">
+                        <property name="text">
+                          <string>Pixel Resolution (um)</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>20</string>
-                  </property>
+                  <spacer name="verticalSpacer_8">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>1</height>
+                      </size>
+                    </property>
+                  </spacer>
                 </item>
+              </layout>
+            </widget>
+            <widget class="QWidget" name="tab_15">
+              <attribute name="title">
+                <string>Overlay</string>
+              </attribute>
+              <layout class="QVBoxLayout" name="verticalLayout_22">
                 <item>
-                  <property name="text">
-                    <string>30</string>
-                  </property>
+                  <widget class="Line" name="line_27">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>50</string>
-                  </property>
+                  <widget class="QLabel" name="label_73">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Information Overlay Settings</string>
+                    </property>
+                  </widget>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>100</string>
-                  </property>
+                  <layout class="QGridLayout" name="gridLayout_28">
+                    <item row="0" column="0">
+                      <widget class="QCheckBox" name="overlay_filename">
+                        <property name="text">
+                          <string>File Name</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QCheckBox" name="overlay_folder">
+                        <property name="text">
+                          <string>Folder</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="4">
+                      <widget class="QCheckBox" name="overlay_antibiotic">
+                        <property name="text">
+                          <string>Antibiotic</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="3">
+                      <widget class="QCheckBox" name="overlay_phenotype">
+                        <property name="text">
+                          <string>Phenotype</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="1">
+                      <widget class="QCheckBox" name="overlay_strain">
+                        <property name="text">
+                          <string>Strain</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="0">
+                      <widget class="QCheckBox" name="overlay_content">
+                        <property name="text">
+                          <string>Content</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="3">
+                      <widget class="QCheckBox" name="overlay_microscope">
+                        <property name="text">
+                          <string>Microscope</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="4">
+                      <widget class="QCheckBox" name="overlay_datemodified">
+                        <property name="text">
+                          <string>Date Modified</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
-              </widget>
-            </item>
-            <item row="0" column="0">
-              <widget class="QLabel" name="label_62">
-                <property name="text">
-                  <string>Mode</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="QComboBox" name="unfold_mode">
                 <item>
-                  <property name="text">
-                    <string>Nested Tiles</string>
-                  </property>
+                  <layout class="QGridLayout" name="gridLayout_29">
+                    <item row="0" column="3">
+                      <widget class="QCheckBox" name="overlay_lightsource">
+                        <property name="text">
+                          <string>Light Source</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QCheckBox" name="overlay_staintarget">
+                        <property name="text">
+                          <string>Stain Target</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <widget class="QCheckBox" name="overlay_modality">
+                        <property name="text">
+                          <string>Modality</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QCheckBox" name="overlay_stain">
+                        <property name="text">
+                          <string>Stain</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
                 <item>
-                  <property name="text">
-                    <string>Smaller Images (Extra FOVs)</string>
-                  </property>
+                  <layout class="QGridLayout" name="gridLayout_30">
+                    <item row="0" column="0">
+                      <widget class="QCheckBox" name="overlay_focus">
+                        <property name="text">
+                          <string>Image Focus</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <widget class="QCheckBox" name="overlay_laplacian">
+                        <property name="text">
+                          <string>Image Laplacian</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QCheckBox" name="overlay_debris">
+                        <property name="text">
+                          <string>Image Debris</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="3">
+                      <widget class="QCheckBox" name="overlay_range">
+                        <property name="text">
+                          <string>Image Range</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
-              </widget>
-            </item>
-          </layout>
+                <item>
+                  <spacer name="verticalSpacer_30">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeType">
+                      <enum>QSizePolicy::Minimum</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>1</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+              </layout>
+            </widget>
+            <widget class="QWidget" name="tab_17">
+              <attribute name="title">
+                <string>Fold/Unfold</string>
+              </attribute>
+              <layout class="QVBoxLayout" name="verticalLayout_24">
+                <item>
+                  <widget class="Line" name="line_28">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_57">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Unfold/Fold into Tiles</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QGridLayout" name="gridLayout_8">
+                    <item row="0" column="0">
+                      <widget class="QPushButton" name="unfold">
+                        <property name="text">
+                          <string>Unfold</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QPushButton" name="fold">
+                        <property name="text">
+                          <string>Fold</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <layout class="QFormLayout" name="formLayout_3">
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="label_58">
+                        <property name="text">
+                          <string>Tile Size (Pixels)</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="1">
+                      <widget class="QComboBox" name="unfold_tile_size">
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                        <property name="currentIndex">
+                          <number>3</number>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>100</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>200</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>300</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>500</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>1000</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="2" column="0">
+                      <widget class="QLabel" name="label_59">
+                        <property name="text">
+                          <string>Tile Overlap (Pixels)</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="1">
+                      <widget class="QComboBox" name="unfold_tile_overlap">
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                        <property name="currentIndex">
+                          <number>3</number>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>20</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>30</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>50</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>100</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_62">
+                        <property name="text">
+                          <string>Mode</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="unfold_mode">
+                        <item>
+                          <property name="text">
+                            <string>Nested Tiles</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Smaller Images (Extra FOVs)</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <spacer name="verticalSpacer_38">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>1</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+              </layout>
+            </widget>
+          </widget>
         </item>
         <item>
           <spacer name="verticalSpacer_6">
             <property name="orientation">
               <enum>Qt::Vertical</enum>
             </property>
             <property name="sizeHint" stdset="0">
@@ -2408,78 +2607,78 @@
                         <item>
                           <property name="text">
                             <string>Required for upload</string>
                           </property>
                         </item>
                       </widget>
                     </item>
-                    <item row="4" column="0">
+                    <item row="5" column="0">
                       <widget class="QLabel" name="label_76">
                         <property name="text">
                           <string>Antibiotic</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="4" column="1">
+                    <item row="5" column="1">
                       <widget class="QComboBox" name="upload_antibiotic">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="editable">
                           <bool>true</bool>
                         </property>
                       </widget>
                     </item>
-                    <item row="5" column="0">
+                    <item row="6" column="0">
                       <widget class="QLabel" name="label_77">
                         <property name="text">
                           <string>Treatment Time (mins)</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="5" column="1">
+                    <item row="6" column="1">
                       <widget class="QComboBox" name="upload_treatmenttime">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="editable">
                           <bool>true</bool>
                         </property>
                         <item>
                           <property name="text">
                             <string/>
                           </property>
                         </item>
                       </widget>
                     </item>
-                    <item row="6" column="0">
+                    <item row="7" column="0">
                       <widget class="QLabel" name="label_78">
                         <property name="text">
                           <string>Antibiotic Concentration</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="6" column="1">
+                    <item row="7" column="1">
                       <widget class="QComboBox" name="upload_abxconcentration">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="editable">
                           <bool>true</bool>
                         </property>
                       </widget>
                     </item>
-                    <item row="7" column="0">
+                    <item row="8" column="0">
                       <widget class="QLabel" name="label_79">
                         <property name="text">
                           <string>Mounting Method</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="7" column="1">
+                    <item row="8" column="1">
                       <widget class="QComboBox" name="upload_mount">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="editable">
                           <bool>true</bool>
                         </property>
@@ -2496,36 +2695,99 @@
                         <item>
                           <property name="text">
                             <string>Chitosan</string>
                           </property>
                         </item>
                       </widget>
                     </item>
-                    <item row="8" column="0">
+                    <item row="9" column="0">
                       <widget class="QLabel" name="label_80">
                         <property name="text">
                           <string>Protocol</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="8" column="1">
+                    <item row="9" column="1">
                       <widget class="QComboBox" name="upload_protocol">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="editable">
                           <bool>true</bool>
                         </property>
                         <item>
                           <property name="text">
                             <string/>
                           </property>
                         </item>
                       </widget>
                     </item>
+                    <item row="4" column="1">
+                      <widget class="QComboBox" name="upload_phenotype">
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string/>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Untreated</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Treated</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Treated Sensitive</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Treated Resistant</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="4" column="0">
+                      <widget class="QLabel" name="label_41">
+                        <property name="text">
+                          <string>Phenotype</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="0">
+                      <widget class="QLabel" name="label_42">
+                        <property name="text">
+                          <string>Strain</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="1">
+                      <widget class="QComboBox" name="upload_strain">
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string/>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>MG1655</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
                   </layout>
                 </item>
               </layout>
             </widget>
             <widget class="QWidget" name="image_metadata">
               <attribute name="title">
                 <string>Image/Channel Metadata</string>
@@ -3476,78 +3738,192 @@
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="maximumSize">
               <size>
                 <width>16777215</width>
-                <height>150</height>
+                <height>500</height>
               </size>
             </property>
             <property name="currentIndex">
               <number>0</number>
             </property>
             <widget class="QWidget" name="tab_10">
               <attribute name="title">
                 <string>Database Download</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_12">
                 <item>
                   <layout class="QGridLayout" name="database_download_buttons_2">
-                    <item row="0" column="1">
-                      <widget class="QComboBox" name="download_sort_order">
+                    <item row="1" column="1">
+                      <widget class="QComboBox" name="download_sort_order_2">
                         <property name="currentIndex">
                           <number>0</number>
                         </property>
                         <item>
                           <property name="text">
+                            <string/>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
                             <string>Random</string>
                           </property>
                         </item>
                         <item>
                           <property name="text">
-                            <string>Date Uploaded (Ascending)</string>
+                            <string>Date Uploaded</string>
                           </property>
                         </item>
                         <item>
                           <property name="text">
-                            <string>Date Uploaded (Descending)</string>
+                            <string>Date Modifed</string>
                           </property>
                         </item>
                         <item>
                           <property name="text">
-                            <string>Date Modifed (Ascending)</string>
+                            <string>Image Laplacian</string>
                           </property>
                         </item>
                         <item>
                           <property name="text">
-                            <string>Date Modifed (Descending)</string>
+                            <string>Num Segmentations</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Image Focus</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Image Debris</string>
                           </property>
                         </item>
                       </widget>
                     </item>
                     <item row="0" column="0">
                       <widget class="QLabel" name="label_15">
                         <property name="text">
-                          <string>Sort Order</string>
+                          <string>Primary Sort Order</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <widget class="QComboBox" name="download_sort_direction_1">
+                        <item>
+                          <property name="text">
+                            <string/>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Ascending</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Descending</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="download_sort_order_1">
+                        <property name="currentIndex">
+                          <number>0</number>
                         </property>
+                        <item>
+                          <property name="text">
+                            <string/>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Random</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Date Uploaded</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Date Modifed</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Image Laplacian</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Num Segmentations</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Image Focus</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Image Debris</string>
+                          </property>
+                        </item>
                       </widget>
                     </item>
                     <item row="1" column="0">
+                      <widget class="QLabel" name="label_23">
+                        <property name="text">
+                          <string>Secondary Sort Order</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="2">
+                      <widget class="QComboBox" name="download_sort_direction_2">
+                        <item>
+                          <property name="text">
+                            <string/>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Ascending</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>Descending</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <layout class="QGridLayout" name="gridLayout_23">
+                    <item row="0" column="0">
                       <widget class="QLabel" name="label_88">
                         <property name="text">
                           <string>Download Limit</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="1">
+                    <item row="0" column="1">
                       <widget class="QComboBox" name="database_download_limit">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
+                        <property name="editable">
+                          <bool>true</bool>
+                        </property>
                         <property name="frame">
                           <bool>true</bool>
                         </property>
                         <item>
                           <property name="text">
                             <string>1</string>
                           </property>
@@ -3600,58 +3976,136 @@
             </widget>
             <widget class="QWidget" name="tab_4">
               <attribute name="title">
                 <string>Database Upload</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_11">
                 <item>
-                  <layout class="QGridLayout" name="database_upload_options_2">
-                    <item row="1" column="1">
-                      <widget class="QCheckBox" name="overwrite_all_metadata">
+                  <widget class="QLabel" name="label_24">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Upload Data</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QGridLayout" name="gridLayout_24">
+                    <item row="0" column="1">
+                      <widget class="QCheckBox" name="upload_segmentations_setting">
+                        <property name="text">
+                          <string>Segmentations/labels</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QCheckBox" name="upload_images_setting">
+                        <property name="text">
+                          <string>Images</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <widget class="QCheckBox" name="upload_metadata_setting">
+                        <property name="text">
+                          <string>Metadata</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_32">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Upload Settings</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QGridLayout" name="gridLayout_25">
+                    <item row="0" column="1">
+                      <widget class="QCheckBox" name="upload_overwrite_masks">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="text">
-                          <string>Overwrite All Metadata</string>
+                          <string>Overwrite Masks/Labels</string>
                         </property>
                       </widget>
                     </item>
                     <item row="0" column="0">
                       <widget class="QCheckBox" name="upload_overwrite_images">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="text">
                           <string>Overwrite Images</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="0" column="1">
-                      <widget class="QCheckBox" name="upload_overwrite_masks">
+                    <item row="1" column="0">
+                      <widget class="QCheckBox" name="overwrite_all_metadata">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="text">
-                          <string>Overwrite Masks/Labels</string>
+                          <string>Overwrite All Metadata</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="0">
+                    <item row="1" column="1">
                       <widget class="QCheckBox" name="overwrite_selected_metadata">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="text">
                           <string>Overwrite Selected Metadata</string>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </item>
                 <item>
+                  <spacer name="verticalSpacer_41">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeType">
+                      <enum>QSizePolicy::Minimum</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>435</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+                <item>
                   <layout class="QGridLayout" name="database_upload_buttons_2">
                     <item row="0" column="1">
                       <widget class="QPushButton" name="upload_all">
                         <property name="enabled">
                           <bool>true</bool>
                         </property>
                         <property name="text">
@@ -3672,30 +4126,14 @@
                   </layout>
                 </item>
               </layout>
             </widget>
           </widget>
         </item>
         <item>
-          <spacer name="verticalSpacer_30">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>435</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
           <layout class="QGridLayout" name="gridLayout_18">
             <item row="0" column="0">
               <widget class="QLabel" name="label_89">
                 <property name="text">
                   <string>Progress</string>
                 </property>
               </widget>
@@ -3716,15 +4154,15 @@
           <spacer name="verticalSpacer_4">
             <property name="orientation">
               <enum>Qt::Vertical</enum>
             </property>
             <property name="sizeHint" stdset="0">
               <size>
                 <width>20</width>
-                <height>40</height>
+                <height>20</height>
               </size>
             </property>
           </spacer>
         </item>
       </layout>
     </widget>
     <widget class="QWidget" name="export_tab">
@@ -3802,14 +4240,17 @@
                         <property name="text">
                           <string>Export Mode</string>
                         </property>
                       </widget>
                     </item>
                     <item row="2" column="1">
                       <widget class="QComboBox" name="export_location">
+                        <property name="currentIndex">
+                          <number>1</number>
+                        </property>
                         <item>
                           <property name="text">
                             <string>Import Directory</string>
                           </property>
                         </item>
                         <item>
                           <property name="text">
@@ -3922,25 +4363,46 @@
                     <item row="1" column="0">
                       <widget class="QCheckBox" name="export_autocontrast">
                         <property name="text">
                           <string>Auto Contrast</string>
                         </property>
                       </widget>
                     </item>
+                    <item row="1" column="1">
+                      <widget class="QCheckBox" name="export_normalise">
+                        <property name="text">
+                          <string>Normalise</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="0">
+                      <widget class="QCheckBox" name="export_scalebar">
+                        <property name="text">
+                          <string>Show Scale Bar</string>
+                        </property>
+                      </widget>
+                    </item>
                     <item row="1" column="2">
                       <widget class="QCheckBox" name="export_invert">
                         <property name="text">
                           <string>Invert</string>
                         </property>
                       </widget>
                     </item>
-                    <item row="1" column="1">
-                      <widget class="QCheckBox" name="export_normalise">
+                    <item row="2" column="1">
+                      <widget class="QCheckBox" name="export_mask_background">
                         <property name="text">
-                          <string>Normalise</string>
+                          <string>Mask Background</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="2">
+                      <widget class="QCheckBox" name="export_crop_zoom">
+                        <property name="text">
+                          <string>Crop to Current Zoom</string>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </item>
                 <item>
                   <spacer name="verticalSpacer_19">
@@ -4154,14 +4616,197 @@
                           <bool>true</bool>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </item>
                 <item>
+                  <spacer name="verticalSpacer_42">
+                    <property name="orientation">
+                      <enum>Qt::Vertical</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>20</width>
+                        <height>40</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_49">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Scale Bar Settings</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QGridLayout" name="gridLayout_27">
+                    <item row="0" column="2">
+                      <widget class="QComboBox" name="export_scalebar_resolution_units">
+                        <property name="maximumSize">
+                          <size>
+                            <width>200</width>
+                            <height>100</height>
+                          </size>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>nm</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>um</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_50">
+                        <property name="text">
+                          <string>Pixel Resolution</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QLineEdit" name="export_scalebar_resolution">
+                        <property name="maximumSize">
+                          <size>
+                            <width>200</width>
+                            <height>16777215</height>
+                          </size>
+                        </property>
+                        <property name="text">
+                          <string>100</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="label_55">
+                        <property name="text">
+                          <string>Scale Bar Size</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="1">
+                      <widget class="QLineEdit" name="export_scalebar_size">
+                        <property name="maximumSize">
+                          <size>
+                            <width>200</width>
+                            <height>16777215</height>
+                          </size>
+                        </property>
+                        <property name="text">
+                          <string>20</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="2">
+                      <widget class="QComboBox" name="export_scalebar_size_units">
+                        <property name="maximumSize">
+                          <size>
+                            <width>200</width>
+                            <height>100</height>
+                          </size>
+                        </property>
+                        <property name="currentIndex">
+                          <number>1</number>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>nm</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>um</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
+                  <layout class="QFormLayout" name="formLayout_19">
+                    <item row="0" column="0">
+                      <widget class="QLabel" name="label_71">
+                        <property name="text">
+                          <string>Scale Bar Colour</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <widget class="QComboBox" name="export_scalebar_colour">
+                        <item>
+                          <property name="text">
+                            <string>Black</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>White</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QLabel" name="label_72">
+                        <property name="text">
+                          <string>Scale Bar Thickness (pixels)</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="1">
+                      <widget class="QComboBox" name="export_scalebar_thickness">
+                        <property name="currentIndex">
+                          <number>3</number>
+                        </property>
+                        <item>
+                          <property name="text">
+                            <string>1</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>2</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>5</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>15</string>
+                          </property>
+                        </item>
+                        <item>
+                          <property name="text">
+                            <string>20</string>
+                          </property>
+                        </item>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
+                <item>
                   <spacer name="verticalSpacer_36">
                     <property name="orientation">
                       <enum>Qt::Vertical</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
                       <size>
                         <width>20</width>
@@ -4205,94 +4850,46 @@
             </property>
           </spacer>
         </item>
       </layout>
     </widget>
     <widget class="QWidget" name="tab_14">
       <attribute name="title">
-        <string>Misc</string>
+        <string>Utilities</string>
       </attribute>
       <layout class="QVBoxLayout" name="verticalLayout_18">
         <item>
           <widget class="Line" name="line_20">
             <property name="orientation">
               <enum>Qt::Horizontal</enum>
             </property>
           </widget>
         </item>
         <item>
-          <spacer name="verticalSpacer_26">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>20</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
           <widget class="QPushButton" name="modify_copymasktoall">
             <property name="text">
               <string>Copy Mask From Active Image to All Images</string>
             </property>
           </widget>
         </item>
         <item>
-          <spacer name="verticalSpacer_37">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>20</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
           <widget class="QPushButton" name="modify_deleteactiveimage">
             <property name="text">
               <string>Delete Active Image [Control-I]</string>
             </property>
           </widget>
         </item>
         <item>
           <widget class="QPushButton" name="modify_deleteotherimages">
             <property name="text">
               <string>Delete All Images Except Active Image [Control-Shift-I]</string>
             </property>
           </widget>
         </item>
         <item>
-          <spacer name="verticalSpacer_38">
-            <property name="orientation">
-              <enum>Qt::Vertical</enum>
-            </property>
-            <property name="sizeType">
-              <enum>QSizePolicy::Minimum</enum>
-            </property>
-            <property name="sizeHint" stdset="0">
-              <size>
-                <width>20</width>
-                <height>20</height>
-              </size>
-            </property>
-          </spacer>
-        </item>
-        <item>
           <widget class="QPushButton" name="modify_deleteactivemasks">
             <property name="text">
               <string>Delete All Masks, Active Image [Control-D]</string>
             </property>
           </widget>
         </item>
         <item>
@@ -4315,14 +4912,21 @@
                 <width>20</width>
                 <height>20</height>
               </size>
             </property>
           </spacer>
         </item>
         <item>
+          <widget class="Line" name="line_22">
+            <property name="orientation">
+              <enum>Qt::Horizontal</enum>
+            </property>
+          </widget>
+        </item>
+        <item>
           <widget class="QLabel" name="label_31">
             <property name="font">
               <font>
                 <pointsize>10</pointsize>
                 <weight>75</weight>
                 <bold>true</bold>
               </font>
@@ -4377,14 +4981,164 @@
                   <bool>true</bool>
                 </property>
               </widget>
             </item>
           </layout>
         </item>
         <item>
+          <spacer name="verticalSpacer_45">
+            <property name="orientation">
+              <enum>Qt::Vertical</enum>
+            </property>
+            <property name="sizeType">
+              <enum>QSizePolicy::Minimum</enum>
+            </property>
+            <property name="sizeHint" stdset="0">
+              <size>
+                <width>20</width>
+                <height>20</height>
+              </size>
+            </property>
+          </spacer>
+        </item>
+        <item>
+          <widget class="Line" name="line_23">
+            <property name="orientation">
+              <enum>Qt::Horizontal</enum>
+            </property>
+          </widget>
+        </item>
+        <item>
+          <widget class="QLabel" name="label_56">
+            <property name="font">
+              <font>
+                <pointsize>10</pointsize>
+                <weight>75</weight>
+                <bold>true</bold>
+              </font>
+            </property>
+            <property name="text">
+              <string>Find/Sort Cells</string>
+            </property>
+          </widget>
+        </item>
+        <item>
+          <layout class="QGridLayout" name="gridLayout_7">
+            <item row="1" column="1">
+              <widget class="QPushButton" name="find_previous">
+                <property name="text">
+                  <string>Find Previous</string>
+                </property>
+              </widget>
+            </item>
+            <item row="0" column="1">
+              <widget class="QComboBox" name="find_mode">
+                <item>
+                  <property name="text">
+                    <string>Ascending</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Descending</string>
+                  </property>
+                </item>
+              </widget>
+            </item>
+            <item row="1" column="0">
+              <widget class="QPushButton" name="find_next">
+                <property name="text">
+                  <string>Find Next</string>
+                </property>
+              </widget>
+            </item>
+            <item row="0" column="0">
+              <widget class="QComboBox" name="find_criterion">
+                <item>
+                  <property name="text">
+                    <string>Cell Area</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Cell Solidity</string>
+                  </property>
+                </item>
+                <item>
+                  <property name="text">
+                    <string>Cell Aspect Ratio</string>
+                  </property>
+                </item>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item>
+          <spacer name="verticalSpacer_46">
+            <property name="orientation">
+              <enum>Qt::Vertical</enum>
+            </property>
+            <property name="sizeType">
+              <enum>QSizePolicy::Minimum</enum>
+            </property>
+            <property name="sizeHint" stdset="0">
+              <size>
+                <width>20</width>
+                <height>20</height>
+              </size>
+            </property>
+          </spacer>
+        </item>
+        <item>
+          <widget class="QLabel" name="label_70">
+            <property name="font">
+              <font>
+                <pointsize>10</pointsize>
+                <weight>75</weight>
+                <bold>true</bold>
+              </font>
+            </property>
+            <property name="text">
+              <string>Automatic Channel Alignment/Registration</string>
+            </property>
+          </widget>
+        </item>
+        <item>
+          <layout class="QFormLayout" name="formLayout_18">
+            <item row="0" column="1">
+              <widget class="QComboBox" name="alignment_channel"/>
+            </item>
+            <item row="0" column="0">
+              <widget class="QLabel" name="label_40">
+                <property name="text">
+                  <string>Reference Channel</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item>
+          <layout class="QGridLayout" name="gridLayout_26">
+            <item row="0" column="0">
+              <widget class="QPushButton" name="align_active_image">
+                <property name="text">
+                  <string>Align Active Image</string>
+                </property>
+              </widget>
+            </item>
+            <item row="0" column="1">
+              <widget class="QPushButton" name="align_all_images">
+                <property name="text">
+                  <string>Align All Images</string>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
+        <item>
           <spacer name="verticalSpacer_13">
             <property name="orientation">
               <enum>Qt::Vertical</enum>
             </property>
             <property name="sizeHint" stdset="0">
               <size>
                 <width>20</width>
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg.egg-info/PKG-INFO` & `napari-bacseg-1.0.5/src/napari_bacseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.4/src/napari_bacseg.egg-info/SOURCES.txt` & `napari-bacseg-1.0.5/src/napari_bacseg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,32 @@
 src/_dev/akseg_dev2.py
 src/_dev/akseg_txt_metadata.py
 src/_dev/align_alex_datadump.py
 src/_dev/alison_datadump.py
 src/_dev/autocontast_dev.py
 src/_dev/cellposedev.py
 src/_dev/cellposeshapely.py
+src/_dev/chatGPT_midlines.py
+src/_dev/check_AluGasketv12_DFP.py
 src/_dev/check_metadata.py
 src/_dev/colicoords_cellldist_dev.py
 src/_dev/colicoords_ldist_dev.py
 src/_dev/database_dev.py
+src/_dev/deepsegmattest.py
 src/_dev/edit_database_columns.py
 src/_dev/fits_dev.py
 src/_dev/fix_alison_missing_file_list.py
 src/_dev/generate_scanr_movie.py
 src/_dev/get_akseg_stats.py
 src/_dev/get_species_info.py
 src/_dev/luke__script.py
 src/_dev/matplotlib_Events.py
 src/_dev/move_AluGasketDFP.py
+src/_dev/move_AluGasketDFP_poster.py
+src/_dev/move_AluGasketv12_DFP.py
 src/_dev/move_conor_nim_dfp_data.py
 src/_dev/move_pillar_data.py
 src/_dev/move_pillar_zstack_data.py
 src/_dev/move_unlearning_files.py
 src/_dev/new_metadata2.pickle.py
 src/_dev/new_read_akseg_directory.py
 src/_dev/nim_dev.py
@@ -52,14 +57,15 @@
 src/_dev/process_alex_datadump_clinical.py
 src/_dev/process_conor_datadump.py
 src/_dev/process_gramstain_datadump.py
 src/_dev/read_non_tif.py
 src/_dev/rebuild_usermeta.py
 src/_dev/rebuild_usermeta_2.py
 src/_dev/recreate_user_metadata.py
+src/_dev/scalebar_dev.py
 src/_dev/sort_midlines.py
 src/_dev/stelios_stats.py
 src/_dev/tile_meta_check.py
 src/_dev/tiler_dev.py
 src/_dev/updade_akseg_metadata.py
 src/_dev/update_img_metadata.py
 src/_dev/video_iamges.py
```

### Comparing `napari-bacseg-1.0.4/tox.ini` & `napari-bacseg-1.0.5/tox.ini`

 * *Files identical despite different names*

