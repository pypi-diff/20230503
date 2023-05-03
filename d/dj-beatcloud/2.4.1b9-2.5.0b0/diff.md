# Comparing `tmp/dj_beatcloud-2.4.1b9.tar.gz` & `tmp/dj_beatcloud-2.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b9.tar", last modified: Tue Apr 25 02:58:27 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.0b0.tar", last modified: Wed May  3 03:53:24 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b9.tar` & `dj_beatcloud-2.5.0b0.tar`

### file list

```diff
@@ -1,68 +1,73 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.594237 dj_beatcloud-2.4.1b9/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b9/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 02:22:26.000000 dj_beatcloud-2.4.1b9/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:58:27.594350 dj_beatcloud-2.4.1b9/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28208 2023-04-25 02:22:18.000000 dj_beatcloud-2.4.1b9/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.582440 dj_beatcloud-2.4.1b9/djtools/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.586050 dj_beatcloud-2.4.1b9/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      466 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4653 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.587016 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29493 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1827 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       37 2023-04-25 02:58:27.000000 dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.589712 dj_beatcloud-2.4.1b9/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1292 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4529 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1173 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1353 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2974 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5102 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1437 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3905 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.591318 dj_beatcloud-2.4.1b9/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      680 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17439 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6108 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.592623 dj_beatcloud-2.4.1b9/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      736 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8218 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4010 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8157 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4686 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/sync/test_sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-25 02:58:27.594105 dj_beatcloud-2.4.1b9/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      795 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9423 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3187 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8505 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1540 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 02:49:40.000000 dj_beatcloud-2.4.1b9/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 01:26:32.000000 dj_beatcloud-2.4.1b9/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      148 2023-04-25 02:58:27.594744 dj_beatcloud-2.4.1b9/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2233 2023-04-25 02:58:11.000000 dj_beatcloud-2.4.1b9/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.217272 dj_beatcloud-2.5.0b0/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.0b0/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2002 2023-05-03 03:53:24.217364 dj_beatcloud-2.5.0b0/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)      717 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.202279 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2002 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1872 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-05-03 03:53:24.000000 dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.203371 dj_beatcloud-2.5.0b0/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2462 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.206815 dj_beatcloud-2.5.0b0/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2815 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1213 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13431 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-03 01:35:47.000000 dj_beatcloud-2.5.0b0/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5020 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.207070 dj_beatcloud-2.5.0b0/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.210947 dj_beatcloud-2.5.0b0/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1768 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4516 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18774 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3516 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3275 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5334 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.212896 dj_beatcloud-2.5.0b0/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16576 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5977 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2151 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.214475 dj_beatcloud-2.5.0b0/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4710 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8276 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4324 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8707 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5000 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      880 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-05-03 03:53:24.216990 dj_beatcloud-2.5.0b0/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      879 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3478 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9526 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8363 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-04-25 19:26:53.000000 dj_beatcloud-2.5.0b0/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-25 19:26:48.000000 dj_beatcloud-2.5.0b0/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-05-03 03:53:24.217669 dj_beatcloud-2.5.0b0/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2223 2023-05-03 01:12:36.000000 dj_beatcloud-2.5.0b0/setup.py
```

### Comparing `dj_beatcloud-2.4.1b9/LICENSE` & `dj_beatcloud-2.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b9/djtools/configs/config.py` & `dj_beatcloud-2.5.0b0/djtools/configs/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 apply to multiple packages. The attributes of this configuration object
 correspond with the "configs" key of config.yaml."""
 import logging
 import os
 from pathlib import Path
 from typing_extensions import Literal
 
-from pydantic import BaseModel, Extra, NonNegativeInt 
+from pydantic import BaseModel, Extra, NonNegativeInt
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseConfig(BaseModel, extra=Extra.allow):
     """Base configuration object used across the whole library."""
@@ -20,22 +20,15 @@
     LOG_LEVEL: Literal[
         "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
     ] = "INFO"
     VERBOSITY: NonNegativeInt = 0
     XML_PATH: Path = None
 
     def __init__(self, *args, **kwargs):
-        """Constructor.
-        
-        Raises:
-            RuntimeError: awscli must be installed.
-            RuntimeError: AWS_PROFILE must be valid.
-            RuntimeError: SPOTIFY_CLIENT_ID, SPOTFIY_CLIENT_SECRET, and
-                SPOTIFY_REDIRECT_URI must all be valid.
-        """
+        """Constructor."""
         super().__init__(*args, **kwargs)
         logger.info(repr(self))
         if self.__class__.__name__ != "BaseConfig":
             return
 
         if not self.AWS_PROFILE:
             logger.warning(
@@ -57,22 +50,22 @@
             #     )
             # _, stderr = proc.communicate()
             # stderr = stderr.decode("utf-8").strip("\n")
             # if stderr == (
             #     f"The config profile ({self.AWS_PROFILE}) could not be found"
             # ):
             #     raise RuntimeError("AWS_PROFILE is not a valid profile!")
-        
+
         if not self.XML_PATH:
             logger.warning(
                 "XML_PATH is not set. Without this set to a valid Rekordbox "
                 "XML export, you cannot use the following features: "
-                "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
-                "REKORDBOX_PLAYLISTS, UPLOAD_XML"
+                "BUILD_PLAYLISTS, COPY_PLAYLISTS, DOWNLOAD_XML, SHUFFLE_PLAYLISTS, "
+                "UPLOAD_XML"
             )
         elif not self.XML_PATH.exists():
             logger.warning(
                 "XML_PATH does not exist. Without this set to a valid "
                 "Rekordbox XML export, you cannot use the following features: "
-                "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
-                "REKORDBOX_PLAYLISTS, UPLOAD_XML"
+                "BUILD_PLAYLISTS, COPY_PLAYLISTS, DOWNLOAD_XML, SHUFFLE_PLAYLISTS, "
+                "UPLOAD_XML"
             )
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/configs/config.yaml` & `dj_beatcloud-2.5.0b0/djtools/configs/config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 configs:
   AWS_PROFILE: 'default'
   LOG_LEVEL: INFO
   VERBOSITY: 0
   XML_PATH: ''
 rekordbox:
+  BUILD_PLAYLISTS: false
+  BUILD_PLAYLISTS_REMAINDER: folder
   COPY_PLAYLISTS: []
   COPY_PLAYLISTS_DESTINATION: ''
   PURE_GENRE_PLAYLISTS: []
-  RANDOMIZE_PLAYLISTS: []
-  REKORDBOX_PLAYLISTS: false
-  REKORDBOX_PLAYLISTS_REMAINDER: folder
+  SHUFFLE_PLAYLISTS: []
 spotify:
   AUTO_PLAYLIST_DEFAULT_LIMIT: 50
   AUTO_PLAYLIST_DEFAULT_PERIOD: week
   AUTO_PLAYLIST_DEFAULT_TYPE: hot
   AUTO_PLAYLIST_FUZZ_RATIO: 70
   AUTO_PLAYLIST_POST_LIMIT: 100
   AUTO_PLAYLIST_SUBREDDITS: []
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/configs/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/configs/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module is responible for building this library's configuration objects
+"""This module is responsible for building this library's configuration objects
 using config.yaml. If command-line arguments are provided, this module
 overrides the corresponding configuration options with these arguments.
 """
 import argparse
 from argparse import ArgumentParser
 import logging
 from pathlib import Path
@@ -87,14 +87,28 @@
         help=(
             'Drop --size-only flag for "aws s3 sync" command; '
             '"--aws-use-date-modified" will permit re-downloading/'
             "re-uploading files if the date modified field changes"
         ),
     )
     parser.add_argument(
+        "--build-playlists",
+        action="store_true",
+        help="Trigger automatic Rekordbox playlist creation",
+    )
+    parser.add_argument(
+        "--build-playlists-remainder",
+        type=str,
+        choices=["folder", "playlist"],
+        help=(
+            'Place remainder tracks in either an "Other" folder of playlists '
+            'or a single "Other" playlist'
+        ),
+    )
+    parser.add_argument(
         "--check-tracks",
         action="store_true",
         help=(
             "Trigger checking for track overlap between the Beatcloud and"
             "CHECK_TRACKS_LOCAL_DIRS and / or CHECK_TRACKS_SPOTIFY_PLAYLISTS"
         ),
     )
@@ -193,20 +207,14 @@
     parser.add_argument(
         "--pure-genre-playlists",
         type=str,
         nargs="+",
         help='List of genre tag substrings to create "pure" playlists for',
     )
     parser.add_argument(
-        "--randomize-playlists",
-        type=str,
-        nargs="+",
-        help="List of Rekordbox playlist names to randomize tracks in",
-    )
-    parser.add_argument(
         "--reddit-client-id",
         type=str,
         help="Reddit API client ID",
     )
     parser.add_argument(
         "--reddit-client-secret",
         type=str,
@@ -214,26 +222,18 @@
     )
     parser.add_argument(
         "--reddit-user-agent",
         type=str,
         help="Reddit API user agent",
     )
     parser.add_argument(
-        "--rekordbox-playlists",
-        action="store_true",
-        help="Trigger automatic Rekordbox playlist creation",
-    )
-    parser.add_argument(
-        "--rekordbox-playlists-remainder",
+        "--shuffle-playlists",
         type=str,
-        choices=["folder", "playlist"],
-        help=(
-            'Place remainder tracks in either an "Other" folder of playlists '
-            'or a single "Other" playlist'
-        ),
+        nargs="+",
+        help="List of Rekordbox playlist names to randomize tracks in",
     )
     parser.add_argument(
         "--spotify-client-id",
         type=str,
         help="Spotify API client ID",
     )
     parser.add_argument(
@@ -327,15 +327,15 @@
         package_root = Path(__file__).parent.parent
         configs_dir = package_root / "configs"
         args.link_configs.symlink_to(configs_dir, target_is_directory=True)
 
     return vars(args)
 
 
-def build_config():
+def build_config() -> BaseConfig:
     """This function loads configurations for the library.
     
     Configurations are loaded from config.yaml. If command-line arguments are
     provided, these override the configuration options set in config.yaml.
 
     Raises:
         RuntimeError: config.yaml must be a valid YAML.
@@ -428,15 +428,15 @@
     """
     super_keys = set(BaseConfig.__fields__)
     return {
         k: v for k, v in sub_config.dict().items() if k not in super_keys
     }
 
 
-def parse_yaml(_yaml: str):
+def parse_yaml(_yaml: str) -> Dict:
     """Parses a YAML string and returns a YAML object.
 
     Args:
         _yaml: String representing YAML.
 
     Raises:
         Exception: YAML string must be valid YAML.
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.0b0/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b9/djtools/configs/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/configs/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from subprocess import PIPE
-from unittest import mock
-
-import pytest
-
+"""Testing for the config module."""
 from djtools.configs.config import BaseConfig
 
 
 def test_baseconfig_aws_profile():
+    """Test for the BaseConfig class."""
     BaseConfig()
 
 
 def test_baseconfig_aws_profile_not_set(caplog):
+    """Test for the BaseConfig class."""
     caplog.set_level("WARNING")
     cfg = {"AWS_PROFILE": ""}
     BaseConfig(**cfg)
     assert caplog.records[0].message == (
         "Without AWS_PROFILE set to a valid profile ('default' or otherwise) "
         "you cannot use any of the following features: CHECK_TRACKS, "
         "DOWNLOAD_MUSIC, DOWNLOAD_XML, UPLOAD_MUSIC, UPLOAD_XML"
@@ -25,51 +23,53 @@
 # def test_baseconfig_aws_profile_invalid():
 #     cfg = {"AWS_PROFILE": "definitely not a real AWS profile"}
 #     with pytest.raises(
 #         RuntimeError, match="AWS_PROFILE is not a valid profile!"
 #     ):
 #         BaseConfig(**cfg)
 
- 
+
 # @mock.patch("djtools.configs.config.Popen", side_effect=Exception())
 # def test_baseconfig_awscli_not_installed(mock_popen):
 #     cfg = {"AWS_PROFILE": "definitely not a real AWS profile"}
 #     with pytest.raises(
 #         RuntimeError,
 #         match=(
 #             "Failed to run AWS command; make sure you've installed awscli "
 #             "correctly."
 #         )
 #     ):
 #         BaseConfig(**cfg)
 
 
 def test_baseconfig_no_xml_path(caplog):
+    """Test for the BaseConfig class."""
     caplog.set_level("WARNING")
     cfg = {
         "AWS_PROFILE": "default",
         "SPOTIFY_CLIENT_ID": "",
         "XML_PATH": None,
     }
     BaseConfig(**cfg)
     assert caplog.records[0].message == (
         "XML_PATH is not set. Without this set to a valid Rekordbox XML "
         "export, you cannot use the following features: "
-        "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
-        "REKORDBOX_PLAYLISTS, UPLOAD_XML"
+        "BUILD_PLAYLISTS, COPY_PLAYLISTS, DOWNLOAD_XML, SHUFFLE_PLAYLISTS, "
+        "UPLOAD_XML"
     )
 
 
 def test_baseconfig_xml_path_does_not_exist(caplog):
+    """Test for the BaseConfig class."""
     caplog.set_level("WARNING")
     cfg = {
         "AWS_PROFILE": "default",
         "SPOTIFY_CLIENT_ID": "",
         "XML_PATH": "nonexistent XML",
     }
     BaseConfig(**cfg)
     assert caplog.records[0].message == (
         "XML_PATH does not exist. Without this set to a valid "
         "Rekordbox XML export, you cannot use the following features: "
-        "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
-        "REKORDBOX_PLAYLISTS, UPLOAD_XML"
+        "BUILD_PLAYLISTS, COPY_PLAYLISTS, DOWNLOAD_XML, SHUFFLE_PLAYLISTS, "\
+        "UPLOAD_XML"
     )
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/configs/test_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,80 @@
+"""Testing for the helpers module."""
 from argparse import Namespace
 from pathlib import Path
 import re
 from typing import List
 from unittest import mock
 
 import pytest
 
-from djtools.configs.config import BaseConfig
 from djtools.configs.helpers import (
-    arg_parse, build_config, convert_to_paths, filter_dict, parse_yaml, pkg_cfg
+    arg_parse,
+    BaseConfig,
+    build_config,
+    convert_to_paths,
+    filter_dict,
+    parse_yaml,
+    pkg_cfg,
 )
 from djtools.utils.helpers import MockOpen
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs(mock_parse_args, tmpdir):
+    """Test for the arg_parse function."""
     config_path = Path(tmpdir) / "test_dir"
     mock_parse_args.return_value = Namespace(
         link_configs=config_path, log_level="INFO"
     )
-    args = arg_parse()
+    arg_parse()
     assert config_path.is_symlink()
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs_dir_does_exist(mock_parse_args, tmpdir):
+    """Test for the arg_parse function."""
     link_path = Path(tmpdir) / "new_dir" / "link_dir"
     mock_parse_args.return_value = Namespace(
         link_configs=link_path, log_level="INFO"
     )
-    args = arg_parse()
+    arg_parse()
     assert link_path.exists()
     assert link_path.is_symlink()
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs_dir_does_not_exist(mock_parse_args, tmpdir):
+    """Test for the arg_parse function."""
     link_path = str(tmpdir)
     mock_parse_args.return_value = Namespace(
         link_configs=link_path, log_level="INFO"
     )
     with pytest.raises(
         ValueError,
         # NOTE(a-rich): WindowsPath needs to be escaped for `\` characters to
         # appear in the `match` argument.
         match=re.escape(
             f'{link_path} must be a directory that does not already exist'
         ),
     ):
-        args = arg_parse()
+        arg_parse()
 
 
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
 @mock.patch(
     "builtins.open",
     MockOpen(
         files=["registered_users.yaml"],
         user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
         user_b=("other_user", "/other/USB/"),
     ).open,
 )
-def test_build_config(mock_get_spotify_client, tmpdir):
+def test_build_config():
+    """Test for the build_config function."""
     with mock.patch(
         "argparse.ArgumentParser.parse_args",
     ) as mock_parse_args:
         mock_parse_args.return_value = Namespace(
             link_configs="", log_level="INFO"
         )
         config = build_config()
@@ -72,75 +82,81 @@
 
 
 @mock.patch("builtins.open", MockOpen(
     files=["config.yaml"],
     content="yaml_valid: {false",
 ).open)
 def test_build_config_invalid_config_yaml(caplog):
+    """Test for the build_config function."""
     caplog.set_level("CRITICAL")
-    with pytest.raises(RuntimeError) as exc:
-        config = build_config()
+    with pytest.raises(RuntimeError):
+        build_config()
     assert 'Error reading "config.yaml"' in caplog.records[0].message
 
 
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
 @mock.patch(
     "builtins.open",
     MockOpen(
         files=["registered_users.yaml", "config.yaml"],
         user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
         user_b=("test_user", "/test/USB/"),
     ).open
 )
 @mock.patch("argparse.ArgumentParser.parse_args")
-def test_build_config_no_config_yaml(mock_parse_args, mock_spotify_client):
+def test_build_config_no_config_yaml(mock_parse_args):
+    """Test for the build_config function."""
     mock_parse_args.return_value = Namespace(
         link_configs="", log_level="INFO"
     )
     config_dir = Path(__file__).parent.parent / "configs"
     config_file = config_dir / "config.yaml"
     with mock.patch.object(Path, "exists", return_value=False):
         assert not config_file.exists()
-        config = build_config()
+        build_config()
     assert config_file.exists()
 
 
 @pytest.mark.parametrize("paths", ["path", ["path1", "path2"]])
 def test_convert_to_paths(paths):
+    """Test for the convert_to_paths function."""
     paths = convert_to_paths(paths)
     if isinstance(paths, List):
         for path in paths:
             assert isinstance(path, Path)
     else:
         assert isinstance(paths, Path)
 
 
-@pytest.mark.parametrize("config", [cfg for cfg in pkg_cfg.values()])
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
+@pytest.mark.parametrize("config", pkg_cfg.values())
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
 @mock.patch(
     "builtins.open",
     MockOpen(files=["registered_users.yaml"], write_only=True).open
 )
-def test_filter_dict(mock_get_spotify_client, config):
+def test_filter_dict(config):
+    """Test for the filter_dict function."""
     super_config = BaseConfig()
     sub_config = config(**dict(super_config))
     result = filter_dict(sub_config)
     super_keys = set(super_config.dict())
     sub_keys = set(sub_config.dict())
     result_keys = set(result)
     assert len(result_keys) + len(super_keys) == len(sub_keys)
     assert result_keys.union(super_keys) == sub_keys
     assert sub_keys.difference(result_keys) == super_keys
     assert sub_keys.difference(super_keys) == result_keys
 
 
 def test_parse_yaml():
+    """Test for the parse_yaml function."""
     yaml_string = "name:\n - stuff"
     yaml_obj = parse_yaml(yaml_string)
     assert isinstance(yaml_obj, dict)
     assert isinstance(yaml_obj["name"], list)
 
 
 def test_parse_yaml_invalid():
+    """Test for the parse_yaml function."""
     yaml_string = "name:\n\t - stuff"
     with pytest.raises(ValueError):
-        yaml_obj = parse_yaml(yaml_string)
+        parse_yaml(yaml_string)
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.0b0/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-djtools/configs/README.md
+dj_beatcloud.egg-info/PKG-INFO
+dj_beatcloud.egg-info/SOURCES.txt
+dj_beatcloud.egg-info/dependency_links.txt
+dj_beatcloud.egg-info/entry_points.txt
+dj_beatcloud.egg-info/requires.txt
+dj_beatcloud.egg-info/top_level.txt
+djtools/__init__.py
+djtools/__main__.py
+djtools/test_main.py
 djtools/configs/__init__.py
 djtools/configs/config.py
 djtools/configs/config.yaml
 djtools/configs/helpers.py
 djtools/configs/logging.conf
 djtools/configs/registered_users.yaml
 djtools/configs/rekordbox_playlists.yaml
 djtools/configs/spotify_playlists.yaml
 djtools/configs/test_config.py
 djtools/configs/test_helpers.py
-djtools/dj_beatcloud.egg-info/PKG-INFO
-djtools/dj_beatcloud.egg-info/SOURCES.txt
-djtools/dj_beatcloud.egg-info/dependency_links.txt
-djtools/dj_beatcloud.egg-info/entry_points.txt
-djtools/dj_beatcloud.egg-info/requires.txt
-djtools/dj_beatcloud.egg-info/top_level.txt
+djtools/logs/empty.txt
 djtools/rekordbox/__init__.py
 djtools/rekordbox/config.py
 djtools/rekordbox/copy_playlists.py
 djtools/rekordbox/helpers.py
 djtools/rekordbox/playlist_builder.py
-djtools/rekordbox/randomize_playlists.py
+djtools/rekordbox/playlist_combiner.py
+djtools/rekordbox/shuffle_playlists.py
 djtools/rekordbox/tag_parsers.py
 djtools/rekordbox/test_config.py
 djtools/rekordbox/test_copy_playlists.py
 djtools/rekordbox/test_helpers.py
 djtools/rekordbox/test_playlist_builder.py
-djtools/rekordbox/test_randomize_playlists.py
+djtools/rekordbox/test_shuffle_playlists.py
 djtools/rekordbox/test_tag_parsers.py
 djtools/spotify/__init__.py
 djtools/spotify/config.py
 djtools/spotify/helpers.py
 djtools/spotify/playlist_builder.py
 djtools/spotify/test_config.py
 djtools/spotify/test_helpers.py
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,32 @@
         playlists to a new location and writes a new XML with these updated
         paths
     * `helpers`: contains helper classes and functions for the other modules of
         this package
     * `playlist_builder`: constructs rekordbox playlists using tags in a
         Collection and a defined playlist structure in
         `rekordbox_playlists.yaml`
-    * `randomize_playlists`: writes sequential numbers to Rekordbox tags of
+    * `shuffle_playlists`: writes sequential numbers to Rekordbox tags of
         shuffled tracks in playlists to emulate playlist shuffling
     * `tag_parsers`: the `TagParser` abstract base class and its
         implementations used by the `playlist_builder`
 """
 
-from .config import RekordboxConfig
-from .copy_playlists import copy_playlists
-from .playlist_builder import rekordbox_playlists
-from .randomize_playlists import randomize_playlists
+from djtools.rekordbox.config import RekordboxConfig
+from djtools.rekordbox.copy_playlists import copy_playlists
+from djtools.rekordbox.playlist_builder import build_playlists
+from djtools.rekordbox.shuffle_playlists import shuffle_playlists
 
 
 REKORDBOX_OPERATIONS = {
+    "BUILD_PLAYLISTS": build_playlists,
     "COPY_PLAYLISTS": copy_playlists,
-    "RANDOMIZE_PLAYLISTS": randomize_playlists,
-    "REKORDBOX_PLAYLISTS": rekordbox_playlists
+    "SHUFFLE_PLAYLISTS": shuffle_playlists,
 }
 
 __all__ = (
+    "build_playlists",
     "copy_playlists",
-    "randomize_playlists",
+    "shuffle_playlists",
     "RekordboxConfig",
     "REKORDBOX_OPERATIONS",
-    "rekordbox_playlists",
 )
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 """This module contains the configuration object for the rekordbox package.
 The attributes of this configuration object correspond with the "rekordbox" key
 of config.yaml
 """
 import logging
 from pathlib import Path
-from typing import List 
+from typing import List
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 class RekordboxConfig(BaseConfig):
     """Configuration object for the rekordbox package."""
 
+    BUILD_PLAYLISTS: bool = False
+    BUILD_PLAYLISTS_REMAINDER: str = "folder"
     COPY_PLAYLISTS:  List[str] = []
     COPY_PLAYLISTS_DESTINATION: Path = None
     PURE_GENRE_PLAYLISTS:  List[str] = []
-    RANDOMIZE_PLAYLISTS:  List[str] = []
-    REKORDBOX_PLAYLISTS: bool = False 
-    REKORDBOX_PLAYLISTS_REMAINDER: str = "folder"
+    SHUFFLE_PLAYLISTS:  List[str] = []
 
     def __init__(self, *args, **kwargs):
         """Constructor.
         
         Raises:
             RuntimeError: XML_PATH must be a valid rekordbox XML file.
             RuntimeError: rekordbox_playlists.yaml must be a valid YAML file.
         """
         super().__init__(*args, **kwargs)
 
         if any(
             [
+                self.BUILD_PLAYLISTS,
                 self.COPY_PLAYLISTS,
-                self.RANDOMIZE_PLAYLISTS,
-                self.REKORDBOX_PLAYLISTS,
+                self.SHUFFLE_PLAYLISTS,
             ]
         ) and (not self.XML_PATH or not self.XML_PATH.exists()):
             raise RuntimeError(
                 "Using the rekordbox package requires the config option "
                 "XML_PATH to be a valid rekordbox XML file"
             )
 
-        if self.REKORDBOX_PLAYLISTS:
+        if self.BUILD_PLAYLISTS:
             playlist_config = (
                 Path(__file__).parent.parent / "configs" /
                 "rekordbox_playlists.yaml"
             )
             if not playlist_config.exists():
                 raise RuntimeError(
                     "rekordbox_playlists.yaml must be a valid YAML to use the "
-                    "REKORDBOX_PLAYLISTS feature"
+                    "BUILD_PLAYLISTS feature"
                 )
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/copy_playlists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module is used to copy the audio files from the provided playlists to a
 new location and write a new XML database with those tracks pointing to these
 new locations.
 
 The purpose of this utility is to:
-    * backup subsets of your library
-    * ensure you have easy access to a preparation on non-Pioneer setups
+
+* backup subsets of your library
+* ensure you have easy access to a preparation on non-Pioneer setups
 """
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 import os
 
 from bs4 import BeautifulSoup
 from tqdm import tqdm
@@ -26,15 +27,15 @@
         config: Configuration object.
 
     Raises:
         LookupError: Playlist names in COPY_PLAYLISTS must exist in
             "XML_PATH".
     """
     # Load Rekordbox database from XML.
-    with open(config.XML_PATH, mode="r", encoding="utf-8") as _file:	
+    with open(config.XML_PATH, mode="r", encoding="utf-8") as _file:
         rekordbox_database = BeautifulSoup(_file.read(), "xml")
 
     # Create destination directory.
     config.COPY_PLAYLISTS_DESTINATION.mkdir(parents=True, exist_ok=True)
 
     # Nodes to not remove when writing the new XML.
     keep_nodes = set()
@@ -50,31 +51,31 @@
             keep_nodes.update([playlist_name])
             next_playlist = playlist
             while next_playlist.parent:
                 next_playlist = next_playlist.parent
                 if not next_playlist.attrs:
                     break
                 keep_nodes.add(next_playlist.attrs["Name"])
-        except IndexError:
-            raise LookupError(f"{playlist_name} not found")
+        except IndexError as exc:
+            raise LookupError(f"{playlist_name} not found") from exc
         playlists_track_keys[playlist_name].update(
             {track["Key"] for track in playlist.children if str(track).strip()}
         )
     flattened_track_keys = {
         track_key for track_keys in playlists_track_keys.values()
         for track_key in track_keys
     }
 
     # Get the map of track IDs to their TRACK nodes.
     # Decompose tracks that aren't in the provided playlists.
     tracks = {}
     for track in rekordbox_database.find_all("TRACK"):
         if (
             not track.get("Location")
-            or track["TrackID"] not in flattened_track_keys 
+            or track["TrackID"] not in flattened_track_keys
         ):
             track.decompose()
         else:
             tracks[track["TrackID"]] = track
 
     # Copy tracks to the destination and update Location for the track.
     payload = [
@@ -93,22 +94,22 @@
     # Decompose irrelevant playlists.
     playlists_root = rekordbox_database.find_all(
         "NODE", {"Name": "ROOT", "Type": "0"}
     )[0]
     for node in playlists_root.find_all("NODE"):
         if node.attrs and node.attrs["Name"] not in keep_nodes:
             node.decompose()
-    
+
     # Repopulate playlists with relocated tracks.
     for playlist_name in config.COPY_PLAYLISTS:
         playlist = rekordbox_database.find_all(
             "NODE", {"Name": playlist_name}
         )[0]
         for track_id in playlists_track_keys[playlist_name]:
             playlist.append(rekordbox_database.new_tag("TRACK", Key=track_id))
-    
+
     # Write new XML.
-    new_db = config.XML_PATH.parent / f"relocated_{config.XML_PATH.name}"
+    new_db = config.XML_PATH.parent / f"auto_{config.XML_PATH.name}"
     with open(
         new_db, mode="wb", encoding=rekordbox_database.original_encoding,
     ) as _file:
         _file.write(rekordbox_database.prettify("utf-8"))
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """This module contains helpers for the rekordbox package."""
 from pathlib import Path
 import re
 import shutil
-from typing import Any, Dict, List, Optional, Set, Tuple 
-from urllib.parse import quote, unquote
+from typing import Any, Dict, List, Optional, Set, Tuple
+from urllib.parse import unquote
 
 import bs4
 from bs4 import BeautifulSoup
 
 
 class BooleanNode:
-    """Node that contains boolean logic for a subexpression."""
+    """Node that contains boolean logic for a sub-expression."""
 
     def __init__(self, parent: Optional[Any] = None):
         """Constructor.
 
         Args:
-            parent: BooleanNode of which this node is a subexpression.
+            parent: BooleanNode of which this node is a sub-expression.
         """
         self.parent = parent
         self.operators = []
         self.tags = []
         self.tracks = []
-    
+
     def __call__(
         self, tracks: Dict[str, List[Tuple[str, List[str]]]]
     ) -> Set[str]:
-        """Evaluates the boolean algebraic subexpression.
+        """Evaluates the boolean algebraic sub-expression.
 
         Args:
             tracks: Map of tags to dicts of track_id: tags.
 
         Raises:
             RuntimeError: Boolean expressions must be formatted correctly.
 
@@ -43,55 +43,55 @@
             raise RuntimeError(
                 f"Invalid boolean expression: track sets: {len(self.tracks)}, "
                 f"tags: {self.tags}, operators: "
                 f"{[x.__name__ for x in self.operators]}"
             )
         while self.tags or self.operators:
             operator = self.operators.pop(0)
-            if len(self.tracks):
-                tracks_A = self.tracks.pop(0)
+            if self.tracks:
+                tracks_set_a = self.tracks.pop(0)
             else:
-                tracks_A = self._get_tag_tracks(
+                tracks_set_a = self._get_tag_tracks(
                     tag=self.tags.pop(0), tracks=tracks
                 )
-            if len(self.tracks):
-                tracks_B = self.tracks.pop(0)
+            if self.tracks:
+                tracks_set_b = self.tracks.pop(0)
             else:
-                tracks_B = self._get_tag_tracks(
+                tracks_set_b = self._get_tag_tracks(
                     tag=self.tags.pop(0), tracks=tracks
                 )
-            self.tracks.insert(0, operator(tracks_A, tracks_B))
-        
+            self.tracks.insert(0, operator(tracks_set_a, tracks_set_b))
+
         return next(iter(self.tracks), set())
 
     def _get_tag_tracks(
         self, tag: str, tracks: Dict[str, List[Tuple[str, List[str]]]]
     ) -> Set[str]:
         """Gets set of track IDs for the provided tag.
 
         If the tag contains a wildcard, denoted with "*", then the union of
-        track IDs with a tag containing the provided tag as a substring is
+        track IDs with a tag containing the provided tag as a sub-string is
         returned.
 
         Args:
             tag: Tag for indexing tracks.
             tracks: Map of tags to dicts of track_id: tags.
 
         Returns:
             Set of track IDs for the provided tag.
         """
         if "*" in tag:
             exp = re.compile(r".*".join(tag.split("*")))
             track_ids = set()
-            for k in tracks:
-                if re.search(exp, k):
-                    track_ids.update(set(tracks[k].keys()))
+            for key in tracks:
+                if re.search(exp, key):
+                    track_ids.update(set(tracks[key].keys()))
             return track_ids
-        else:
-            return set(tracks.get(tag, {}).keys())
+
+        return set(tracks.get(tag, {}).keys())
 
 
 def copy_file(
     track: bs4.element.Tag,
     destination: Path,
     loc_prefix: str="file://localhost",
 ):
@@ -104,15 +104,15 @@
     """
     loc = Path(unquote(track["Location"]).split(loc_prefix)[-1])
     new_loc = Path(destination / loc.name).as_posix()
     shutil.copyfile(loc.as_posix(), new_loc)
     track["Location"] = f"{loc_prefix}{new_loc}"
 
 
-def get_playlist_track_locations(
+def get_playlist_tracks(
     soup: BeautifulSoup, _playlist: str, seen_tracks: Set[str]
 ) -> List[str]:
     """Finds playlist in "XML_PATH" that matches "_playlist" and returns a list
         of the track nodes in that playlist that aren't in "seen_tracks".
 
     Args:
         soup: Parsed XML.
@@ -135,15 +135,15 @@
         if str(track).strip() and track["Key"] not in seen_tracks
     ]
     seen_tracks.update(playlist_tracks)
 
     return playlist_tracks
 
 
-def set_tag(track: str, index: int):
+def set_track_number(track: str, index: int):
     """Threaded process to set TRACK node's TrackNumber tag.
 
     Args:
         track: TRACK node.
         index: New TrackNumber.
     """
     track["TrackNumber"] = index
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 """This module is used to automatically generate a playlist structure using
 genre tags and the "My Tags" Rekordbox feature. It also supports creating
 "Combiner" playlists with arbitrary boolean algebra using:
-    * "(" and ")" groupings
-    * "&", "|", and "~" operators
-    * playlist selectors, e.g. "{My favorite playlist}"
-    * BPM selectors, e.g. "[80-90, 140, 165-174]"
-    * Rating selectors, e.g. "[1, 2-4"
-    * tag names (genre or "My Tags")
+
+* "(" and ")" groupings
+* "&", "|", and "~" operators
+* playlist selectors, e.g. "{My favorite playlist}"
+* BPM selectors, e.g. "[80-90, 140, 165-174]"
+* Rating selectors, e.g. "[1, 2-4"
+* tag names (genre or "My Tags")
 
 NOTE: In order for "My Tags" to be stored in the exported XML files, users must
 enable the 'Add "My Tag" to the "Comments"' setting under
 "Preferences > Advanced > Browse".
 """
 from collections import defaultdict
 import logging
 from pathlib import Path
-from typing import Dict, List, Set, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 
 import bs4
 from bs4 import BeautifulSoup
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.rekordbox import tag_parsers
-from djtools.rekordbox.tag_parsers import Combiner
+from djtools.rekordbox.playlist_combiner import Combiner
 
 
 logger = logging.getLogger(__name__)
 
 
 class PlaylistBuilder:
     """This class writes an XML Rekordbox database with auto-playlists.
     
     The XML written by this class  will contain auto-generated playlists using
     configurations found in "rekordbox_playlists.yaml".
 
     The "rekordbox_playlists.yaml" configuration file maps implemented
     TagParsers to a playlist taxonomy. Currently supported TagParsers are:
-        * GenreTagParser: reads "Genre" field of tracks and creates a list of
-            tags splitting on "/" characters. 
-        * MyTagParser: reads "Comments" field of tracks and searches for the
-            regex pattern /* tag_1 / tag_2 / tag_3 */
-            and creates a list of tags splitting on "/" characters.
+
+    * GenreTagParser: reads "Genre" field of tracks and creates a list of tags
+        splitting on "/" characters. 
+    * MyTagParser: reads "Comments" field of tracks and searches for the regex
+        pattern /* tag_1 / tag_2 / tag_3 */ and creates a list of tags
+        splitting on "/" characters.
     
     A "rekordbox_playlists.yaml" configuration file may also contain a
     "Combiner" key which is distinct from a TagParser implementation.
     Rather than parse tags, this class accepts the constructed tag -> track
     mapping and applies boolean algebra to create playlists using operators:
-        * AND (designated with "&"): result set will contain tracks having both tags.
-        * OR (designated with "|"): result set will contain tracks having either tag.
-        * NOT (designated with "~"): result set will not contain tracks having this tag.
-        * "()": encloses a grouping of operators which are evaluated first.
-        * "{}": encloses a playlist name to select those tracks. 
-        * "[]": encloses a comma-delimited list of integers representing
-            ratings (1 through 5) or BPMs (numbers greater than 5); ranges can
-            be specified by separating two integers with a dash.
+
+    * AND (designated with "&"): result set will contain tracks having both tags.
+    * OR (designated with "|"): result set will contain tracks having either tag.
+    * NOT (designated with "~"): result set will not contain tracks having this tag.
+    * "()": encloses a grouping of operators which are evaluated first.
+    * "{}": encloses a playlist name to select those tracks. 
+    * "[]": encloses a comma-delimited list of integers representing
+        ratings (1 through 5) or BPMs (numbers greater than 5); ranges can
+        be specified by separating two integers with a dash.
     """
     def __init__(
         self,
         rekordbox_database: Path,
         playlist_config: Path,
-        pure_genre_playlists: List[str] = [],
+        pure_genre_playlists: Optional[List[str]] = None,
         playlist_remainder_type: str = "",
     ):
         """Constructor.
 
         Args:
             rekordbox_database: Path to Rekordbox XML.
             playlist_config: Playlist taxonomy.
@@ -100,104 +103,106 @@
         with open(playlist_config, mode="r", encoding="utf-8") as _file:
             self._playlist_config = (
                 yaml.load(_file, Loader=yaml.FullLoader) or {}
             )
         self._parsers = {}
         self._combiner_parser = None
         for playlist_type, config in self._playlist_config.items():
+            if playlist_type == "Combiner":
+                self._combiner_parser = Combiner(
+                    parser_config=config,
+                    rekordbox_database=self._database,
+                )
+                continue
+
             try:
                 parser = getattr(tag_parsers, playlist_type)
-            except AttributeError:
+            except AttributeError as exc:
                 raise AttributeError(
                     f"{playlist_type} is not a valid TagParser!"
-                )
+                ) from exc
 
             parser = parser(
                 parser_config=config,
                 pure_genre_playlists=pure_genre_playlists,
                 rekordbox_database=self._database,
             )
 
-            # "Combiner" class used to assemble playlists by applying
-            # boolean algebra to tags.
-            if isinstance(parser, Combiner):
-                self._combiner_parser = parser
-                continue
-
             self._parsers[playlist_type] = parser
 
     def __call__(self):
         """Generates auto-playlists by:
-            * creating playlists nodes
-            * generating tags -> tracks mapping
-            * inserting tags to the appropriate playlist nodes for "Genre" and
-                "My Tags" playlists
-            * applying "Combiner" boolean algebra to tags
-            * writting new XML database
+
+        * creating playlists nodes
+        * generating tags -> tracks mapping
+        * inserting tags to the appropriate playlist nodes for "Genre" and
+            "My Tags" playlists
+        * applying "Combiner" boolean algebra to tags
+        * writing new XML database
         """
         tracks = {k: defaultdict(list) for k in self._parsers}
-        playlists = {} 
+        playlists = {}
         for track in self._database.find_all("TRACK"):
             if not track.get("Location"):
                 continue
             for playlist_type, parser in self._parsers.items():
                 # Initialize each type of playlist with a node and tag set.
                 if playlist_type not in playlists:
                     tag_set = set()
                     playlists[playlist_type] = {
                         "tags": tag_set,
                         "playlists": self._create_playlists(
                             soup=self._database,
                             content=parser.parser_config,
                             tags=tag_set,
                             top_level=True,
-                        ) 
+                        )
                     }
 
                 # Create tags -> tracks map.
                 tags = parser(track)
                 for tag in tags:
                     tracks[playlist_type][tag].append((track["TrackID"], tags))
-        
+
         # Add tracks to their respective playlists.
         for playlist_type, playlist_data in playlists.items():
             if self._playlist_remainder_type:
                 # Insert tracks otherwise not captured by the configuration's
                 # playlist taxonomy into "Other" groupings.
                 self._add_other(
                     soup=self._database,
                     remainder_type= self._playlist_remainder_type,
                     tags=playlist_data["tags"],
                     tracks=tracks[playlist_type],
                     playlists=playlist_data["playlists"],
                 )
-            
+
             # Insert tracks into their respective playlists.
             self._add_tracks(
                 soup=self._database,
                 playlists=playlist_data["playlists"],
                 tracks=tracks[playlist_type],
             )
-            
+
             # Insert playlist node into the playlist root.
             self._auto_playlists_root.insert(0, playlist_data["playlists"])
-        
+
         if self._combiner_parser:
             # Create Combiner playlist structure.
             combiner_playlists = self._create_playlists(
                 soup=self._database,
                 content=self._combiner_parser.parser_config,
                 top_level=True,
-            ) 
+            )
 
             # Reduce track tags across parsers unioning when there is overlap.
             merged_tracks = defaultdict(list)
             for values in tracks.values():
-                for k, v in values.items():
-                    merged_tracks[k].extend(v)
+                for key, value in values.items():
+                    merged_tracks[key].extend(value)
 
             # Use the most up-to-date Rekordbox database to update the track
             # lookup with playlist selectors to their component tracks.
             playlist_mapping = self._combiner_parser.get_playlist_mapping(
                 self._auto_playlists_root
             )
             merged_tracks.update(playlist_mapping)
@@ -215,15 +220,15 @@
             # Insert playlist node into the playlist root.
             self._auto_playlists_root.insert(0, combiner_playlists)
 
         # Decompose irrelevant playlists.
         for node in self._playlists_root.find_all("NODE"):
             if node.attrs and node.attrs["Name"] != "ROOT":
                 node.decompose()
-        
+
         # Insert the auto-playlists into the playlists root.
         self._playlists_root.insert(0, self._auto_playlists_root)
 
         # Write XML file.
         _dir = self._database_path.parent
         _file = self._database_path.name
         auto_xml_path = _dir / f"auto_{_file}"
@@ -359,20 +364,20 @@
 
                         if track_id not in seen[_seen_index]:
                             _all.append(soup.new_tag("TRACK", Key=track_id))
                             seen[_seen_index].add(track_id)
                     except IndexError:
                         break
                     parent = parent.parent
-            
+
     def _create_playlists(
         self,
         soup: BeautifulSoup,
         content: Union[str, Dict],
-        tags: Set[str] = set(),
+        tags: Optional[Set[str]] = None,
         top_level: bool = False,
     ) -> bs4.element.Tag:
         """Recursively traverses "rekordbox_playlists.yaml" and creates the
             corresponding XML tag structure to be populated with tracks. If a
             folder is encountered, an additional playlist is created called
             "All <folder name>" (this does not apply to the top-level folder). If a
             folder named "_ignore" is encountered, tag playlists specified in the
@@ -389,54 +394,55 @@
 
         Raises:
             ValueError: "rekordbox_playlists.yaml" must be properly formatted.
 
         Returns:
             Populated playlist structure.
         """
+        node = None
+        tags = tags or set()
         if isinstance(content, dict):
             content = {k.lower(): v for k, v in content.items()}
             if content["name"] == "_ignore":
                 tags.update(set(content["playlists"]))
             else:
-                folder = soup.new_tag("NODE", Name=content["name"], Type="0")
+                node = soup.new_tag("NODE", Name=content["name"], Type="0")
                 if not top_level:
                     _all = soup.new_tag(
                         "NODE",
                         KeyType="0",
                         Name=f'All {content["name"]}',
                         Type="1",
                     )
-                    folder.append(_all)
+                    node.append(_all)
                 for playlist in content["playlists"]:
                     _playlist = self._create_playlists(
                         soup=soup, content=playlist, tags=tags
                     )
                     if _playlist:
-                        folder.append(_playlist)
-                return folder
+                        node.append(_playlist)
         elif isinstance(content, str):
             tags.add(content)
-            playlist = soup.new_tag("NODE", KeyType="0", Name=content, Type="1")
-            return playlist
+            node = soup.new_tag("NODE", KeyType="0", Name=content, Type="1")
         else:
             raise ValueError(
                 f"Encountered invalid input type {type(content)}: {content}"
             )
+        return node
 
 
-def rekordbox_playlists(config: BaseConfig):
+def build_playlists(config: BaseConfig):
     """Runs the PlaylistBuilder.
 
     Args:
         config: Configuration object.
     """
     playlist_config = (
         Path(__file__).parent.parent / "configs" / "rekordbox_playlists.yaml"
     )
     playlist_builder = PlaylistBuilder(
         rekordbox_database=config.XML_PATH,
         playlist_config=playlist_config,
         pure_genre_playlists=config.PURE_GENRE_PLAYLISTS,
-        playlist_remainder_type=config.REKORDBOX_PLAYLISTS_REMAINDER,
+        playlist_remainder_type=config.BUILD_PLAYLISTS_REMAINDER,
     )
     playlist_builder()
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/shuffle_playlists.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """This module is used to emulate shuffling the track order of one or more
 playlists. This is done by setting the Rekordbox tag (i.e. "TrackNumber") of
 tracks in the playlists to sequential numbers. After setting the TrackNumber
-tags of tracks in the provided playlists, those tracks must be reimported
+tags of tracks in the provided playlists, those tracks must be re-imported
 for Rekordbox to be aware of the update.
 """
 from concurrent.futures import ThreadPoolExecutor
 import logging
 import os
 import random
 
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
 
 from djtools.configs.config import BaseConfig
-from djtools.rekordbox.helpers import get_playlist_track_locations, set_tag
+from djtools.rekordbox.helpers import get_playlist_tracks, set_track_number
 
 
 logger = logging.getLogger(__name__)
 
 
-def randomize_playlists(config: BaseConfig):
-    """For each playlist in "RANDOMIZE_PLAYLISTS", shuffle the tracks and
+def shuffle_playlists(config: BaseConfig):
+    """For each playlist in "SHUFFLE_PLAYLISTS", shuffle the tracks and
     sequentially set the TrackNumber tag to a number to emulate track
     randomization.
 
     Args:
         config: Configuration object.
     """
     # Load Rekordbox database from XML.
@@ -35,44 +35,44 @@
     # Create track ID lookup.
     lookup = {}
     for track in soup.find_all("TRACK"):
         if not track.get("Location"):
             continue
         lookup[track["TrackID"]] = track
 
-    # Build a list of tracks to randomize from the provided list of playlists.
+    # Build a list of tracks to shuffle from the provided list of playlists.
     seen_tracks = set()
-    randomized_tracks = []
-    for playlist in config.RANDOMIZE_PLAYLISTS:
+    shuffled_tracks = []
+    for playlist in config.SHUFFLE_PLAYLISTS:
         try:
-            tracks = get_playlist_track_locations(soup, playlist, seen_tracks)
+            tracks = get_playlist_tracks(soup, playlist, seen_tracks)
         except LookupError as exc:
-            raise LookupError(f"{playlist} not found")
+            raise LookupError(f"{playlist} not found") from exc
 
         random.shuffle(tracks)
-        randomized_tracks.extend(tracks)
+        shuffled_tracks.extend(tracks)
 
     # Shuffle the track number field of the tracks.
-    randomized_tracks = [lookup[x] for x in randomized_tracks]
-    payload = [randomized_tracks, list(range(1, len(randomized_tracks) + 1))]
+    shuffled_tracks = [lookup[x] for x in shuffled_tracks]
+    payload = [shuffled_tracks, list(range(1, len(shuffled_tracks) + 1))]
     with ThreadPoolExecutor(max_workers=os.cpu_count() * 4) as executor:
         _ = list(
             tqdm(
-                executor.map(set_tag, *payload),
-                total=len(randomized_tracks),
-                desc=f"Randomizing {len(randomized_tracks)} tracks",
+                executor.map(set_track_number, *payload),
+                total=len(shuffled_tracks),
+                desc=f"Randomizing {len(shuffled_tracks)} tracks",
             )
         )
 
-    # Insert randomized tracks playlist into the playlist root.
+    # Insert shuffled tracks playlist into the playlist root.
     playlists_root = soup.find_all("NODE", {"Name": "ROOT", "Type": "0"})[0]
     new_playlist = soup.new_tag(
-        "NODE", KeyType="0", Name="AUTO_RANDOMIZE", Type="1"
+        "NODE", KeyType="0", Name="AUTO_SHUFFLE", Type="1"
     )
-    for track in randomized_tracks:
+    for track in shuffled_tracks:
         new_playlist.append(soup.new_tag("TRACK", Key=track["TrackID"]))
     playlists_root.insert(0, new_playlist)
 
     # Write XML file.
     _dir = config.XML_PATH.parent
     _file = config.XML_PATH.name
     auto_xml_path = _dir / f"auto_{_file}"
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/playlist_combiner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,78 @@
-"""This module contains the abstract bass class, TagParser, and implementations
-of TagParser.
+"""The "Combiner" constructs Rekordbox playlists by evaluating arbitrary
+boolean algebra expressions provided as the playlist name.
 
-A TagParser implementation is instantiated with a "parser_config" which
-describes the taxonomy of folders and playlists to be constructed from
-particular tags. An instantiated TagParser is called with a track and must
-return a list of tags from which playlists are to be constructed.
-
-In addition to these, a special "Combiner" TagParser may be configured. The
-"Combiner" configuration must specify a flat list of "playlists" which are
-defined as boolean algebra expressions which combine any of the tags generated
-by the other TagParsers ("Combiner" runs after the other TagParsers).
+The supported operands are:
+
+- string literals matching one of the possible returned tags from a TagParser
+    implementation (see GenreTagParser and MyTagParser)
+- playlist names enclosed in curly braces e.g. {My Favorites}
+- ratings in the inclusive range [0, 5], separated by commas with ranges
+    denoted using a dash; both styles are enclosed with square brackets e.g.
+    [0, 2-5]
+- BPMs in the inclusive range [6, inf], separated by commas with ranges denoted
+    using a dash; both styles are enclosed with square brackets e.g.
+    [80-90, 140, 160-180]
+
+NOTE: the use of an asterisk `*` in an operand will glob other tags. For
+example, the providing "* Techno" as an operand would match "Acid Techno" and
+"Hard Techno" but not "somethingTechno" (because of the space character).
+Providing "Deep *" as an operand would match "Deep House" as well as
+"Deep Dubstep".
+
+The supported operators are:
+
+- `&` a.k.a. AND a.k.a set intersection: resulting tracks must be in BOTH sets
+- `|` a.k.a. OR a.k.a set union: resulting tracks may be in EITHER sets
+- `~` a.k.a. NOT a.k.a set difference: resulting tracks are those from the
+    left-hand side of the operator with the tracks appearing on the right-hand
+    side of the operator removed
+- `(`, `)`: parentheses are used to control the order of operations
+
+Some example expressions:
+
+- "(([120-129] & *Techno) | [130-160]) ~ [5]" This will first match all tracks
+    in the BPM range 120-129 inclusive before intersecting those with tracks
+    with a tag containing "Techno" as a suffix before unioning with all tracks
+    in the BPM range 130-160. Lastly, any tracks having a rating of 5 are
+    removed from the playlist.
+- "(Chill | Melodic) ~ {All Bass}" This will first take the union of all tracks
+    with either a "Chill" tag or a "Melodic" tag before removing all tracks
+    that appear in a playlist called "All Bass".
+
+The "Combiner" configuration must specify a flat list of "playlists" which
+define the boolean algebra expressions used by the Combiner.
 """
-from abc import ABC, abstractmethod
 from collections import defaultdict
 import logging
 import re
-from typing import Dict, List, Optional, Set, Tuple, Union
+from typing import Dict, List, Set, Tuple, Union
 
-import bs4
 from bs4 import BeautifulSoup
 
 from djtools.rekordbox.helpers import BooleanNode
 
 
 logger = logging.getLogger(__name__)
 
 
-class TagParser(ABC):
-    """Abstract base class for parsing tags from a Rekordbox database."""
-
-    def __init__(
-        self,
-        parser_config: Dict[str, Union[str, List[Union[str, Dict]]]],
-        **kwargs,
-    ):
-        """Constructor.
-
-        Args:
-            parser_config: YAML playlist structure.
-        """
-        self.parser_config = parser_config
-
-    @abstractmethod
-    def __call__(self, track: bs4.element.Tag) -> List[str]:
-        """Produces a list of tags from a track.
-
-        Args:
-            track: A track from a Rekordbox database.
-
-        Raises:
-            NotImplementedError: Implementations must define tag parsing.
-
-        Returns:
-            List of tags.
-        """
-        raise NotImplementedError(
-            "Classes inheriting from TagParser must override the __call__ method."
-        )
-
-
-class Combiner(TagParser):
+class Combiner:
     """Parses a boolean algebra expression to combine tag playlists."""
 
     def __init__(
         self,
         parser_config: Dict[str, Union[str, List[Union[str, Dict]]]],
         rekordbox_database: BeautifulSoup,
-        **kwargs,
     ):
         """Constructor.
 
         Args:
             parser_config: YAML playlist structure.
         """
-        super().__init__(parser_config, **kwargs)
+        self.parser_config = parser_config
         self._tracks = defaultdict(lambda: defaultdict(list))
         self._bpm_rating_lookup = {}
         self._prescan(rekordbox_database)
         self._operators = {
             "&": set.intersection,
             "|": set.union,
             "~": set.difference,
@@ -95,17 +90,17 @@
             Dict mapping boolean expression to a set of track IDs.
         """
         self._tracks.update({k: dict(v) for k, v in tracks.items()})
         playlist_tracks = {
             expression: self._parse_boolean_expression(expression)
             for expression in self.parser_config.get("playlists", [])
         }
-        
+
         return playlist_tracks
-    
+
     def _add_tag(self, tag: str, node: BooleanNode) -> str:
         """Strips whitespace off of a tag and, if non-empty, adds it to a node.
 
         Args:
             tag: Potentially assembled tag string.
             node: BooleanNode to potentially have tag added to it.
 
@@ -159,15 +154,15 @@
     def _parse_boolean_expression(self, expression: str) -> Set[str]:
         """Parses a boolean algebra expression by constructing a tree.
 
         Args:
             expression: String representing boolean algebra expression.
 
         Returns:
-            Set of track IDs reduced from the evaulation of the expression.
+            Set of track IDs reduced from the evaluation of the expression.
         """
         node = BooleanNode()
         tag = ""
         for char in expression:
             if char == "(":
                 node = BooleanNode(parent=node)
             elif char in self._operators:
@@ -180,15 +175,15 @@
                 if tracks:
                     node.tracks.append(tracks)
             else:
                 tag += char
         tag = self._add_tag(tag, node)
 
         return node(self._tracks)
-    
+
     def _parse_bpms_and_ratings(
         self, bpm_rating_match: List[str]
     ) -> List[Tuple]:
         """Parses a string match of one or more BPM and / or rating selectors.
 
         Args:
             bpm_rating_match: List of BPM or rating strings.
@@ -218,28 +213,26 @@
                     _range = list(map(int, part.split("-")))
                     _range = range(min(_range), max(_range) + 1)
                     if all(0 <= x <= 5 for x in _range):
                         ratings.extend(map(str, _range))
                     elif all(x > 5 for x in _range):
                         bpms.extend(map(str, _range))
                     else:
-                        logger.error(
-                            "Bad BPM or rating number range: {}".format(part)
-                        )
+                        logger.error(f"Bad BPM or rating number range: {part}")
                         continue
                 else:
                     logger.error(
-                        "Malformed BPM or rating filter part: {}".format(part)
+                        f"Malformed BPM or rating filter part: {part}"
                     )
                     continue
-                
+
                 self._bpm_rating_lookup[
                     tuple(map(str, _range or [])) or str(number)
                 ] = f"[{part}]"
-                
+
         return bpms, ratings
 
     def _prescan(self, rekordbox_database: BeautifulSoup):
         """Populates track lookup using BPM and rating selectors.
 
         Boolean expressions may contain zero or more indicators for selectors:
             * BPM selectors: comma-delimited list of integers or integer ranges
@@ -271,15 +264,15 @@
 
         Raises:
             LookupError: Playlists in expressions must exist in "XML_PATH".
         """
         # Get the sets of BPMs, ratings, and playlists in order to pre-populate
         # the track lookup.
         bpms, ratings, self._playlists = set(), set(), set()
-        for expression in self.parser_config.get("playlists", []): 
+        for expression in self.parser_config.get("playlists", []):
             self._playlists.update(re.findall(r"(?<={)[^{}]*(?=})", expression))
             bpm_rating_match = re.findall(r"(?<=\[)[^\[\]]*(?=\])", expression)
             if not bpm_rating_match:
                 continue
             _bpms, _ratings = self._parse_bpms_and_ratings(bpm_rating_match)
             bpms.update(_bpms)
             ratings.update(_ratings)
@@ -308,77 +301,7 @@
                 if val in values_set:
                     for value, tag in self._bpm_rating_lookup.items():
                         if (
                             (isinstance(value, str) and value == val) or
                             (isinstance(value, tuple) and val in value)
                         ):
                             self._tracks[tag][track["TrackID"]] = []
-
-
-class GenreTagParser(TagParser):
-    """Parses the "Genre" field of a track to produce tags."""
-
-    def __init__(
-        self,
-        parser_config: Dict[str, Union[str, List[Union[str, Dict]]]],
-        pure_genre_playlists: Optional[List[str]] = list(),
-        **kwargs,
-    ):
-        """Constructor.
-
-        Args:
-            parser_config: YAML playlist structure.
-            pure_genre_playlists: List of genre tags from which "pure"
-                playlists will be generated. A "pure" playlist is one in which
-                every track has genre tags which all contain a corresponding
-                element in this list.
-        """
-        super().__init__(parser_config)
-        self._pure_playlists = pure_genre_playlists
-
-    def __call__(self, track: bs4.element.Tag) -> List[str]:
-        """Produces a list of genre tags from a track.
-
-        Args:
-            track: A track from a Rekordbox database.
-
-        Returns:
-            List of genre tags.
-        """
-        tags = [x.strip() for x in track["Genre"].split("/")]
-        for genre in self._pure_playlists:
-            if all(genre.lower() in x.lower() for x in tags):
-                tags.append(f"Pure {genre}")
-        
-        return tags
-
-
-class MyTagParser(TagParser):
-    """Parses the "Comments" field of a track to produce tags."""
-
-    def __init__(
-        self,
-        parser_config: Dict[str, Union[str, List[Union[str, Dict]]]],
-        **kwargs,
-    ):
-        """Constructor.
-
-        Args:
-            parser_config: YAML playlist structure.
-        """
-        super().__init__(parser_config, **kwargs)
-        self._regex = re.compile(r"(?<=\/\*).*(?=\*\/)")
-
-    def __call__(self, track: bs4.element.Tag) -> List[str]:
-        """Produces a list of "My Tags" tags from a track.
-
-        Args:
-            track: A track from a Rekordbox database.
-
-        Returns:
-            List of "My Tags" tags.
-        """
-        tags = re.search(self._regex, track.get("Comments"))
-        if not tags:
-            return []
-
-        return [x.strip() for x in tags.group().split("/")]
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_copy_playlists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+"""Testing for the copy_playlists module."""
 from pathlib import Path
 from urllib.parse import unquote
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.rekordbox.copy_playlists import copy_playlists
 
 
 def test_copy_playlists(tmpdir, test_config, test_xml):
+    """Test for the copy_playlists function."""
     target_playlists = ["Hip Hop"]
     test_xml = Path(test_xml)
-    new_xml = test_xml.parent / "relocated_rekordbox.xml"
+    new_xml = test_xml.parent / "auto_rekordbox.xml"
     test_output_dir = Path(tmpdir) / "output"
     test_config.XML_PATH = test_xml
     test_config.COPY_PLAYLISTS = target_playlists
     test_config.COPY_PLAYLISTS_DESTINATION = Path(test_output_dir)
     copy_playlists(test_config)
     assert list(test_output_dir.iterdir())
     assert new_xml.exists()
     with open(new_xml, mode="r", encoding="utf-8") as _file:
         xml = BeautifulSoup(_file.read(), "xml")
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
         assert any(x in track["Genre"] for x in target_playlists)
         assert test_output_dir.as_posix() in unquote(track["Location"])
-        
+
 
 def test_copy_playlists_invalid_playlist(tmpdir, test_config, test_xml):
+    """Test for the copy_playlists function."""
     playlist = "invalid_playlist"
     test_config.XML_PATH = test_xml
     test_config.COPY_PLAYLISTS = [playlist]
     test_config.COPY_PLAYLISTS_DESTINATION = Path(tmpdir)
     with pytest.raises(LookupError, match=f"{playlist} not found"):
         copy_playlists(test_config)
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+"""Testing for the helpers module."""
 import inspect
 from pathlib import Path
 import re
 from urllib.parse import unquote
 
 import pytest
 
 from djtools.rekordbox.helpers import (
     BooleanNode,
     copy_file,
-    get_playlist_track_locations,
-    set_tag,
+    get_playlist_tracks,
+    set_track_number,
 )
 
 
 @pytest.mark.parametrize(
     "node_attributes",
     [
         (
@@ -22,14 +23,15 @@
             {11,12},
         ),
         ([set.difference], ["*House", "Bass House"], {3,5,6,7,8}),
         ([set.intersection], ["{All DnB}", "Dark"], {2}),
     ],
 )
 def test_booleannode(node_attributes):
+    """Test for the BooleanNode class."""
     operators, tags, expected = node_attributes
     tracks = {
         "{All DnB}": [1,2,3],
         "Acid House": [7,8],
         "Bass House": [9,10],
         "Breaks": [3,4],
         "Dark": [2,11],
@@ -43,16 +45,17 @@
     node.operators = operators
     node.tags = tags
     result = node(tracks)
     assert result == expected
 
 
 def test_booleannode_raises_runtime_eror():
+    """Test for the BooleanNode class."""
     node = BooleanNode()
-    node.operators = [set.union] 
+    node.operators = [set.union]
     node.tags = ["tag"]
     with pytest.raises(
         RuntimeError,
         match=(
             re.escape(
                 f"Invalid boolean expression: track sets: {len(node.tracks)}, "
             ) +
@@ -60,43 +63,47 @@
             re.escape(f"{[x.__name__ for x in node.operators]}")
         ),
     ):
         node({})
 
 
 def test_copy_file(tmpdir, test_track):
+    """Test for the copy_file function."""
     dest_dir = Path(tmpdir) / "output"
     dest_dir.mkdir(parents=True, exist_ok=True)
     old_track_loc = Path(test_track["Location"])
     copy_file(track=test_track, destination=dest_dir)
     new_track_loc = unquote(test_track["Location"])
     loc_prefix = inspect.signature(
         copy_file
     ).parameters.get("loc_prefix").default
     new_file_path = dest_dir / old_track_loc.name
     # NOTE(a-rich): `Location` attributes in the XML's `TRACK` tags always
     # have unix-style paths so comparisons made with paths created in Windows
-    # must be interpretted `.as_posix()`.
+    # must be interpreted `.as_posix()`.
     assert new_track_loc == f"{loc_prefix}{new_file_path.as_posix()}"
     assert new_file_path.exists()
 
 
-def test_get_playlist_track_locations(xml):
+def test_get_playlist_tracks(xml):
+    """Test for the get_playlist_tracks function."""
     playlist = "Hip Hop"
     seen_tracks = set()
-    ret = get_playlist_track_locations(xml, playlist, seen_tracks)
+    ret = get_playlist_tracks(xml, playlist, seen_tracks)
     assert seen_tracks
     assert ret
     assert len(ret) == len(seen_tracks)
 
 
-def test_get_playlist_track_locations_no_playlist(xml):
+def test_get_playlist_tracks_no_playlist(xml):
+    """Test for the get_playlist_tracks function."""
     playlist = "nonexistent playlist"
     seen_tracks = set()
     with pytest.raises(LookupError, match=f"{playlist} not found"):
-        get_playlist_track_locations(xml, playlist, seen_tracks)
+        get_playlist_tracks(xml, playlist, seen_tracks)
 
 
 @pytest.mark.parametrize("index", [0, 5, 9])
-def test_set_tag(index, test_track):
-    set_tag(test_track, index)
+def test_set_track_number(index, test_track):
+    """Test for the set_track_number function."""
+    set_track_number(test_track, index)
     assert test_track.get("TrackNumber") == index
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_playlist_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,50 @@
+"""Testing for the playlist_builder module."""
 import os
 from pathlib import Path
 
 from bs4 import BeautifulSoup
 import pytest
 import yaml
 
 from djtools.rekordbox.playlist_builder import (
-    PlaylistBuilder, rekordbox_playlists    
+    build_playlists, PlaylistBuilder
 )
 
 
+def test_build_playlists(test_config, test_xml):
+    """Test for the build_playlists function."""
+    test_config.XML_PATH = Path(test_xml)
+    build_playlists(test_config)
+
+
 @pytest.mark.parametrize(
     "remainder_type", ["", "folder", "playlist", "invalid"]
 )
 def test_playlistbuilder(remainder_type, test_xml, test_playlist_config):
-    playlist_builder = PlaylistBuilder(
+    """Test for the PlaylistBuilder class."""
+    PlaylistBuilder(
         rekordbox_database=Path(test_xml),
         playlist_config=Path(test_playlist_config),
         pure_genre_playlists=["Dubstep"],
         playlist_remainder_type=remainder_type
     )()
 
 
 def test_playlistbuilder_combiner_playlist_contains_new_playlist_selector_tracks(
     test_playlist_config, test_xml, xml
 ):
+    """Test for the PlaylistBuilder class."""
     # Insert test track and Combiner playlist to target it.
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     new_track = xml.new_tag("TRACK")
-    new_track_ID = "-1"
+    new_track_id = "-1"
     new_track.attrs = {
-        "TrackID": new_track_ID,
+        "TrackID": new_track_id,
         "AverageBpm": "140.00",
         "Genre": "Dubstep",
         "Rating": "255",
         "Location": "file://localhost/test-track.mp3",
         "Comments": "",
     }
     collection = xml.find_all("COLLECTION")[0]
@@ -50,58 +59,60 @@
         playlist_config = yaml.dump(playlist_config, _file)
     with open(test_xml, mode="wb", encoding=xml.orignal_encoding) as _file:
         _file.write(xml.prettify("utf-8"))
 
     # Test pre-conditions.
     playlist = xml.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
-        assert (
-            track_key["Key"] != new_track_ID,
+        assert track_key["Key"] != new_track_id, (
             "Test track should not exist in Dubstep!"
         )
     test_track = None
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
-        if track.get("TrackID") == new_track_ID:
+        if track.get("TrackID") == new_track_id:
             test_track = track
     assert test_track, "Test track should exist in XML!"
 
     # Run the PlaylistBuilder (GenreTagParser and Combiner).
-    playlist_builder = PlaylistBuilder(
+    PlaylistBuilder(
         rekordbox_database=Path(test_xml),
         playlist_config=Path(test_playlist_config),
     )()
 
     # Load XML generated by the PlaylistBuilder.
     path, file_name = os.path.split(test_xml)
-    with open(os.path.join(path, f"auto_{file_name}"), mode="r", encoding="utf-8") as _file:
-        db = BeautifulSoup(_file.read(), "xml")
+    with open(
+        os.path.join(path, f"auto_{file_name}"), mode="r", encoding="utf-8"
+    ) as _file:
+        database = BeautifulSoup(_file.read(), "xml")
 
     # Test that the test track was inserted into the "Dubstep" playlist.
     test_track = None
-    playlist = db.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
+    playlist = database.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
-        if track_key["Key"] == new_track_ID:
+        if track_key["Key"] == new_track_id:
             test_track = track_key
     assert test_track, "New track was not found in the genre playlist!"
 
     # Test that the test track was inserted into the Combiner playlist.
     test_track = None
     test_track = None
-    playlist = db.find_all("NODE", {"Name": selector_playlist, "Type": "1"})[0]
+    playlist = database.find_all(
+        "NODE", {"Name": selector_playlist, "Type": "1"}
+    )[0]
     for track_key in playlist.find_all("TRACK"):
-        if track_key["Key"] == new_track_ID:
+        if track_key["Key"] == new_track_id:
             test_track = track_key
     assert test_track, "New track was not found in the Combiner playlist!"
 
 
-def test_playlistbuilder_invalid_parser(
-    tmpdir, test_xml, test_playlist_config
-):
+def test_playlistbuilder_invalid_parser(test_xml, test_playlist_config):
+    """Test for the PlaylistBuilder class."""
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     parser_type = "nonexistent_parser"
     playlist_config[parser_type] = {}
     with open(test_playlist_config, mode="w", encoding="utf-8",) as _file:
         playlist_config = yaml.dump(playlist_config, _file)
     with pytest.raises(
@@ -110,17 +121,16 @@
     ):
         PlaylistBuilder(
             rekordbox_database=test_xml,
             playlist_config=test_playlist_config,
         )()
 
 
-def test_playlistbuilder_invalid_playlist(
-    tmpdir, test_xml, test_playlist_config
-):
+def test_playlistbuilder_invalid_playlist(test_xml, test_playlist_config):
+    """Test for the PlaylistBuilder class."""
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     content = [0]
     playlist_config = {
         "GenreTagParser": {"name": "invalid", "playlists": content}
     }
     with open(test_playlist_config, mode="w", encoding="utf-8",) as _file:
@@ -129,12 +139,7 @@
         ValueError,
         match=f"Encountered invalid input type {type(content[0])}: {content[0]}"
     ):
         PlaylistBuilder(
             rekordbox_database=test_xml,
             playlist_config=test_playlist_config,
         )()
-
-
-def test_rekordbox_playlists(test_config, test_xml):
-    test_config.XML_PATH = Path(test_xml)
-    rekordbox_playlists(test_config)
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.0b0/djtools/rekordbox/test_tag_parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""Testing for the tag_parser module."""
 import pytest
 import yaml
 
+from djtools.rekordbox.playlist_combiner import Combiner
 from djtools.rekordbox.tag_parsers import (
-    Combiner, GenreTagParser, MyTagParser, TagParser
+    GenreTagParser, MyTagParser, TagParser
 )
 
 
 def test_combiner(test_playlist_config, xml, caplog):
+    """Test Combiner class."""
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     bad_playlist = "Dark & [-1, 5-7, a-5]"
     selector_playlists = [
         x for x in playlist_config["Combiner"]["playlists"]
         if "[" in x or "{" in x
     ]
@@ -33,27 +36,29 @@
         "Malformed BPM or rating filter part: a-5"
     )
 
 
 def test_combiner_raises_lookuperror_for_bad_playlist(
     test_playlist_config, xml
 ):
+    """Test Combiner class."""
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     bad_playlist = "nonexistent playlist"
     playlist_config["Combiner"]["playlists"] = [f"{{{bad_playlist}}} | Dark"]
     with pytest.raises(LookupError, match=f"{bad_playlist} not found"):
         combiner_parser = Combiner(
             parser_config=playlist_config["Combiner"],
             rekordbox_database=xml,
         )
         combiner_parser.get_playlist_mapping(xml)
 
 
 def test_genretagparser(test_playlist_config, xml):
+    """Test GenreTagParser class."""
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     genre = "Hip Hop"
     parser = GenreTagParser(
         parser_config=playlist_config["GenreTagParser"],
         pure_genre_playlists=[genre],
     )
@@ -69,14 +74,15 @@
         if f"Pure {genre}" in tags:
             assert all(
                 genre in tag for tag in tags
             )
 
 
 def test_mytagparser(test_playlist_config, xml):
+    """Test MyTagParser class."""
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
     mytag = "Dark"
     parser = MyTagParser(parser_config=playlist_config["MyTagParser"])
     tracks = {
         track["TrackID"]: track for track in xml.find_all("TRACK")
         if track.get("Location")
@@ -85,27 +91,29 @@
     for track_key in playlist.find_all("TRACK"):
         track = tracks[track_key["Key"]]
         tags = parser(track)
         assert mytag in tags
 
 
 def test_tagparser_raises_type_error():
+    """Test TagParser class."""
     with pytest.raises(
         TypeError,
         match=(
             "Can't instantiate abstract class TagParser with abstract method"
         ),
     ):
-        TagParser()
+        TagParser(parser_config={})
 
 
 def test_tagparser_call_raises_not_imlemented_error(test_track):
+    """Test TagParser class."""
     TagParser.__abstractmethods__ = set()
     class TagParserSubclass(TagParser):
-        pass
+        """Dummy sub-class."""
 
     with pytest.raises(
         NotImplementedError,
         match=(
             "Classes inheriting from TagParser must override the __call__ "
             "method."
         ),
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """The `spotify` package contains modules:
     * `config`: the configuration object for the `spotify` package
     * `helpers`: helper functions for `playlist_builder`
     * `playlist_builder`: constructs or updates Spotify playlists using either
         Subreddit posts or the Discord webhook output from `UPLOAD_MUSIC`
 """
-from .config import SpotifyConfig
-from .playlist_builder import playlist_from_upload, update_auto_playlists
+from djtools.spotify.config import SpotifyConfig
+from djtools.spotify.playlist_builder import (
+    playlist_from_upload, update_auto_playlists
+)
 
 
 SPOTIFY_OPERATIONS = {
     "PLAYLIST_FROM_UPLOAD": playlist_from_upload,
     "AUTO_PLAYLIST_UPDATE": update_auto_playlists,
 }
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/config.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
     AUTO_PLAYLIST_DEFAULT_LIMIT: NonNegativeInt = 50
     AUTO_PLAYLIST_DEFAULT_PERIOD: str = "week"
     AUTO_PLAYLIST_DEFAULT_TYPE: str = "hot"
     AUTO_PLAYLIST_FUZZ_RATIO: NonNegativeInt = 70
     AUTO_PLAYLIST_POST_LIMIT: NonNegativeInt = 100
     AUTO_PLAYLIST_SUBREDDITS: List[SubredditConfig] = []
-    AUTO_PLAYLIST_UPDATE: bool = False 
-    PLAYLIST_FROM_UPLOAD: bool = False 
+    AUTO_PLAYLIST_UPDATE: bool = False
+    PLAYLIST_FROM_UPLOAD: bool = False
     REDDIT_CLIENT_ID: str = ""
     REDDIT_CLIENT_SECRET: str = ""
     REDDIT_USER_AGENT: str = ""
     SPOTIFY_CLIENT_ID: str = ""
     SPOTIFY_CLIENT_SECRET: str = ""
     SPOTIFY_REDIRECT_URI: str = ""
     SPOTIFY_USERNAME: str  = ""
@@ -69,22 +69,22 @@
         ):
             raise RuntimeError(
                 "Without all the configuration options SPOTIFY_CLIENT_ID, "
                 "SPOTIFY_CLIENT_SECRET, SPOTIFY_REDIRECT_URI, and "
                 "SPOTIFY_USERNAME set to valid values, you cannot use "
                 "AUTO_PLAYLIST_UPDATE or PLAYLIST_FROM_UPLOAD"
             )
-        elif self.AUTO_PLAYLIST_UPDATE or self.PLAYLIST_FROM_UPLOAD:
+        if self.AUTO_PLAYLIST_UPDATE or self.PLAYLIST_FROM_UPLOAD:
             from djtools.spotify.helpers import get_spotify_client
             spotify = get_spotify_client(self)
             try:
                 spotify.current_user()
-            except Exception:
-                raise RuntimeError("Spotify credentials are invalid!")
-        
+            except Exception as exc:
+                raise RuntimeError("Spotify credentials are invalid!") from exc
+
         if self.AUTO_PLAYLIST_UPDATE and not all(
             [
                 self.REDDIT_CLIENT_ID,
                 self.REDDIT_CLIENT_SECRET,
                 self.REDDIT_USER_AGENT,
             ]
         ):
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """This module contains helper functions used by the "spotify" module."""
 from concurrent.futures import ThreadPoolExecutor
 import logging
 from operator import itemgetter
-import os
 from pathlib import Path
 import sys
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import Any, AsyncGenerator, Dict, List, Optional, Set, Tuple, Union
 
 import asyncpraw as praw
 from fuzzywuzzy import fuzz
 import spotipy
 from spotipy.oauth2 import SpotifyOAuth
 from tqdm import tqdm
 import yaml
@@ -42,14 +41,34 @@
         username, name=f"{subreddit.title()}"
     )
     spotify.playlist_add_items(playlist["id"], ids, position=None)
 
     return playlist
 
 
+async def catch(generator: AsyncGenerator, message: Optional[str] = "") -> Any:
+    """This function permits one-line try/except logic for comprehensions.
+
+    Args:
+        generator: Async generator.
+        message: Prefix message for logger warning.
+
+    Returns:
+        Return of the AsyncGenerator.
+    """
+    while True:
+        try:
+            yield await generator.__anext__()
+        except StopAsyncIteration:
+            return
+        except Exception as exc:
+            logger.warning(f"{message}: {exc}" if message else exc)
+            continue
+
+
 def filter_results(
     spotify: spotipy.Spotify,
     results: List[Dict],
     threshold: float,
     title: str,
     artist: str,
 ) -> Tuple[Dict[str, Any], float]:
@@ -62,31 +81,32 @@
         threshold: Minimum Levenshtein distance.
         title: Potential title of a track.
         artist: Potential artist of a track.
 
     Returns:
         Tuple of track object and Levenshtein distance. 
     """
+    track, dist = {}, 0.0
     tracks = filter_tracks(
         results["tracks"]["items"], threshold, title, artist
     )
     while results["tracks"]["next"]:
         try:
             results = spotify.next(results["tracks"])
         except Exception:
             logger.warning(f"Failed to get next tracks for {title, artist}")
             break
         tracks.extend(
             filter_tracks(results["tracks"]["items"], threshold, title, artist)
         )
 
     if tracks:
-        track, _ = sorted(tracks, key=itemgetter(1)).pop()
+        track, dist = max(tracks, key=itemgetter(1))
 
-        return track
+    return track, dist
 
 
 def filter_tracks(
     tracks: Dict, threshold: float, title: str, artist: str
 ) -> List[Tuple[Dict[str, Any], float]]:
     """Applies Levenshtein distance filtering on both the resulting
         tracks' "artist" and "name" fields to qualify a match for the
@@ -98,27 +118,29 @@
         title: Potential title of a track.
         artist: Potential artist of a track.
 
     Returns:
         List of tuple of track object and Levenshtein distance. 
     """
     results = []
+    artist = ", ".join(sorted([x.strip() for x in artist.split(",")]))
     for track in tracks:
-        artists = sorted({x["name"].lower() for x in track["artists"]})
+        artists = ", ".join(
+            sorted({x["name"].lower() for x in track["artists"]})
+        )
         title_match = max(
             fuzz.ratio(track["name"].lower(), title.lower()),
             fuzz.ratio(track["name"].lower(), artist.lower())
         )
-        if title_match >= threshold:
-            if any(
-                fuzz.ratio(a, part) >= threshold
-                for part in [title.lower(), artist.lower()]
-                for a in artists + [", ".join(artists)]
-            ):
-                results.append((track, title_match))
+        artist_match = max(
+            fuzz.ratio(artists.lower(), title.lower()),
+            fuzz.ratio(artists.lower(), artist.lower()),
+        )
+        if title_match >= threshold and artist_match >= threshold:
+            results.append((track, title_match + artist_match))
 
     return results
 
 
 def fuzzy_match(
     spotify: spotipy.Spotify, title: str, threshold: float
 ) -> Optional[Tuple[str]]:
@@ -131,52 +153,55 @@
         spotify: Spotify client.
         title: Submission title.
         threshold: Minimum Levenshtein distance.
 
     Returns:
         Tuple of matching track's ID and artist - title or None if no match.
     """
-    title, artist = parse_title(title)
-    if not (title and artist):
-        return
-
-    query = (
-        f'{title.replace(" ", "+")}+'
-        f'{artist.replace(" ", "+").replace(",", "")}'
-    )
-    try:
-        results = spotify.search(
-            q=query,
-            type="track",
-            limit=50,
-        )
-    except Exception as exc:
-        logger.error(f'Error searching for "{title} - {artist}": {exc}')
-        return
-
-    match = filter_results(spotify, results, threshold, title, artist)
-    if match:
-        artists = ", ".join([y["name"] for y in match["artists"]])
-        return match["id"], f'{match["name"]} - {artists}'
+    ret = None
+    parts = parse_title(title)
+    if not all(parts):
+        return ret
+
+    matches = []
+    for track, artist in [parts, parts[::-1]]:
+        try:
+            results = spotify.search(
+                q=f"track:{track} artist:{artist}",
+                type="track",
+                limit=50,
+            )
+        except Exception as exc:
+            logger.error(f'Error searching for "{track} - {artist}": {exc}')
+            continue
+
+        artist = ", ".join(sorted([x.strip() for x in artist.split(",")]))
+        match, dist = filter_results(spotify, results, threshold, track, artist)
+        if match:
+            artists = ", ".join([y["name"] for y in match["artists"]])
+            matches.append((dist, match["id"], f'{match["name"]} - {artists}'))
+
+    if matches:
+        ret = tuple(max(matches, key=itemgetter(0))[1:])
 
-    return
+    return ret
 
 
 def get_playlist_ids() -> Dict[str, str]:
     """Load Spotify playlist names -> IDs lookup.
 
     Returns:
         Dictionary of Spotify playlist names mapped to playlist IDs. 
     """
     playlist_ids = {}
     ids_path = Path(__file__).parent.parent / "configs" / "spotify_playlists.yaml"
     if ids_path.exists():
         with open(ids_path, mode="r", encoding="utf-8") as _file:
             playlist_ids = yaml.load(_file, Loader=yaml.FullLoader) or {}
-    
+
     return playlist_ids
 
 
 def get_reddit_client(config: BaseConfig) -> praw.Reddit:
     """Instantiate a Reddit API client.
 
     Args:
@@ -187,15 +212,15 @@
     """
     reddit = praw.Reddit(
         client_id=config.REDDIT_CLIENT_ID,
         client_secret=config.REDDIT_CLIENT_SECRET,
         user_agent=config.REDDIT_USER_AGENT,
         timeout=30,
     )
-    
+
     return reddit
 
 
 def get_spotify_client(config: BaseConfig) -> spotipy.Spotify:
     """Instantiate a Spotify API client.
 
     Args:
@@ -212,15 +237,15 @@
             scope="playlist-modify-public",
             requests_timeout=30,
             cache_handler=spotipy.CacheFileHandler(
                 cache_path=Path(__file__).parent / ".spotify.cache"
             ),
         )
     )
-    
+
     return spotify
 
 
 async def get_subreddit_posts(
     spotify: spotipy.Spotify,
     reddit: praw.Reddit,
     subreddit: Dict[str, Union[str, int]],
@@ -238,16 +263,14 @@
         config: Configuration object.
         praw_cache: Cached praw submissions.
 
     Returns:
         List of Spotify track ("id", "name") tuples and SubredditConfig as a
             dictionary.
     """
-    from djtools.utils.helpers import catch
-    
     sub = await reddit.subreddit(subreddit["name"])
     func = getattr(sub, subreddit["type"])
     kwargs = {"limit": config.AUTO_PLAYLIST_POST_LIMIT}
     if subreddit["type"]== "top":
         kwargs["time_filter"] = subreddit["period"]
     subs = [
         x async for x in catch(
@@ -259,15 +282,15 @@
     submissions = []
     for submission in tqdm(subs, desc=msg):
         if submission.id in praw_cache:
             continue
         submissions.append(submission)
         praw_cache[submission.id] = True
     new_tracks = []
-    if len(submissions):
+    if submissions:
         msg = (
             f"Searching Spotify for {len(submissions)} new submission(s) from "
             f'"r/{subreddit["name"]}"'
         )
         logger.info(msg)
         payload = [
             submissions,
@@ -289,15 +312,15 @@
         )
     else:
         logger.info(f'No new submissions from "r/{subreddit["name"]}"')
 
     return new_tracks, subreddit
 
 
-def parse_title(title: str) -> Tuple[str]:
+def parse_title(title: str) -> List[str]:
     """Attempts to split submission title into two parts
         (track name, artist(s)).
 
     Args:
         title: Submission title.
 
     Returns:
@@ -306,32 +329,45 @@
     """
     try:
         title, artist = map(str.strip, title.split(" - "))
     except ValueError:
         try:
             title, artist = map(str.strip, title.lower().split(" by "))
         except ValueError:
-            return None, None
+            return [None, None]
 
     title, artist = map(str.strip, [title.split("(")[0], artist.split("(")[0]])
     title, artist = map(str.strip, [title.split("[")[0], artist.split("[")[0]])
-    artist = ", ".join(sorted([x.strip() for x in artist.split(",")]))
 
-    return title, artist
+    return [title, artist]
 
 
 def populate_playlist(
     playlist_name: str,
     playlist_ids: Dict[str, str],
     spotify_username: str,
     spotify: spotipy.Spotify,
-    tracks: List[Tuple[str]], 
+    tracks: List[Tuple[str]],
     playlist_limit: Optional[int] = sys.maxsize,
     verbosity: Optional[int] = 0,
 ):
+    """Inserts tracks into either a new playlist or an existing one.
+
+    Args:
+        playlist_name: Name of the playlist.
+        playlist_ids: Lookup of playlist IDs.
+        spotify_username: Spotify users's username.
+        spotify: Spotify client.
+        tracks: List of tracks.
+        playlist_limit: Maximum number of tracks allowed in a playlist.
+        verbosity: Logging verbosity level.
+
+    Returns:
+        Updated playlist IDs.
+    """
     playlist_id = playlist_ids.get(playlist_name)
     playlist = None
     if playlist_id and tracks:
         playlist = update_existing_playlist(
             spotify,
             playlist_id,
             tracks,
@@ -350,15 +386,15 @@
     elif playlist_id:
         playlist = spotify.playlist(playlist_id)
     if playlist:
         logger.info(
             f'"{playlist["name"]}": '
             f'{playlist["external_urls"].get("spotify")}'
         )
-    
+
     return playlist_ids
 
 
 def process(
     submission: praw.models.Submission,
     spotify: spotipy.Spotify,
     threshold: float,
@@ -473,15 +509,15 @@
                 logger.info(f"\t{track}")
 
     if tracks_removed:
         logger.info(f"{len(tracks_removed)} old tracks removed")
         if verbosity > 0:
             for track in tracks_removed:
                 logger.info(f"\t{track}")
-    
+
     if not (tracks_added or tracks_removed):
         logger.info("No tracks added or removed")
 
     if remove_payload:
         spotify.playlist_remove_specific_occurrences_of_items(playlist,
                                                               remove_payload)
     if add_payload:
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/playlist_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 'ARTIST NAME - TRACK TITLE' or 'TRACK TITLE - ARTIST NAME'. These components
 are then used to search the Spotify API for tracks. The resulting tracks have
 their title and artist fields compared with the reddit post title and are added
 to the respective playlist if the Levenshtein similarity passes a threshold.
 """
 import asyncio
 import logging
-import os
 from pathlib import Path
 
 import pyperclip
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.spotify.helpers import (
@@ -50,21 +49,21 @@
 
     Args:
         config: Configuration object.
     """
     spotify = get_spotify_client(config)
     reddit = get_reddit_client(config)
     playlist_ids = get_playlist_ids()
-    
+
     praw_cache = {}
     cache_file = Path(__file__).parent / ".praw.cache"
     if cache_file.exists():
         with open(cache_file, mode="r", encoding="utf-8") as _file:
             praw_cache = yaml.load(_file, Loader=yaml.FullLoader) or {}
-    
+
     tasks = [
         asyncio.create_task(
             get_subreddit_posts(
                 spotify,
                 reddit,
                 subreddit,
                 config,
@@ -81,15 +80,15 @@
             playlist_ids=playlist_ids,
             spotify_username=config.SPOTIFY_USERNAME,
             spotify=spotify,
             tracks=tracks,
             playlist_limit=subreddit["limit"],
             verbosity=config.VERBOSITY,
         )
-    
+
     await reddit.close()
 
     write_playlist_ids(playlist_ids)
 
     with open(cache_file, mode="w", encoding="utf-8") as _file:
         yaml.dump(praw_cache, _file)
 
@@ -138,34 +137,30 @@
         files.append((track, artist))
     files = list(filter(lambda x: len(x) == 2, files))
 
     # Query Spotify for files in upload output.
     threshold = config.AUTO_PLAYLIST_FUZZ_RATIO
     tracks = []
     for title, artist in files:
-        artist = ", ".join(sorted([x.strip() for x in artist.split(",")]))
-        query = (
-            f'{title.replace(" ", "+")}+'
-            f'{artist.replace(" ", "+").replace(",", "")}'
-        )
+        query = f"track:{title} artist:{artist}"
         try:
             results = spotify.search(q=query, type="track", limit=50)
         except Exception as exc:
             logger.error(f'Error searching for "{title} - {artist}": {exc}')
             continue
 
-        match = filter_results(spotify, results, threshold, title, artist)
+        match, _ = filter_results(spotify, results, threshold, title, artist)
         if match:
             artists = ", ".join([y["name"] for y in match["artists"]])
             logger.info(f"Matched {match['name']} - {artists} to {title} - {artist}")
         else:
             logger.warning(f"Could not find a match for {title} - {artist}")
             continue
         tracks.append((match["id"], f'{match["name"]} - {artists}'))
-    
+
     playlist_ids = populate_playlist(
         playlist_name=f"{user} Uploads",
         playlist_ids=playlist_ids,
         spotify_username=config.SPOTIFY_USERNAME,
         spotify=spotify,
         tracks=tracks,
         verbosity=config.VERBOSITY,
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,54 @@
+"""Testing for the config module."""
 from unittest import mock
 
 import pytest
 
 from djtools.spotify.config import SpotifyConfig
 
 
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
-def test_spotifyconfig(mock_get_spotify_client):
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
+def test_spotifyconfig():
+    """Test for the SpotifyConfig class."""
     SpotifyConfig()
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 def test_baseconfig_invalid_spotify_credentials(mock_spotify):
+    """Test for the SpotifyConfig class."""
     mock_spotify.return_value.current_user.side_effect = Exception()
     cfg = {
         "PLAYLIST_FROM_UPLOAD": True,
         "SPOTIFY_CLIENT_ID": "not a real ID",
         "SPOTIFY_CLIENT_SECRET": "not a real secret",
         "SPOTIFY_REDIRECT_URI": "not a real URI",
         "SPOTIFY_USERNAME": "not a real username",
     }
     with pytest.raises(RuntimeError, match="Spotify credentials are invalid!"):
         SpotifyConfig(**cfg)
 
 
 def test_spotifyconfig_no_spotify_credentials():
+    """Test for the SpotifyConfig class."""
     cfg = {"PLAYLIST_FROM_UPLOAD": True, "SPOTIFY_CLIENT_ID": ""}
     with pytest.raises(
         RuntimeError,
         match=(
             "Without all the configuration options SPOTIFY_CLIENT_ID, "
             "SPOTIFY_CLIENT_SECRET, SPOTIFY_REDIRECT_URI, and "
             "SPOTIFY_USERNAME set to valid values, you cannot use "
             "AUTO_PLAYLIST_UPDATE or PLAYLIST_FROM_UPLOAD"
         ),
     ):
         SpotifyConfig(**cfg)
 
 
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
-def test_spotifyconfig_no_reddit_credentials(mock_get_spotify_client):
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.Mock())
+def test_spotifyconfig_no_reddit_credentials():
+    """Test for the SpotifyConfig class."""
     cfg = {
         "AUTO_PLAYLIST_UPDATE": True,
         "REDDIT_CLIENT_ID": "",
         "SPOTIFY_CLIENT_ID": "id",
         "SPOTIFY_CLIENT_SECRET": "secret",
         "SPOTIFY_REDIRECT_URI": "uri",
         "SPOTIFY_USERNAME": "name",
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Testing for the helpers module."""
 import asyncio
 from unittest import mock
 
 import pytest
 
 from djtools.spotify.config import SubredditConfig
 from djtools.spotify.helpers import (
     build_new_playlist,
+    catch,
     filter_results,
     filter_tracks,
     fuzzy_match,
     get_playlist_ids,
     get_reddit_client,
     get_spotify_client,
     get_subreddit_posts,
@@ -20,15 +22,16 @@
     update_existing_playlist,
     write_playlist_ids
 )
 from djtools.utils.helpers import MockOpen
 
 
 async def aiter(obj, num_subs):
-    for i in range(num_subs):
+    """Helper function for mocking asyncpraw."""
+    for _ in range(num_subs):
         yield obj
         await asyncio.sleep(0.1)
 
 
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify."
     "playlist_add_items",
@@ -43,43 +46,76 @@
     "djtools.spotify.helpers.spotipy.Spotify",
 )
 def test_build_new_playlist(
     mock_spotify,
     mock_spotify_user_playlist_create,
     mock_spotify_playlist_add_items,
 ):
+    """Test for the build_new_playlist function."""
     mock_spotify.user_playlist_create.return_value = (
         mock_spotify_user_playlist_create.return_value
     )
     mock_spotify.playlist_add_items.return_value = (
         mock_spotify_playlist_add_items.return_value
     )
     new_tracks = [("test_id", "track title - artist name")]
     ret = build_new_playlist(mock_spotify, "test_user", "r/techno", new_tracks)
     assert isinstance(ret, dict)
 
 
+@pytest.mark.asyncio
+@pytest.mark.parametrize("message", ["", "oops"])
+async def test_catch(message, caplog):
+    """Test for the catch function."""
+    exc = ZeroDivisionError("You can't divide by zero!")
+    class Generator:
+        """Dummy async generator class."""
+        def __init__(self):
+            self._iters = 2
+            self._i = 0
+
+        def __aiter__(self):
+            return self
+
+        async def __anext__(self):
+            if self._i >= self._iters:
+                raise StopAsyncIteration
+            self._i += 1
+            await asyncio.sleep(0.1)
+            if self._i % 2 == 0:
+                raise exc
+
+            return self._i
+
+    caplog.set_level("WARNING")
+    _ = [x async for x in catch(Generator(), message=message)]
+    assert caplog.records[0].message == (
+        f"{message}: {str(exc)}" if message else str(exc)
+    )
+
+
 @pytest.mark.parametrize("spotify_next_fails", [True, False])
 @mock.patch(
     "djtools.spotify.helpers.filter_tracks",
     return_value=[
         (
             {
                 "id": "some_id",
                 "name": "Arctic Oscillations",
                 "artists": [ 
                     {"name": "Fanu"},
                 ],
             },
-            "Arctic Oscillations - Fanu" 
+            100,
         )
     ],
 )
 @mock.patch("djtools.spotify.helpers.spotipy.Spotify")
-def test_filter_results(mock_spotify, mock_spotify_next, spotify_next_fails):
+def test_filter_results(mock_spotify, mock_filter_tracks, spotify_next_fails):
+    """Test for the filter_results function."""
     results = {
         "tracks": {
             "items": [
                 {
                     "track": {
                         "name": "Arctic Oscillations",
                         "artists": [ 
@@ -98,15 +134,15 @@
             ],
             "next": True,
         },
     }
     threshold = 100
     title = "Arctic Oscillations"
     artist = "Fanu"
-    mock_spotify.next.return_value = mock_spotify_next.return_value
+    mock_spotify.next.return_value = mock_filter_tracks.return_value
     with mock.patch(
         "djtools.spotify.helpers.spotipy.Spotify.next",
         return_value={
             "tracks": {
                 "items": [
                     {
                         "track": {
@@ -120,25 +156,29 @@
                 "next": False,
             },
         },
     ) as mock_spotify_next:
         if spotify_next_fails:
             mock_spotify_next.side_effect = Exception()
         ret = filter_results(mock_spotify, results, threshold, title, artist)
-    expected = {
-        "id": "some_id",
-        "name": "Arctic Oscillations",
-        "artists": [ 
-            {"name": "Fanu"},
-        ],
-    }
+    expected = (
+        {
+            "id": "some_id",
+            "name": "Arctic Oscillations",
+            "artists": [ 
+                {"name": "Fanu"},
+            ],
+        },
+        100,
+    )
     assert ret == expected
 
 
 def test_filter_tracks():
+    """Test for the filter_tracks function."""
     tracks = [
         {
             "name": "Arctic Oscillations",
             "artists": [ 
                 {"name": "Fanu"},
             ],
         },
@@ -157,15 +197,15 @@
         (
             {
                 "name": title,
                 "artists": [ 
                     {"name": artist},
                 ],
             },
-            threshold 
+            threshold * 2
         )
     ]
     assert ret == expected
 
 
 @pytest.mark.parametrize("match_result", [True, False])
 @pytest.mark.parametrize(
@@ -201,51 +241,56 @@
                 },
             ],
             "next": False,
         },
     },
 )
 def test_fuzzy_match(mock_spotify_search, mock_spotify, title, match_result):
+    """Test for the fuzzy_match function."""
     mock_spotify.search.return_value = mock_spotify_search.return_value
     threshold = 100
     with mock.patch(
         "djtools.spotify.helpers.parse_title",
         return_value=title,
     ), mock.patch(
         "djtools.spotify.helpers.filter_results",
-        return_value={
-            "id": "some_id",
-            "name": "Arctic Oscillations",
-            "artists": [ 
-                {"name": "Fanu"},
-            ],
-        } if match_result else None,
+        return_value=(
+            {
+                "id": "some_id",
+                "name": "Arctic Oscillations",
+                "artists": [ 
+                    {"name": "Fanu"},
+                ],
+            },
+            100,
+        ) if match_result else (None, 0),
     ) as mock_filter_results:
         ret = fuzzy_match(mock_spotify, title, threshold)
     if not all(x for x in title):
         assert not ret
     if not match_result:
         assert not ret
     if match_result and all(x for x in title):
         assert isinstance(ret, tuple)
         id_, match = ret
-        expected_ret = mock_filter_results.return_value
+        expected_ret = mock_filter_results.return_value[0]
         assert id_ == expected_ret["id"]
         artists = ", ".join([y["name"] for y in expected_ret["artists"]])
         assert match == f'{expected_ret["name"]} - {artists}'
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify.search",
     side_effect=Exception()
 )
 def test_fuzzy_match_handles_spotify_exception(
     mock_spotify_search, mock_spotify, caplog
 ):
+    """Test for the fuzzy_match function."""
     caplog.set_level("ERROR")
     mock_spotify.search.side_effect = mock_spotify_search.side_effect
     threshold = 100
     title = "Arctic Oscillations"
     artist = "Fanu"
     with mock.patch(
         "djtools.spotify.helpers.parse_title",
@@ -262,60 +307,63 @@
     "builtins.open",
     MockOpen(
         files=["spotify_playlists.yaml"],
         content="playlist: playlist-id",
     ).open
 )
 def test_get_playlist_ids():
+    """Test for the get_playlist_ids function."""
     playlist_ids = get_playlist_ids()
     assert isinstance(playlist_ids, dict)
 
 
 @mock.patch("djtools.spotify.helpers.praw.Reddit")
 def test_get_reddit_client(test_config):
+    """Test for the get_reddit_client function."""
     test_config.REDDIT_CLIENT_ID = "test_client_id"
     test_config.REDDIT_CLIENT_SECRET = "test_client_secret"
     test_config.REDDIT_USER_AGENT = "test_user_agent"
     get_reddit_client(test_config)
 
 
 @mock.patch("djtools.spotify.helpers.spotipy.Spotify")
 def test_get_spotify_client(test_config):
+    """Test for the get_spotify_client function."""
     test_config.SPOTIFY_CLIENT_ID = "test_client_id"
     test_config.SPOTIFY_CLIENT_SECRET = "test_client_secret"
     test_config.SPOTIFY_REDIRECT_URI = "test_redirect_uri"
     get_spotify_client(test_config)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("subreddit_type", ["hot", "top"])
 @pytest.mark.parametrize("num_subs", [5, 0])
-@mock.patch("djtools.spotify.helpers.praw.Reddit.close")
+@mock.patch("djtools.spotify.helpers.praw.Reddit.close", mock.Mock())
 @mock.patch("djtools.spotify.helpers.process")
 @mock.patch("djtools.spotify.helpers.praw.models.Submission")
 @mock.patch("djtools.spotify.helpers.praw.Reddit")
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 async def test_get_subreddit_posts(
     mock_spotify,
     mock_praw,
     mock_praw_submission,
     mock_process,
-    mock_praw_close,
     subreddit_type,
     num_subs,
     test_config,
     caplog,
 ):
+    """Test for the get_subreddit_posts function."""
     caplog.set_level("INFO")
     subreddit = SubredditConfig(name="techno", type=subreddit_type).dict()
     praw_cache = {}
     mock_praw_submission.id = "test_id"
     mock_process.return_value = "track - artist"
     with mock.patch(
-        "djtools.utils.helpers.catch",
+        "djtools.spotify.helpers.catch",
     ) as mock_catch, mock.patch(
         "djtools.spotify.helpers.praw.Reddit.subreddit",
         new=mock.AsyncMock(),
     ):
         mock_catch.return_value=aiter(mock_praw_submission, num_subs)
         await get_subreddit_posts(
             mock_spotify, mock_praw, subreddit, test_config, praw_cache
@@ -343,20 +391,21 @@
         "Arctic Oscillations - Fanu (this track is cool)",
         "Arctic Oscillations - Fanu [love this track]",
         "Fanu - Arctic Oscillations",
         "A submission title that doesn't include the artist or track info",
     ],
 )
 def test_parse_title(title):
+    """Test for the parse_title function."""
     split_chars = ["[", "("]
     ret = parse_title(title)
-    assert isinstance(ret, tuple)
+    assert isinstance(ret, list)
     if " - " in title:
         assert all(x for x in ret)
-        if any(x in title for x in split_chars): 
+        if any(x in title for x in split_chars):
             assert all(x not in r for x in split_chars for r in ret)
     else:
         assert not any(x for x in ret)
 
 
 @pytest.mark.parametrize("playlist_ids", [{}, {"playlist": "id"}])
 @pytest.mark.parametrize("tracks", [[], [("id", "title - artist")]])
@@ -369,14 +418,15 @@
     mock_update_existing_playlist,
     mock_build_new_playlist,
     mock_spotify_playlist,
     playlist_ids,
     tracks,
     caplog,
 ):
+    """Test for the populate_playlist function."""
     ret_val = {
         "name": "playlist",
         "external_urls": {"spotify": "https://test-url.com"},
         "id": "test-id",
     }
     mock_update_existing_playlist.return_value = ret_val
     mock_build_new_playlist.return_value = ret_val
@@ -402,16 +452,16 @@
         assert mock_build_new_playlist.call_count == 1
         assert playlist_name in ret_playlist_ids
     elif playlist_ids:
         assert mock_spotify_playlist.call_count == 1
 
     if not (playlist_ids or tracks):
         assert (
-            mock_update_existing_playlist.call_count == 
-            mock_build_new_playlist.call_count == 
+            mock_update_existing_playlist.call_count ==
+            mock_build_new_playlist.call_count ==
             mock_spotify_playlist.call_count == 0
         )
         assert len(caplog.records) == 0
     else:
         assert caplog.records.pop(0).message == (
             f'"{ret_val["name"]}": {ret_val["external_urls"].get("spotify")}'
         )
@@ -435,16 +485,17 @@
 )
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 @mock.patch(
     "djtools.spotify.helpers.praw.models.Submission",
     autospec=True
 )
 def test_process(mock_praw_submission, mock_spotipy, url, title):
+    """Test for the process function."""
     mock_praw_submission.url = url
-    mock_praw_submission.title = title 
+    mock_praw_submission.title = title
     with mock.patch(
         "djtools.spotify.helpers.fuzzy_match",
         return_value=(url, title)
     ):
         ret = process(mock_praw_submission, mock_spotipy, 50)
     assert isinstance(ret, tuple)
     assert ret == (url, title)
@@ -452,28 +503,29 @@
 
 @pytest.mark.parametrize(
     "playlist_track_names", [
         ["Arctic Oscillations - Fanu"], ["Not a Match - Some Artist"],
     ],
 )
 def test_track_name_too_similar(playlist_track_names, caplog):
+    """Test for the track_name_too_similar function."""
     caplog.set_level("WARNING")
     track = "Arctic Oscillations - Fanu"
     ret = track_name_too_similar(track, playlist_track_names)
     if any("Not a Match" in x for x in playlist_track_names):
         assert not ret
     else:
         assert ret
         assert caplog.records[0].message == (
             f'Candidate new track "{track}" is too similar to existing '
             f'track "{playlist_track_names[0]}"'
         )
 
 
-@pytest.mark.parametrize("track_name_too_similar", [True, False])
+@pytest.mark.parametrize("too_similar", [True, False])
 @mock.patch(
     "djtools.spotify.helpers.track_name_too_similar",
     return_value=None,
 )
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify."
     "playlist_add_items",
@@ -539,28 +591,29 @@
     mock_spotify,
     mock_spotify_playlist,
     mock_spotify_next,
     mock_spotify_track,
     mock_spotify_playlist_remove_specific_occurrences_of_items,
     mock_spotify_playlist_add_items,
     mock_track_name_too_similar,
-    track_name_too_similar,
+    too_similar,
     caplog,
 ):
+    """Test for the update_existing_playlist function."""
     caplog.set_level("WARNING")
     mock_spotify.playlist.return_value = mock_spotify_playlist.return_value
     mock_spotify.next.return_value = mock_spotify_next.return_value
     mock_spotify.track.return_value = mock_spotify_track.return_value
     mock_spotify.playlist_remove_specific_occurrences_of_items.return_value = (
         mock_spotify_playlist_remove_specific_occurrences_of_items.return_value
     )
     mock_spotify.playlist_add_items.return_value = (
         mock_spotify_playlist_add_items.return_value
     )
-    mock_track_name_too_similar.return_value = track_name_too_similar
+    mock_track_name_too_similar.return_value = too_similar
     playlist = ""
     new_tracks = [
         ("test_id", "test track"),
         ("unique_id", "another track"),
         ("https://open.spotify.com/track/1lps8esDJ9M6rG3HBjhuux", "a track"),
     ]
     limit = 1
@@ -574,8 +627,9 @@
     )
 
 
 @mock.patch(
     "builtins.open", MockOpen(files=["spotify_playlists.yaml"]).open
 )
 def test_write_playlist_ids():
-        write_playlist_ids({})
+    """Test for the write_playlist_ids function."""
+    write_playlist_ids({})
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.0b0/djtools/spotify/test_playlist_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Testing for the playlist_builder module."""
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.spotify.config import SubredditConfig
 from djtools.spotify.playlist_builder import (
@@ -14,48 +15,51 @@
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "playlist_subreddits", [[], [SubredditConfig(name="jungle").dict()]],
 )
 @pytest.mark.parametrize("got_playlist_ids", [True, False])
 @pytest.mark.parametrize("got_tracks", [True, False])
-@mock.patch.object(Path, "exists",return_value=True)
+@mock.patch.object(Path, "exists", mock.Mock(return_value=True))
 @mock.patch(
     "djtools.spotify.helpers.update_existing_playlist",
-    return_value={
-        "name": "test_playlist",
-        "external_urls": {"spotify": "https://test-url.com"},
-        "id": "test-id",
-    },
+    mock.Mock(
+        return_value={
+            "name": "test_playlist",
+            "external_urls": {"spotify": "https://test-url.com"},
+            "id": "test-id",
+        },
+    ),
 )
 @mock.patch(
     "djtools.spotify.helpers.build_new_playlist",
-    return_value={
-        "name": "test_playlist",
-        "external_urls": {"spotify": "https://test-url.com"},
-        "id": "test-id",
-    },
+    mock.Mock(
+        return_value={
+            "name": "test_playlist",
+            "external_urls": {"spotify": "https://test-url.com"},
+            "id": "test-id",
+        },
+    ),
 )
 @mock.patch(
     "djtools.spotify.playlist_builder.get_subreddit_posts",
     return_value=[
         [("track-id", "track name")], SubredditConfig(name="jungle").dict()],
 )
-@mock.patch("djtools.spotify.playlist_builder.get_spotify_client")
+@mock.patch(
+    "djtools.spotify.playlist_builder.get_spotify_client", mock.MagicMock()
+)
 async def test_async_update_auto_playlists(
-    mock_spotify,
     mock_get_subreddit_posts,
-    mock_build_new_playlist,
-    mock_update_existing_playlist,
-    mock_os_path_exists,
     got_tracks,
     got_playlist_ids,
     playlist_subreddits,
     test_config,
 ):
+    """Test for the async_update_auto_playlists function."""
     if not got_tracks:
         mock_get_subreddit_posts.return_value[0] = []
     test_config.SPOTIFY_CLIENT_ID = "test_client_id"
     test_config.SPOTIFY_CLIENT_SECRET = "test_client_secret"
     test_config.SPOTIFY_REDIRECT_URI = "test_redirect_uri"
     test_config.AUTO_PLAYLIST_SUBREDDITS = playlist_subreddits
     with mock.patch(
@@ -66,65 +70,72 @@
         ).open
     ):
         await async_update_auto_playlists(test_config)
 
 
 @mock.patch(
     "djtools.spotify.playlist_builder.filter_results",
-    return_value={
-        "id": "some_id",
-        "name": "some_name",
-        "artists": [ 
-            {"name": "some_artist"},
-        ],
-    }
+    mock.Mock(
+        return_value=(
+            {
+                "id": "some_id",
+                "name": "some_name",
+                "artists": [ 
+                    {"name": "some_artist"},
+                ],
+            },
+            100,
+        )
+    ),
 )
 @mock.patch(
     "djtools.spotify.playlist_builder.populate_playlist",
-    return_value={"some-playlist": "some-id"},
+    mock.Mock(
+        return_value={"some-playlist": "some-id"},
+    ),
+)
+@mock.patch(
+    "djtools.spotify.playlist_builder.get_spotify_client", mock.MagicMock()
 )
-@mock.patch("djtools.spotify.playlist_builder.get_spotify_client")
 @mock.patch(
     "pyperclip.paste",
     return_value="""aweeeezy/Bass/2022-09-03: 5
                    Brazil - A.M.C.mp3
                    Endless Haze - Koherent.mp3
                    Two Rangers - Two Rangers.mp3
                    Under Pressure - Alix Perez, T-Man.mp3
                    zoom.1 - Relativity Lounge, wicker's portal.mp3
                   aweeeezy/House/2022-09-03: 2
                    Shirt - Cour T..mp3
                    UNKNOWN - 1 - Unknown Artist.mp3""",
 )
-def test_playlist_from_upload(
-    mock_spotify,
-    mock_populate_playlist,
-    mock_filter_results,
-    test_config,
-    tmpdir,
-):
+def test_playlist_from_upload(test_config):
+    """Test for the playlist_from_upload function."""
     test_config.SPOTIFY_CLIENT_ID = "test_client_id"
     test_config.SPOTIFY_CLIENT_SECRET = "test_client_secret"
     test_config.SPOTIFY_REDIRECT_URI = "test_redirect_uri"
     test_config.PLAYLIST_FROM_UPLOAD = True
     with mock.patch(
         "builtins.open",
         MockOpen(files=["spotify_playlists.yaml"], content="{}").open
     ):
         playlist_from_upload(test_config)
 
 
 @mock.patch(
     "djtools.spotify.playlist_builder.filter_results",
-    return_value={},
+    mock.Mock(
+        return_value=({}, 100),
+    ),
 )
-@mock.patch("djtools.spotify.playlist_builder.get_spotify_client")
-def test_playlist_from_upload_handles_non_match(
-    mock_spotify, mock_filter_results, test_config, caplog
-):
+@mock.patch(
+    "djtools.spotify.playlist_builder.get_spotify_client", mock.MagicMock()
+)
+def test_playlist_from_upload_handles_non_match(test_config, caplog):
+    """Test for the playlist_from_upload function."""
     caplog.set_level("WARNING")
     title = "Under Pressure"
     artist = "Alix Perez, T-Man"
     test_config.PLAYLIST_FROM_UPLOAD = True
     with mock.patch(
         "builtins.open",
         MockOpen(files=["spotify_playlists.yaml"], content="{}").open
@@ -143,14 +154,15 @@
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify.search",
     side_effect=Exception()
 )
 def test_playlist_from_upload_handles_spotify_exception(
     mock_spotify_search, mock_spotify, test_config, caplog
 ):
+    """Test for the playlist_from_upload function."""
     caplog.set_level("ERROR")
     mock_spotify.return_value.search.side_effect = (
         mock_spotify_search.side_effect
     )
     title = "Under Pressure"
     artist = "Alix Perez, T-Man"
     test_config.PLAYLIST_FROM_UPLOAD = True
@@ -169,25 +181,25 @@
     assert caplog.records[0].message.startswith(
         f'Error searching for "{title} - {artist}"'
     )
 
 
 @mock.patch("pyperclip.paste", return_value="")
 def test_playlist_from_upload_raises_runtimeerror(test_config):
+    """Test for the playlist_from_upload function."""
     test_config.PLAYLIST_FROM_UPLOAD = True
     with pytest.raises(
         RuntimeError,
         match="Generating a Spotify playlist from an upload requires output "
             "from an upload_music Discord webhook to be copied to the "
             "system's clipboard"
     ):
         playlist_from_upload(test_config)
 
 
 @mock.patch(
     "djtools.spotify.playlist_builder.async_update_auto_playlists",
-    return_value=lambda x: None,
+    mock.AsyncMock(return_value=lambda x: None),
 )
-def test_update_auto_playlists(
-    mock_async_update_auto_playlists, test_config
-):
+def test_update_auto_playlists(test_config):
+    """Test for the update_auto_playlists function."""
     update_auto_playlists(test_config)
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/__init__.py` & `dj_beatcloud-2.5.0b0/djtools/sync/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """The `sync` package contains modules:
     * `config`: the configuration object for the `sync` package
     * `helpers`: helper functions for the `sync_operations` module
     * `sync_operations`: for syncing audio and Rekordbox XML files to the
         Beatcloud
 """
-from .config import SyncConfig
-from .helpers import upload_log
-from .sync_operations import (
+from djtools.sync.config import SyncConfig
+from djtools.sync.helpers import upload_log
+from djtools.sync.sync_operations import (
     download_music, download_xml, upload_music, upload_xml
 )
 
 
 SYNC_OPERATIONS = {
     'DOWNLOAD_MUSIC': download_music,
     'DOWNLOAD_XML': download_xml,
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/config.py` & `dj_beatcloud-2.5.0b0/djtools/sync/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """This module contains the configuration object for the sync package.
 The attributes of this configuration object correspond with the "sync" key
 of config.yaml
 """
 import getpass
 import logging
 from pathlib import Path
-from typing import List, Union
+from typing import List, Optional, Union
 
 from pydantic import validator
 import yaml
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 class SyncConfig(BaseConfig):
     """Configuration object for the sync package."""
 
-    AWS_USE_DATE_MODIFIED: bool = False 
+    AWS_USE_DATE_MODIFIED: bool = False
     DISCORD_URL: str = ""
     DOWNLOAD_EXCLUDE_DIRS: List[Path] = []
     DOWNLOAD_INCLUDE_DIRS: List[Path] = []
-    DOWNLOAD_MUSIC: bool = False 
+    DOWNLOAD_MUSIC: bool = False
     DOWNLOAD_SPOTIFY: str = ""
-    DOWNLOAD_XML: bool = False 
+    DOWNLOAD_XML: bool = False
     DRYRUN: bool = False
     IMPORT_USER: str = ""
     UPLOAD_EXCLUDE_DIRS: List[Path] = []
     UPLOAD_INCLUDE_DIRS: List[Path] = []
-    UPLOAD_MUSIC: bool = False 
-    UPLOAD_XML: bool = False 
-    USB_PATH: str = ""
+    UPLOAD_MUSIC: bool = False
+    UPLOAD_XML: bool = False
+    USB_PATH: Optional[Union[str, Path]] = None
     USER: str = ""
 
     def __init__(self, *args, **kwargs):
         """Constructor.
 
         Raises:
             ValueError: Both include and exclude dirs can't be provided at the
@@ -57,42 +57,39 @@
             msg = (
                 "Config must neither contain both UPLOAD_INCLUDE_DIRS and "
                 "UPLOAD_EXCLUDE_DIRS or both DOWNLOAD_INCLUDE_DIRS and "
                 "DOWNLOAD_EXCLUDE_DIRS"
             )
             logger.critical(msg)
             raise ValueError(msg)
-        
+
         if any(
             [
                 self.DOWNLOAD_MUSIC,
                 self.DOWNLOAD_XML,
                 self.UPLOAD_MUSIC,
                 self.UPLOAD_XML,
             ]
         ):
             if not self.AWS_PROFILE:
                 msg = "Config must include AWS_PROFILE for sync operations"
                 logger.critical(msg)
                 raise RuntimeError(msg)
-        
+
         if (
-            any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and not
-            (
-                self.USB_PATH if isinstance(self.USB_PATH, str)
-                else self.USB_PATH.exists()
-            )
+            any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and
+            (not self.USB_PATH or not self.USB_PATH.exists())
         ):
             msg = (
                 "Config must include USB_PATH for both DOWNLOAD_MUSIC and "
                 "UPLOAD_MUSIC sync operations"
             )
             logger.critical(msg)
             raise RuntimeError(msg)
-        
+
         if self.UPLOAD_MUSIC and not self.DISCORD_URL:
             logger.warning(
                 'DISCORD_URL is not configured...set this for "New Music" '
                 "discord messages!"
             )
 
         registered_users_path = (
@@ -128,17 +125,18 @@
 
         # Enter USER into "registered_users.yaml".
         registered_users[self.USER] = str(self.USB_PATH)
         with open(registered_users_path, mode="w", encoding="utf-8") as _file:
             yaml.dump(registered_users, _file)
 
     @validator("USB_PATH")
-    def usb_path_as_pathlib_path(cls, v: str) -> Union[Path, str]:
-        """_summary_
+    @classmethod
+    def usb_path_as_pathlib_path(cls, value: str) -> Union[Path, str]:
+        """Validator to convert USB_PATH to a pathlib.Path.
 
         Args:
-            v: USB_PATH field
+            value: USB_PATH field
 
         Returns:
             pathlib.Path representing the USB_PATH field or else an empty string.
         """
-        return v if not v else Path(v)
+        return value if not value else Path(value)
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/sync/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 def parse_sync_command(
     _cmd: str, config: BaseConfig, upload: Optional[bool] = False,
 ) -> str:
     """Appends flags to "aws s3 sync" command. If "*_INCLUDE_DIRS" is
         specified, all directories are ignored except those specified. If
         "*_EXCLUDE_DIRS" is specified, all directories are included except
         those specified. Only one of these can be specified at once. If
-        "AWS_USE_DATE_MODIFIED", then tracks will be redownloaded / reuploaded
-        if their date modified at the source is after that of the destination.
+        "AWS_USE_DATE_MODIFIED", then tracks will be
+        re-downloaded / re-uploaded if their date modified at the source is
+        after that of the destination.
 
     Args:
         _cmd: Partial "aws s3 sync" command.
         config: Configuration object.
         upload: Whether uploading or downloading.
 
     Returns:
@@ -150,15 +151,15 @@
             proc.stdout.close()
             return_code = proc.wait()
         if return_code:
             raise CalledProcessError(return_code, " ".join(_cmd))
     except Exception as exc:
         msg = f"Failure while syncing: {exc}"
         logger.critical(msg)
-        raise Exception(msg)
+        raise Exception(msg) from exc
 
     new_music = ""
     if tracks:
         logger.info(
             f'Successfully {"down" if "s3://" in _cmd[3] else "up"}loaded the '
             "following tracks:"
         )
@@ -191,15 +192,16 @@
             "AWS_PROFILE"
         )
         return
 
     dst = f"s3://dj.beatcloud.com/dj/logs/{config.USER}/{log_file.name}"
     cmd = f"aws s3 cp {log_file.as_posix()} {dst}"
     logger.info(cmd)
-    Popen(cmd, shell=True).wait()
+    with Popen(cmd, shell=True) as proc:
+        proc.wait()
 
     now = datetime.now()
     one_day = timedelta(days=1)
     for _file in log_file.parent.rglob("*"):
         if _file.name == "empty.txt":
             continue
         if _file.lstat().st_mtime < (now - one_day).timestamp():
@@ -237,10 +239,10 @@
             except IndexError:
                 break
             index -= 1
         remainder = batch[index+1:] + remainder
         batch = batch[:index+1]
 
         if batch:
-            requests.post(url, json={"content": batch})
+            requests.post(url, json={"content": batch}, timeout=10)
             batch = remainder[:content_size_limit]
             remainder = remainder[content_size_limit:]
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.0b0/djtools/sync/sync_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """This module is responsible for syncing tracks between "USB_PATH" and the
-beatcloud (upload and download). It also handles uploading the Rekordbox XML
+Beatcloud (upload and download). It also handles uploading the Rekordbox XML
 located at "XML_PATH" and downloading the Rekordbox XML uploaded to the
-beatcloud by "IMPORT_USER" before modifying it to point to track locations at
+Beatcloud by "IMPORT_USER" before modifying it to point to track locations at
 "USB_PATH".
 """
 import logging
 from os.path import getmtime
 from pathlib import Path
 from subprocess import Popen
-from typing import List
+from typing import List, Optional
 
 from djtools.configs.config import BaseConfig
 from djtools.sync.helpers import (
     parse_sync_command, rewrite_xml, run_sync, webhook
 )
 from djtools.utils.check_tracks import compare_tracks
 
 
 logger = logging.getLogger(__name__)
 
 
-def download_music(config: BaseConfig, beatcloud_tracks: List[str] = []):
-    """This function syncs tracks from the beatcloud to "USB_PATH".
+def download_music(config: BaseConfig, beatcloud_tracks: Optional[List[str]] = None):
+    """This function syncs tracks from the Beatcloud to "USB_PATH".
 
     If "DOWNLOAD_SPOTIFY" is set to a playlist name that exists in
     "spotify_playlists.yaml", then "DOWNLOAD_INCLUDE_DIRS" will be populated
     with tracks in that playlist that match Beatcloud tracks.
 
     Args:
         config: Configuration object.
@@ -58,20 +58,20 @@
 
     new = {str(p) for p in dest.rglob(glob_path)}
     difference = sorted(list(new.difference(old)), key=getmtime)
     if difference:
         logger.info(f"Found {len(difference)} new files")
         for diff in difference:
             logger.info(f"\t{diff}")
-    
+
     return beatcloud_tracks
 
 
 def download_xml(config: BaseConfig):
-    """This function downloads the beatcloud XML of "IMPORT_USER" and modifies
+    """This function downloads the Beatcloud XML of "IMPORT_USER" and modifies
         the "Location" field of all the tracks so that it points to USER's
         "USB_PATH".
 
     Args:
         config: Configuration object.
     """
     logger.info("Syncing remote rekordbox.xml...")
@@ -79,23 +79,24 @@
     xml_dir.mkdir(parents=True, exist_ok=True)
     _file = Path(xml_dir) / f'{config.IMPORT_USER}_rekordbox.xml'
     cmd = (
         "aws s3 cp s3://dj.beatcloud.com/dj/xml/"
         f'{config.IMPORT_USER}/rekordbox.xml {_file}'
     )
     logger.info(cmd)
-    Popen(cmd, shell=True).wait()
+    with Popen(cmd, shell=True) as proc:
+        proc.wait()
     if config.USER != config.IMPORT_USER:
         rewrite_xml(config)
 
 
 def upload_music(config: BaseConfig):
-    """This function syncs tracks from "USB_PATH" to the beatcloud.
-        "AWS_USE_DATE_MODIFIED" can be used in order to reupload tracks that
-        already exist in the beatcloud but have been modified since the last
+    """This function syncs tracks from "USB_PATH" to the Beatcloud.
+        "AWS_USE_DATE_MODIFIED" can be used in order to re-upload tracks that
+        already exist in the Beatcloud but have been modified since the last
         time they were uploaded (i.e. ID3 tags have been altered).
 
     Args:
         config: Configuration object.
     """
     hidden_files = set(
         (Path(config.USB_PATH) / "DJ Music").rglob(
@@ -118,17 +119,18 @@
             content=run_sync(parse_sync_command(cmd, config, upload=True)),
         )
     else:
         run_sync(parse_sync_command(cmd, config, upload=True))
 
 
 def upload_xml(config: BaseConfig):
-    """This function uploads "XML_PATH" to beatcloud.
+    """This function uploads "XML_PATH" to Beatcloud.
 
     Args:
         config: Configuration object.
     """
     logger.info(f"Uploading {config.USER}'s rekordbox.xml...")
     dst = f"s3://dj.beatcloud.com/dj/xml/{config.USER}/"
     cmd = f"aws s3 cp {config.XML_PATH} {dst}"
     logger.info(cmd)
-    Popen(cmd, shell=True).wait()
+    with Popen(cmd, shell=True) as proc:
+        proc.wait()
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/test_config.py` & `dj_beatcloud-2.5.0b0/djtools/sync/test_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pathlib import Path
+"""Testing for the config module."""
 from unittest import mock
 
 import getpass
 import pytest
 
 
 from djtools.sync.config import SyncConfig
@@ -13,14 +13,15 @@
     "builtins.open",
     MockOpen(
         files=["registered_users.yaml"],
         content="bad:\tfile",
     ).open,
 )
 def test_syncconfig_bad_registered_users():
+    """Test for the SyncConfig class."""
     with pytest.raises(
         RuntimeError,
         match="Error reading registered_users.yaml",
     ):
         SyncConfig()
 
 
@@ -28,14 +29,15 @@
     "builtins.open",
     MockOpen(files=["registered_users.yaml"],
     write_only=True).open,
 )
 @pytest.mark.parametrize("operations", [(True, False), (False, True)])
 @pytest.mark.parametrize("usb_path", ["", "nonexistent/path"])
 def test_syncconfig_download_or_upload_without_usb_path(operations, usb_path):
+    """Test for the SyncConfig class."""
     download, upload = operations
     cfg = {
         "AWS_PROFILE": "myprofile",
         "DOWNLOAD_MUSIC": download,
         "UPLOAD_MUSIC": upload,
         "USB_PATH": usb_path,
     }
@@ -46,14 +48,15 @@
             "UPLOAD_MUSIC sync operations"
         ),
     ):
         SyncConfig(**cfg)
 
 
 def test_syncconfig_download_without_import_user():
+    """Test for the SyncConfig class."""
     cfg = {
         "DOWNLOAD_XML": True,
         "AWS_PROFILE": "myprofile",
         "IMPORT_USER": "not a valid user",
     }
     with pytest.raises(
         RuntimeError,
@@ -62,27 +65,29 @@
             f'"{cfg["IMPORT_USER"]}"'
         ),
     ):
         SyncConfig(**cfg)
 
 
 def test_syncconfig_mutually_exclusive_dirs():
+    """Test for the SyncConfig class."""
     cfg = {"UPLOAD_INCLUDE_DIRS": ["test"], "UPLOAD_EXCLUDE_DIRS": ["test"]}
     with pytest.raises(
         ValueError,
         match=(
             "Config must neither contain both UPLOAD_INCLUDE_DIRS and "
             "UPLOAD_EXCLUDE_DIRS or both DOWNLOAD_INCLUDE_DIRS and "
             "DOWNLOAD_EXCLUDE_DIRS"
         ),
     ):
         SyncConfig(**cfg)
 
 
 def test_syncconfig_no_aws_profile():
+    """Test for the SyncConfig class."""
     cfg = {"AWS_PROFILE": "", "UPLOAD_XML": True}
     with pytest.raises(
         RuntimeError,
         match="Config must include AWS_PROFILE for sync operations"
     ):
         SyncConfig(**cfg)
 
@@ -92,18 +97,17 @@
     lambda path: mock_exists([("registered_users.yaml", False)], path)
 )
 @mock.patch(
     "builtins.open",
     MockOpen(files=["registered_users.yaml"],
     write_only=True).open,
 )
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
-def test_syncconfig_no_registered_users(
-    mock_get_spotify_client, test_xml, caplog
-):
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.MagicMock())
+def test_syncconfig_no_registered_users(test_xml, caplog):
+    """Test for the SyncConfig class."""
     cfg = {
         "XML_PATH": test_xml,
         "SPOTIFY_CLIENT_ID": "id",
         "SPOTIFY_CLIENT_SECRET": "secret",
         "SPOTIFY_REDIRECT_URI": "uri",
         "SPOTIFY_USERNAME": "name",
     }
@@ -114,29 +118,29 @@
 
 @mock.patch(
     "builtins.open",
     MockOpen(files=["registered_users.yaml"],
     write_only=True).open,
 )
 def test_syncconfig_set_user():
+    """Test for the SyncConfig class."""
     cfg = {"USER": ""}
     assert not SyncConfig.__fields__["USER"].default
     sync_config = SyncConfig(**cfg)
     assert sync_config.USER == getpass.getuser()
 
 
 @mock.patch(
     "builtins.open",
     MockOpen(files=["registered_users.yaml"],
     write_only=True).open,
 )
-@mock.patch("djtools.spotify.helpers.get_spotify_client")
-def test_syncconfig_upload_without_discord_url(
-    mock_get_spotify_client, test_xml, caplog
-):
+@mock.patch("djtools.spotify.helpers.get_spotify_client", mock.MagicMock())
+def test_syncconfig_upload_without_discord_url(test_xml, caplog):
+    """Test for the SyncConfig class."""
     caplog.set_level("WARNING")
     cfg = {
         "USB_PATH": ".",
         "UPLOAD_MUSIC": True,
         "DISCORD_URL": "",
         "XML_PATH": test_xml,
         "SPOTIFY_CLIENT_ID": "id",
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/sync/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+"""Testing for the helpers module."""
 from datetime import datetime, timedelta
 import os
 from pathlib import Path
-import shutil
 import tempfile
 from unittest import mock
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.sync.helpers import (
@@ -28,14 +28,15 @@
     test_config,
     upload,
     include_dirs,
     exclude_dirs,
     use_date_modified,
     dryrun,
 ):
+    """Test for the parse_sync_command function."""
     tmpdir = str(tmpdir)
     if upload:
         test_config.UPLOAD_INCLUDE_DIRS = include_dirs
         test_config.UPLOAD_EXCLUDE_DIRS = exclude_dirs
     else:
         test_config.DOWNLOAD_INCLUDE_DIRS = include_dirs
         test_config.DOWNLOAD_EXCLUDE_DIRS = exclude_dirs
@@ -67,53 +68,57 @@
     MockOpen(
         files=["registered_users.yaml"],
         user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
         user_b=("other_user", "/Volumes/my_beat_stick/"),
     ).open
 )
 def test_rewrite_xml(test_config, test_xml, xml):
+    """Test for the rewrite_xml function."""
     user_a_path= "/Volumes/AWEEEEZY/"
     user_b_path= "/Volumes/my_beat_stick/"
     test_user = "aweeeezy"
     other_user = "other_user"
     test_config.USER = test_user
     test_config.IMPORT_USER = other_user
     test_config.XML_PATH = test_xml
     other_users_xml = Path(test_xml).parent / f"{other_user}_rekordbox.xml"
-    other_users_xml.write_text(Path(test_xml).read_text())
+    other_users_xml.write_text(
+        Path(test_xml).read_text(encoding="utf-8"), encoding="utf-8"
+    )
 
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
         # NOTE(a-rich): `Location` attributes in the XML's `TRACK` tags always
         # have unix-style paths so paths created in Windows must be
-        # interpretted `.as_posix()`.
+        # interpreted `.as_posix()`.
         track["Location"] = (
             Path(track["Location"]).parent / user_b_path.strip("/") /
             Path(track["Location"]).name
         ).as_posix()
-    
+
     with open(
         other_users_xml, mode="wb", encoding=xml.orignal_encoding
     ) as _file:
         _file.write(xml.prettify("utf-8"))
-        
+
     rewrite_xml(test_config)
 
     with open(other_users_xml, mode="r", encoding="utf-8") as _file:
         soup = BeautifulSoup(_file.read(), "xml")
         for track in soup.find_all("TRACK"):
             if not track.get("Location"):
                 continue
             assert user_a_path in track["Location"]
             assert user_b_path not in track["Location"]
 
 
 @mock.patch("djtools.sync.helpers.Popen")
 def test_run_sync(mock_popen, tmpdir):
+    """Test for the run_sync function."""
     with open(Path(tmpdir) / "track.mp3", mode="w", encoding="utf-8") as _file:
         _file.write("")
     cmd = ["aws", "s3", "sync", str(tmpdir), "s3://dj.beatcloud.com/dj/music/"]
     sync_output = (
         "upload: ../../Volumes/AWEEEEZY/DJ Music/Bass/2022-12-21/track - "
             "artist.mp3 to s3://dj.beatcloud.com/dj/music/Bass/2022-12-21/"
             "track - artist.mp3\n"
@@ -125,87 +130,89 @@
             "2022-12-22/last track - last artist.mp3"
         "\nirrelevant line"
     )
     # NOTE(a-rich): Windows does not allow opening a temporary file after it's
     # been created. The WAR is to initialize a `NamedTemporaryFile` with the
     # `delete` argument set to `False` and explicitly `.close()` the object
     # before calling `open()` on it.
-    tmp_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
-    tmp_file.write(sync_output)
-    tmp_file.seek(0)
-    tmp_file.close()
-    tmp_file = open(tmp_file.name)
-    process = mock_popen.return_value.__enter__.return_value
-    process.stdout = tmp_file
-    process.wait.return_value = 0
-    ret = run_sync(cmd)
+    with tempfile.NamedTemporaryFile(mode="w", delete=False) as tmp_file:
+        tmp_file.write(sync_output)
+        tmp_file.seek(0)
+        tmp_file.close()
+        with open(tmp_file.name, encoding="utf-8") as tmp_file:
+            process = mock_popen.return_value.__enter__.return_value
+            process.stdout = tmp_file
+            process.wait.return_value = 0
+            ret = run_sync(cmd)
     expected = (
         "Bass/2022-12-21: 1\n\ttrack - artist.mp3\nBass/2O22-12-21: 1\n\tother"
         " track - other artist.mp3\nTechno/2022-12-22: 1\n\tlast track - last "
         "artist.mp3\n"
     )
     assert ret == expected
 
 
 @mock.patch("djtools.sync.helpers.Popen")
 def test_run_sync_handles_return_code(mock_popen, tmpdir, caplog):
+    """Test for the run_sync function."""
     caplog.set_level("CRITICAL")
     # NOTE(a-rich): subprocess calls to `awscli` need to have unix-style path
     # arguments.
     cmd = [
         "aws",
         "s3",
         "sync",
         Path(tmpdir).as_posix(),
         "s3://dj.beatcloud.com/dj/music/",
     ]
-    tmp_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
-    tmp_file.write("")
-    tmp_file.seek(0)
-    tmp_file.close()
-    tmp_file = open(tmp_file.name)
-    process = mock_popen.return_value.__enter__.return_value
-    process.stdout = tmp_file
-    process.wait.return_value = 1
-    msg = (
-        f"Failure while syncing: Command '{' '.join(cmd)}' returned "
-        f"non-zero exit status {process.wait.return_value}."
-    )
-    with pytest.raises(Exception, match=msg):
-        run_sync(cmd)
+    with tempfile.NamedTemporaryFile(mode="w", delete=False) as tmp_file:
+        tmp_file.write("")
+        tmp_file.seek(0)
+        tmp_file.close()
+        with open(tmp_file.name, encoding="utf-8") as tmp_file:
+            process = mock_popen.return_value.__enter__.return_value
+            process.stdout = tmp_file
+            process.wait.return_value = 1
+            msg = (
+                f"Failure while syncing: Command '{' '.join(cmd)}' returned "
+                f"non-zero exit status {process.wait.return_value}."
+            )
+            with pytest.raises(Exception, match=msg):
+                run_sync(cmd)
     assert caplog.records[0].message == msg
 
 
-@mock.patch("subprocess.Popen.wait")
-def test_upload_log(mock_subprocess, tmpdir, test_config):
+@mock.patch("subprocess.Popen.wait", mock.Mock())
+def test_upload_log(tmpdir, test_config):
+    """Test for the upload_log function."""
     test_config.AWS_PROFILE = "DJ"
     now = datetime.now()
     one_day_ago = now - timedelta(days=1)
     test_log = f'{now.strftime("%Y-%m-%d")}.log'
     filenames = [
         "empty.txt",
-        test_log, 
+        test_log,
         f'{one_day_ago.strftime("%Y-%m-%d")}.log',
     ]
     ctime = one_day_ago.timestamp()
     for filename in filenames:
         file_path = Path(tmpdir) / filename
         with open(file_path, mode="w", encoding="utf-8") as _file:
             _file.write("stuff")
-        if filename != test_log: 
+        if filename != test_log:
             os.utime(file_path, (ctime, ctime))
     upload_log(test_config, Path(tmpdir) / test_log)
     assert len(list(Path(tmpdir).iterdir())) == len(filenames) - 1
 
 
 def test_upload_log_no_aws_profile(test_config, caplog):
+    """Test for the upload_log function."""
     caplog.set_level("WARNING")
     test_config.AWS_PROFILE = ""
-    ret = upload_log(test_config, "some_file.txt")
-    assert ret is None
+    upload_log(test_config, "some_file.txt")
     assert (
         caplog.records[0].message == "Logs cannot be backed up without "
         "specifying the config option AWS_PROFILE"
     )
 
 
 @pytest.mark.parametrize(
@@ -215,23 +222,24 @@
         "*"*2001,
         "*"*1900 + "\n" + "*"*99,
         "*"*1900 + "\n" + "*"*100,
     ],
 )
 @mock.patch("requests.post", side_effect=lambda *args, **kwargs: None)
 def test_webhook(mock_post, content):
+    """Test for the webhook function."""
     url = "https://discord.com/api/webhooks/some-id/"
     content_size_limit = 2000
     posts = len(content) // content_size_limit
     remainder = len(content) % content_size_limit
     posts = posts + 1 if remainder else posts
     webhook(url=url, content_size_limit=content_size_limit, content=content)
     assert mock_post.call_count == max(posts, len(content.split("\n")))
 
 
 def test_webhook_no_content(caplog):
+    """Test for the webhook function."""
     caplog.set_level("INFO")
     url = "https://discord.com/api/webhooks/some-id/"
     content = ""
-    ret = webhook(url=url, content=content)
-    assert not ret
+    webhook(url=url, content=content)
     assert caplog.records[0].message == "There's no content"
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.0b0/djtools/sync/test_sync_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,53 @@
+"""Testing for the sync_operations module."""
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.sync.sync_operations import (
     download_music, download_xml, upload_music, upload_xml
 )
 from djtools.utils.helpers import MockOpen
 
 
 @pytest.mark.parametrize("playlist_name", ["", "playlist Uploads"])
 @mock.patch(
     "djtools.sync.sync_operations.compare_tracks",
-    return_value=(
-        ["file.mp3"],
-        ["playlist/file.mp3"],
+    mock.Mock(
+        return_value=(
+            ["file.mp3"],
+            ["playlist/file.mp3"],
+        ),
     ),
 )
-def test_download_music(
-    mock_compare_tracks, playlist_name, test_config, tmpdir, caplog
-):
+def test_download_music(playlist_name, test_config, tmpdir, caplog):
+    """Test for the download_music function."""
     caplog.set_level("INFO")
     test_config.USB_PATH = tmpdir
     test_config.DOWNLOAD_SPOTIFY = playlist_name
     write_path = Path(tmpdir) / "DJ Music" / "file.mp3"
     cmd = [
         "aws",
         "s3",
         "sync",
         "s3://dj.beatcloud.com/dj/music/",
         write_path.parent.as_posix(),
     ]
     if playlist_name:
         cmd += ["--exclude", "*", "--include", "playlist/file.mp3"]
     cmd += ["--size-only"]
+
+    def dummy_func():
+        with open(write_path, mode="w", encoding="utf-8") as _file:
+            _file.write("")
+
     with mock.patch(
         "djtools.sync.sync_operations.run_sync",
-        side_effect=lambda *args, **kwargs: open(
-            write_path, mode="w", encoding="utf-8",
-        ).write("") 
+        side_effect=lambda *args, **kwargs: dummy_func()
     ) as mock_run_sync:
         download_music(test_config)
         mock_run_sync.assert_called_with(cmd)
     assert caplog.records[0].message == "Found 0 files"
     assert caplog.records[1].message == "Syncing remote track collection..."
     assert caplog.records[2].message == " ".join(cmd)
     assert caplog.records[3].message == "Found 1 new files"
@@ -54,51 +59,51 @@
     MockOpen(
         files=["registered_users.yaml"],
         user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
         user_b=("test_user", "/test/USB/"),
     ).open,
 )
 @mock.patch("djtools.sync.sync_operations.rewrite_xml")
-@mock.patch("subprocess.Popen.wait")
-def test_download_xml(
-    mock_subprocess, mock_rewrite_xml, test_config, test_xml, caplog
-):
+@mock.patch("subprocess.Popen.wait", mock.Mock())
+def test_download_xml(mock_rewrite_xml, test_config, test_xml, caplog):
+    """Test for the download_xml function."""
     caplog.set_level("INFO")
     test_user = "test_user"
     other_user = "aweeeezy"
     test_xml = Path(test_xml)
     new_xml = test_xml.parent / f"{other_user}_rekordbox.xml"
-    new_xml.write_text(test_xml.read_text())
+    new_xml.write_text(test_xml.read_text(encoding="utf-8"), encoding="utf-8")
     test_config.USER = test_user
     test_config.IMPORT_USER = other_user
     test_config.XML_PATH = test_xml
     download_xml(test_config)
     cmd = [
         "aws",
         "s3",
         "cp",
         f's3://dj.beatcloud.com/dj/xml/{other_user}/rekordbox.xml',
         # NOTE(a-rich): since we could be passing a `test_xml` formatted as a
         # WindowsPath, the comparison needs to be made with `str(new_xml)`
         # (rather than `new_xml.as_posix()`).
         str(new_xml),
-    ] 
+    ]
     assert caplog.records[0].message == "Syncing remote rekordbox.xml..."
     assert caplog.records[1].message == " ".join(cmd)
     mock_rewrite_xml.assert_called_once()
 
 
 @pytest.mark.parametrize(
     "discord_url", ["", "https://discord.com/api/webhooks/some-id/"]
 )
 @mock.patch("djtools.sync.sync_operations.run_sync", return_value=None)
 @mock.patch("djtools.sync.sync_operations.webhook", return_value=None)
 def test_upload_music(
     mock_webhook, mock_run_sync, discord_url, tmpdir, test_config, caplog
 ):
+    """Test for the upload_music function."""
     caplog.set_level("INFO")
     test_config.USB_PATH = tmpdir
     test_config.DISCORD_URL = discord_url
     test_dir = Path(tmpdir) / "DJ Music"
     test_dir.mkdir(parents=True, exist_ok=True)
     for file_name in [".test_file.mp3", "test_file.mp3"]:
         with open(test_dir / file_name, mode="w", encoding="utf-8") as file_:
@@ -120,16 +125,17 @@
     mock_run_sync.assert_called_with(cmd)
     if discord_url:
         mock_webhook.assert_called_with(
             "https://discord.com/api/webhooks/some-id/", content=None
         )
 
 
-@mock.patch("subprocess.Popen.wait")
-def test_upload_xml(mock_subprocess, test_config, test_xml, caplog):
+@mock.patch("subprocess.Popen.wait", mock.Mock())
+def test_upload_xml(test_config, test_xml, caplog):
+    """Test for the upload_xml function."""
     caplog.set_level("INFO")
     test_user = "test_user"
     test_config.USER = test_user
     test_config.XML_PATH = test_xml
     cmd = f"aws s3 cp {test_xml} s3://dj.beatcloud.com/dj/xml/{test_user}/"
     upload_xml(test_config)
     assert caplog.records[0].message == (
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.0b0/djtools/utils/check_tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 def compare_tracks(
     config: BaseConfig,
-    beatcloud_tracks: Optional[List[str]] = [],
+    beatcloud_tracks: Optional[List[str]] = None,
     download_spotify_playlist: Optional[str] = "",
 ) -> Tuple[List[str], List[str]]:
     """Compares tracks from Spotify / local with Beatcloud tracks.
     
     Gets track titles and artists from Spotify playlist(s) and / or file names
     from local directories, and get file names from the beatcloud. Then compute
     the Levenshtein similarity between their product in order to identify any
@@ -65,30 +65,30 @@
             track_sets.append((tracks, "Local Directory Tracks"))
 
     if not track_sets:
         return beatcloud_tracks, beatcloud_matches
 
     if not beatcloud_tracks:
         beatcloud_tracks = get_beatcloud_tracks()
-    
+
     path_lookup = {x.stem: x for x in beatcloud_tracks}
-    
+
     for tracks, track_type in track_sets:
         matches = find_matches(
             tracks,
             path_lookup.keys(),
             config,
         )
         logger.info(f"\n{track_type} / Beatcloud Matches: {len(matches)}")
         for loc, matches in groupby(
             sorted(matches, key=itemgetter(0)), key=itemgetter(0)
         ):
             logger.info(f"{loc}:")
             for _, track, beatcloud_track, fuzz_ratio in matches:
                 beatcloud_matches.append(path_lookup[beatcloud_track])
                 logger.info(f"\t{fuzz_ratio}: {track} | {beatcloud_track}")
-    
+
     if download_spotify_playlist:
         config.CHECK_TRACKS_SPOTIFY_PLAYLISTS = cached_playlists
         config.CHECK_TRACKS_LOCAL_DIRS = cached_local_dirs
 
     return beatcloud_tracks, beatcloud_matches
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/config.py` & `dj_beatcloud-2.5.0b0/djtools/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""This module contains the configuration object for the utils package. The
+attributes of this configuration object correspond with the "utils" key of
+config.yaml
+"""
 import logging
 from pathlib import Path
 from typing import List
 
 from pydantic import NonNegativeInt
 
 from djtools.configs.config import BaseConfig
@@ -9,15 +13,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class UtilsConfig(BaseConfig):
     """Configuration object for the utils package."""
 
-    CHECK_TRACKS: bool = False 
+    CHECK_TRACKS: bool = False
     CHECK_TRACKS_FUZZ_RATIO: NonNegativeInt = 80
     CHECK_TRACKS_LOCAL_DIRS:  List[Path] = []
     CHECK_TRACKS_SPOTIFY_PLAYLISTS:  List[str] = []
     URL_DOWNLOAD: str = ""
     URL_DOWNLOAD_DESTINATION: Path = None
 
     def __init__(self, *args, **kwargs):
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/helpers.py` & `dj_beatcloud-2.5.0b0/djtools/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,82 @@
 """This module contains helper functions that are not specific to any
-particular subpackage of this library.
+particular sub-package of this library.
 """
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from itertools import product
 import logging
 import logging.config
 import os
 from pathlib import Path
 from subprocess import check_output
 import tempfile
-from typing import Any, AsyncGenerator, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, List, Optional, Set, Tuple
 from unittest import mock
 
 from fuzzywuzzy import fuzz
 import spotipy
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
 from djtools.spotify.helpers import get_playlist_ids, get_spotify_client
 
 
 logger = logging.getLogger(__name__)
 
 
 class MockOpen:
+    """Class for mocking the builtin open function."""
     builtin_open = open
 
     def __init__(
         self,
         files: List[str],
         user_a: Optional[Tuple[str]] = None,
         user_b: Optional[Tuple[str]] = None,
         content: Optional[str] = "",
         write_only: Optional[bool] = False,
     ):
-        self._user_a = user_a 
-        self._user_b = user_b 
+        self._user_a = user_a
+        self._user_b = user_b
         self._files = files
         self._content = content
         self._write_only = write_only
 
     def open(self, *args, **kwargs):
+        """Function to replace the builtin open function.
+
+        Returns:
+            File handler.
+        """
         file_name = os.path.basename(args[0])
         if file_name in self._files:
             if "w" in kwargs.get("mode"):
                 return tempfile.TemporaryFile(mode=kwargs["mode"])
-            elif not self._write_only:
+            if not self._write_only:
                 return self._file_strategy(file_name, *args, **kwargs)
         return self.builtin_open(*args, **kwargs)
-    
+
     def _file_strategy(self, file_name, *args, **kwargs):
+        """Apply logic for file contents based on file name.
+
+        Args:
+            file_name: Name of the file to open.
+
+        Returns:
+            Mock file handler object.
+        """
+        data = "{}"
         if self._content:
             data = self._content
         elif file_name == "registered_users.yaml":
             data = (
                 f'{{"{self._user_a[0]}": "{self._user_a[1]}", '
                 f'"{self._user_b[0]}": "{self._user_b[1]}"}}'
             )
-        else:
-            data = "{}"
 
         return mock.mock_open(read_data=data)(*args, **kwargs)
 
 
 def add_tracks(result: Dict[str, Any]) -> List[str]:
     """Parses a page of Spotify API result tracks and returns a list of the
         track titles and artist names.
@@ -79,34 +92,14 @@
         title = track["track"]["name"]
         artists = ", ".join([y["name"] for y in track["track"]["artists"]])
         tracks.append(f"{title} - {artists}")
 
     return tracks
 
 
-async def catch(generator: AsyncGenerator, message: Optional[str] = "") -> Any:
-    """This function permits one-line try/except logic for comprehensions.
-
-    Args:
-        generator: Async generator.
-        message: Prefix message for logger warning.
-
-    Returns:
-        Return of the AsyncGenerator.
-    """
-    while True:
-        try:
-            yield await generator.__anext__()
-        except StopAsyncIteration:
-            return
-        except Exception as exc:
-            logger.warning(f"{message}: {exc}" if message else exc)
-            continue
-
-
 def compute_distance(
     spotify_playlist: str,
     spotify_track: str,
     beatcloud_track: str,
     threshold: float,
 ) -> Tuple[str, float]:
     """Qualifies a match between a Spotify track and a beatcloud track using
@@ -118,17 +111,19 @@
         beatcloud_track: Beatcloud track title and artist name
         threshold: Levenshtein similarity threshold for acceptance.
 
     Returns:
         Tuple of Spotify playlist, Spotify "TRACK TITLE - ARTIST NAME",
             beatcloud "TRACK TITLE - ARTIST NAME", Levenshtein similarity.
     """
+    ret = ()
     fuzz_ratio = fuzz.ratio(spotify_track, beatcloud_track)
     if fuzz_ratio >= threshold:
-        return spotify_playlist, spotify_track, beatcloud_track, fuzz_ratio
+        ret = spotify_playlist, spotify_track, beatcloud_track, fuzz_ratio
+    return ret
 
 
 def find_matches(
     spotify_tracks: Dict[str, Set[str]],
     beatcloud_tracks: List[str],
     config: BaseConfig,
 ) -> List[Tuple[str, float]]:
@@ -138,15 +133,15 @@
 
     Args:
         spotify_tracks: Spotify track titles and artist names.
         beatcloud_tracks: Beatcloud track titles and artist names.
         config: Configuration object.
 
     Returns:
-        List of tuples of Spotify playlist, Spotify track, Beatcloud track, andl
+        List of tuples of Spotify playlist, Spotify track, Beatcloud track, and
             Levenshtein distance.
     """
     spotify_tracks = [
         (playlist, track) for playlist, tracks in spotify_tracks.items()
         for track in tracks
     ]
     _product = list(product(spotify_tracks, beatcloud_tracks))
@@ -177,19 +172,18 @@
 def get_beatcloud_tracks() -> List[str]:
     """Lists all the music files in S3 and parses out the track titles and
         artist names.
     
     Returns:
         Beatcloud track titles and artist names.
     """
-    logger.info("Getting tracks from the beatcloud...")
     cmd = "aws s3 ls --recursive s3://dj.beatcloud.com/dj/music/"
     output = check_output(cmd, shell=True).decode("utf-8").split("\n")
     tracks = [Path(track) for track in output if track]
-    logger.info(f"Got {len(tracks)} tracks")
+    logger.info(f"Got {len(tracks)} tracks from the beatcloud")
 
     return tracks
 
 
 def get_local_tracks(config: BaseConfig) -> Dict[str, List[str]]:
     """Aggregates the files from one or more local directories in a dictionary
         mapped with parent directories.
@@ -204,16 +198,19 @@
     for _dir in config.CHECK_TRACKS_LOCAL_DIRS:
         if not _dir.exists():
             logger.warning(
                 f"{_dir} does not exist; will not be able to check its "
                 "contents against the beatcloud"
             )
             continue
-        files = _dir.rglob("**/*.*")
-        local_dir_tracks[_dir] = [_file.stem for _file in files]
+        files = [_file.stem for _file in _dir.rglob("**/*.*")]
+        if files:
+            local_dir_tracks[_dir] = files
+    local_tracks_count = sum(len(x) for x in local_dir_tracks.values())
+    logger.info(f"Got {local_tracks_count} files under local directories")
 
     return local_dir_tracks
 
 
 def get_playlist_tracks(
     spotify: spotipy.Spotify, playlist_id: str
 ) -> Set[str]:
@@ -256,28 +253,33 @@
     Returns:
         Spotify track titles and artist names keyed by playlist name.
     """
     spotify = get_spotify_client(config)
     playlist_ids = get_playlist_ids()
 
     playlist_tracks = {}
+    _sum = 0
     for playlist in config.CHECK_TRACKS_SPOTIFY_PLAYLISTS:
         playlist_id = playlist_ids.get(playlist)
         if not playlist_id:
             logger.error(f"{playlist} not in spotify_playlists.yaml")
             continue
 
-        logger.info(f'Getting tracks from Spotify playlist "{playlist}"...')
         playlist_tracks[playlist] = get_playlist_tracks(spotify, playlist_id)
         length = len(playlist_tracks[playlist])
-        logger.info(f"Got {length} track{'' if length == 1 else 's'}")
+        logger.info(
+            f'Got {length} track{"" if length == 1 else "s"} from Spotify '
+            f'playlist "{playlist}"'
+        )
+        _sum += length
 
         if config.VERBOSITY > 0:
             for track in playlist_tracks[playlist]:
                 logger.info(f"\t{track}")
+    logger.info(f"Got {_sum} tracks from Spotify in total")
 
     return playlist_tracks
 
 
 def initialize_logger() -> Tuple[logging.Logger, str]:
     """Initializes logger from configuration.
 
@@ -296,12 +298,14 @@
         disable_existing_loggers=False,
     )
 
     return logging.getLogger(__name__), log_file
 
 
 def mock_exists(files, path):
+    """Function for mocking the existence of pathlib.Path object."""
+    ret = True
     for file_name, exists in files:
         if file_name == path.name:
-            return exists
-
-    return True
+            ret = exists
+            break
+    return ret
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.5.0b0/djtools/utils/test_check_tracks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Testing for the check_tracks module."""
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.utils.check_tracks import compare_tracks
 
 
+
 @pytest.mark.parametrize("get_spotify_tracks_flag", [True, False])
 @pytest.mark.parametrize("get_local_tracks_flag", [True, False])
 @pytest.mark.parametrize("beatcloud_tracks", [[], [Path("track - artist")]])
 @pytest.mark.parametrize("download_spotify", ["", "playlist Uploads"])
 @mock.patch("djtools.utils.check_tracks.get_local_tracks", return_value={})
 @mock.patch(
     "djtools.utils.check_tracks.get_beatcloud_tracks",
@@ -24,26 +26,27 @@
     get_local_tracks_flag,
     beatcloud_tracks,
     download_spotify,
     test_config,
     tmpdir,
     caplog,
 ):
+    """Test the compare_tracks function."""
     caplog.set_level("INFO")
     spotify_playlist = "playlist"
     tmpdir = Path(tmpdir)
     test_config.CHECK_TRACKS = True
     test_config.CHECK_TRACKS_SPOTIFY_PLAYLISTS = [spotify_playlist]
     test_config.CHECK_TRACKS_LOCAL_DIRS = [tmpdir]
     test_config.DOWNLOAD_SPOTIFY = download_spotify
     if get_spotify_tracks_flag or download_spotify:
         mock_get_spotify_tracks.return_value = {"playlist": ["track - artist"]}
     if get_local_tracks_flag:
         mock_get_local_tracks.return_value = {tmpdir: ["track - artist"]}
-    ret_beatcloud_tracks, beatcloud_matches = compare_tracks(
+    compare_tracks(
         test_config,
         beatcloud_tracks,
         download_spotify_playlist=download_spotify,
     )
     if not get_spotify_tracks_flag and not download_spotify:
         assert caplog.records.pop(0).message == (
             "There are no Spotify tracks; make sure "
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.0b0/djtools/utils/test_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import asyncio
+"""Testing for the helpers module."""
 from datetime import datetime
 from pathlib import Path
 import logging
 from unittest import mock
 
 import pytest
 
 from djtools.utils.helpers import (
     add_tracks,
     compute_distance,
-    catch,
     find_matches,
-    initialize_logger,
     get_beatcloud_tracks,
     get_local_tracks,
     get_playlist_tracks,
     get_spotify_tracks,
+    initialize_logger,
+    MockOpen,
 )
-from djtools.utils.helpers import MockOpen
 
 
 def test_add_tracks():
+    """Test for the add_tracks function."""
     test_input = {
         "items": [
             {
                 "track": {
                     "name": "track title",
                     "artists": [ 
                         {"name": "artist name"},
@@ -46,64 +46,36 @@
         "track title - artist name",
         "another track title - another artist name, a second artist name"
     ]
     output = add_tracks(test_input)
     assert output == expected
 
 
-@pytest.mark.asyncio
-@pytest.mark.parametrize("message", ["", "oops"])
-async def test_catch(message, caplog):
-    exc = ZeroDivisionError("You can't divide by zero!")
-    class Generator:
-        def __init__(self):
-            self._iters = 2
-            self._i = 0
-
-        def __aiter__(self):
-            return self
-
-        async def __anext__(self):
-            if self._i >= self._iters:
-                raise StopAsyncIteration
-            self._i += 1
-            await asyncio.sleep(0.1)
-            if self._i % 2 == 0:
-                raise exc
-
-            return self._i
-
-    caplog.set_level("WARNING")
-    results = [x async for x in catch(Generator(), message=message)]
-    assert caplog.records[0].message == (
-        f"{message}: {str(exc)}" if message else str(exc)
-    )
-
-
 @pytest.mark.parametrize("track_a", ["some track", "another track"])
 @pytest.mark.parametrize("track_b", ["some track", "another track"])
 def test_compute_distance(track_a, track_b):
+    """Test for the compute_distance function."""
     ret = compute_distance(
         "playlist",
         track_a,
         track_b,
         99,
     )
     if track_a == track_b:
         assert ret
-        playlist, ret_track_a, ret_track_b, fuzz_ratio = ret
-        assert playlist == "playlist"
-        assert ret_track_a == track_a
-        assert ret_track_b == track_b
-        assert fuzz_ratio == 100
+        assert ret[0] == "playlist"
+        assert ret[1] == track_a
+        assert ret[2] == track_b
+        assert ret[3] == 100
     else:
         assert not ret
 
 
 def test_find_matches(test_config):
+    """Test for the find_matches function."""
     test_config.CHECK_TRACKS_FUZZ_RATIO = 99
     expected_matches = [
         "track 1 - someone unique",
         "track 2 - seen them before",
     ]
     matches = find_matches(
         spotify_tracks={
@@ -133,30 +105,32 @@
             "aweeeezy/Bass/2022-12-21/track - artist.mp3",
             "aweeeezy/Techno/2022-12-21/track - artist.mp3",
         ]
     ]
 )
 @mock.patch("djtools.utils.helpers.check_output")
 def test_get_beatcloud_tracks(mock_os_popen, proc_dump):
+    """Test for the get_beatcloud_tracks function."""
     proc_dump = list(map(Path, proc_dump))
-    process = mock_os_popen.return_value = b"\n".join(
+    mock_os_popen.return_value = b"\n".join(
         map(lambda x: x.as_posix().encode(), proc_dump)
     )
     tracks = get_beatcloud_tracks()
     mock_os_popen.assert_called_once()
     assert len(tracks) == len(proc_dump)
     for track, line in zip(tracks, proc_dump):
         assert track == line
 
 
 def test_get_local_tracks(tmpdir, test_config):
+    """Test for the get_local_tracks function."""
     check_dirs = []
     tmpdir = Path(tmpdir)
-    for dir in ["dir1", "dir2"]:
-        path = tmpdir / dir
+    for _dir in ["dir1", "dir2"]:
+        path = tmpdir / _dir
         path.mkdir(parents=True, exist_ok=True)
         check_dirs.append(path)
     test_config.CHECK_TRACKS_LOCAL_DIRS = check_dirs + [Path("nonexistent_dir")]
     beatcloud_tracks = ["test_file1.mp3", "test_file2.mp3"]
     for index, track in enumerate(beatcloud_tracks):
         with open(
             check_dirs[index % len(check_dirs)] / f"{track}",
@@ -165,14 +139,23 @@
         ) as _file:
             _file.write("")
     local_dir_tracks = get_local_tracks(test_config)
     assert all(x in local_dir_tracks for x in check_dirs)
     assert len(local_dir_tracks) == len(check_dirs)
 
 
+def test_get_local_tracks_empty(tmpdir, test_config, caplog):
+    """Test for the get_local_tracks function."""
+    caplog.set_level("INFO")
+    test_config.CHECK_TRACKS_LOCAL_DIRS = [Path(tmpdir)]
+    local_dir_tracks = get_local_tracks(test_config)
+    assert not local_dir_tracks
+    assert caplog.records[0].message == "Got 0 files under local directories"
+
+
 @mock.patch("djtools.spotify.helpers.spotipy.Spotify")
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify.next",
     return_value={
         "items": [
             {
                 "track": {
@@ -212,14 +195,15 @@
             "next": True,
         },
     },
 )
 def test_get_playlist_tracks(
     mock_spotipy_playlist, mock_spotipy_next, mock_spotipy
 ):
+    """Test for the get_playlist_tracks function."""
     mock_spotipy.playlist.return_value = mock_spotipy_playlist.return_value
     mock_spotipy.next.return_value = mock_spotipy_next.return_value
     expected = sorted(set([
         "track title - artist name",
         "another track title - another artist name, a second artist name",
         "last track title - final artist name"
     ]))
@@ -231,14 +215,15 @@
 @mock.patch(
     "djtools.spotify.helpers.spotipy.Spotify.playlist",
     side_effect=Exception()
 )
 def test_get_playlist_tracks_handles_spotipy_exception(
     mock_spotipy_playlist, mock_spotipy
 ):
+    """Test for the get_playlist_tracks function."""
     test_playlist_id = "some ID"
     mock_spotipy.playlist.side_effect = mock_spotipy_playlist.side_effect
     with pytest.raises(
         Exception, match=f"Failed to get playlist with ID {test_playlist_id}"
     ):
         get_playlist_tracks(mock_spotipy, test_playlist_id)
 
@@ -251,34 +236,35 @@
 @mock.patch(
     "djtools.utils.helpers.get_playlist_tracks",
     return_value={"some track - some artist"},
 )
 def test_get_spotify_tracks(
     mock_get_playlist_tracks, test_config, verbosity, caplog
 ):
+    """Test for the get_spotify_tracks function."""
     caplog.set_level("INFO")
     test_config.SPOTIFY_CLIENT_ID = "spotify client ID"
     test_config.SPOTIFY_CLIENT_SECRET = "spotify client secret"
     test_config.SPOTIFY_REDIRECT_URI = "spotify redirect uri"
     test_config.CHECK_TRACKS_SPOTIFY_PLAYLISTS = [
         "playlist A", "r/techno | Top weekly Posts"
     ]
     test_config.VERBOSITY = verbosity
     tracks = get_spotify_tracks(test_config)
     assert isinstance(tracks, dict)
     assert caplog.records[0].message == (
         "playlist A not in spotify_playlists.yaml"
     )
     assert caplog.records[1].message == (
-        'Getting tracks from Spotify playlist "r/techno | Top weekly Posts"...'
+        'Got 1 track from Spotify playlist "r/techno | Top weekly Posts"'
     )
-    assert caplog.records[2].message == "Got 1 track"
     if verbosity:
-        assert caplog.records[3].message == "\tsome track - some artist"
+        assert caplog.records[2].message == "\tsome track - some artist"
     mock_get_playlist_tracks.assert_called_once()
 
 
 def test_initialize_logger():
+    """Test for the intitialize_logger function."""
     today = f'{datetime.now().strftime("%Y-%m-%d")}.log'
     logger, log_file = initialize_logger()
     assert isinstance(logger, logging.Logger)
     assert log_file.name == today
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.0b0/djtools/utils/test_url_download.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Testing for the url_download module."""
 from pathlib import Path
 from unittest import mock
 
 import pytest
 from youtube_dl.utils import DownloadError
 
 from djtools.utils.url_download import fix_up, url_download
@@ -21,35 +22,39 @@
         (
             "Some Artist - Some Track.mp3",
             "Some Track - Some Artist.mp3",
         ),
     ],
 )
 def test_fix_up(test_assets):
+    """Test for the fix_up function."""
     test_file, expected_clean_file = map(Path, test_assets)
     clean_file = fix_up(test_file)
     assert clean_file == expected_clean_file
 
 
 def test_url_download(tmpdir, test_config):
+    """Test for the url_download function."""
     tmpdir = Path(tmpdir)
     test_config.URL_DOWNLOAD = (
         "https://soundcloud.com/aweeeezy_music/sets/test-download"
     )
     test_config.URL_DOWNLOAD_DESTINATION = tmpdir
+
+    def dummy_func():
+        with open(tmpdir / "file.mp3", mode="w", encoding="utf-8") as _file:
+            _file.write("")
+
     with mock.patch(
         "youtube_dl.YoutubeDL",
     ) as mock_ytdl:
-        context = mock_ytdl.return_value.__enter__.return_value 
-        context.download.side_effect = lambda *args, **kwargs: open(
-            tmpdir / "file.mp3",
-            mode="w",
-            encoding="utf-8",
-        ).write("")
+        context = mock_ytdl.return_value.__enter__.return_value
+        context.download.side_effect = lambda *args, **kwargs: dummy_func()
         url_download(test_config)
     assert len(list(tmpdir.iterdir())) == 1
 
 
 def test_url_download_invalid_url(test_config):
+    """Test for the url_download function."""
     test_config.URL_DOWNLOAD = ""
     with pytest.raises(DownloadError):
         url_download(test_config)
```

### Comparing `dj_beatcloud-2.4.1b9/djtools/utils/url_download.py` & `dj_beatcloud-2.5.0b0/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b9/setup.py` & `dj_beatcloud-2.5.0b0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,18 @@
 with open('README.md', encoding='utf-8') as _file:
     LONG_DESCRIPTION = _file.read()
 
 REQUIREMENTS = [
     "asyncpraw==7.6.1",
     "awscli==1.27.45",
     "beautifulsoup4==4.11.1",
-    "eyed3==0.9.7",
     "fuzzywuzzy==0.18.0",
     "lxml==4.9.2",
     "pydantic==1.9.1",
     "pyperclip==1.8.2",
-    "pytest==7.2.0",
-    "pytest-asyncio==0.20.3",
-    "pytest-cov==4.0.0",
     "PyYAML==5.4.1",
     "requests==2.28.0",
     "setuptools==58.1.0",
     "spotipy==2.21.0",
     "tqdm==4.64.0",
     "youtube-dl==2021.12.17",
 ]
@@ -48,30 +44,36 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b9',
+    version='2.5.0b0',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
     author='Alex Richards',
     author_email='alex.richards006@gmail.com',
     license='GNU GPLv3',
-    package_dir={"": "djtools"},
-    packages=find_packages(where="djtools"),
+    packages=[
+        "djtools",
+        "djtools.configs",
+        "djtools.rekordbox",
+        "djtools.spotify",
+        "djtools.sync",
+        "djtools.utils",
+    ],
     classifiers=CLASSIFIERS,
     install_requires=REQUIREMENTS,
     extras_require=EXTRAS,
     python_requires=">=3.6",
     include_package_data=True,
     keywords='MP3 Rekordbox XML spotify reddit aws s3',
     entry_points={
-        'console_scripts': ['djtools=djtools:dj_tools.main']
-    }
+        'console_scripts': ['djtools=djtools:main']
+    },
 )
```

