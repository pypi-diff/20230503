# Comparing `tmp/Shark sac Korean editor-0.0.1.tar.gz` & `tmp/Shark sac Korean editor-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shark sac Korean editor-0.0.1.tar", last modified: Wed May  3 02:38:27 2023, max compression
+gzip compressed data, was "Shark sac Korean editor-2.0.5.tar", last modified: Mon May  1 09:13:43 2023, max compression
```

## Comparing `Shark sac Korean editor-0.0.1.tar` & `Shark sac Korean editor-2.0.5.tar`

### file list

```diff
@@ -1,108 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.442234 Shark sac Korean editor-0.0.1/
--rw-rw-rw-   0        0        0     1071 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       95 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11064 2023-05-03 02:38:27.442234 Shark sac Korean editor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10427 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/README.md
--rw-rw-rw-   0        0        0      206 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 02:38:27.442234 Shark sac Korean editor-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1159 2023-05-03 02:37:03.000000 Shark sac Korean editor-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.352524 Shark sac Korean editor-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.371312 Shark sac Korean editor-0.0.1/src/Shark_sac_Korean_editor.egg-info/
--rw-rw-rw-   0        0        0    11064 2023-05-03 02:38:27.000000 Shark sac Korean editor-0.0.1/src/Shark_sac_Korean_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3305 2023-05-03 02:38:27.000000 Shark sac Korean editor-0.0.1/src/Shark_sac_Korean_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 02:38:27.000000 Shark sac Korean editor-0.0.1/src/Shark_sac_Korean_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-03 02:38:27.000000 Shark sac Korean editor-0.0.1/src/Shark_sac_Korean_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 02:38:27.000000 Shark sac Korean editor-0.0.1/src/Shark_sac_Korean_editor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.388026 Shark sac Korean editor-0.0.1/src/modkr2/
--rw-rw-rw-   0        0        0      281 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/__init__.py
--rw-rw-rw-   0        0        0     9605 2023-05-01 09:12:19.000000 Shark sac Korean editor-0.0.1/src/modkr2/__main__.py
--rw-rw-rw-   0        0        0    10240 2023-04-26 10:58:08.000000 Shark sac Korean editor-0.0.1/src/modkr2/adb_handler.py
--rw-rw-rw-   0        0        0    13764 2023-04-26 10:44:46.000000 Shark sac Korean editor-0.0.1/src/modkr2/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-04-26 08:21:08.000000 Shark sac Korean editor-0.0.1/src/modkr2/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.389284 Shark sac Korean editor-0.0.1/src/modkr2/edits/
--rw-rw-rw-   0        0        0       67 2023-04-26 08:19:36.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.394538 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8976 2023-04-27 12:50:49.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-04-26 08:20:39.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     4041 2023-04-27 11:46:25.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16755 2023-04-27 11:45:13.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.403355 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8994 2023-04-27 02:57:22.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11449 2023-04-30 07:58:40.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3262 2023-04-26 08:44:31.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1083 2023-04-27 03:03:55.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2883 2023-04-27 03:19:09.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1277 2023-04-27 03:06:18.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     8065 2023-04-27 02:58:27.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4634 2023-04-30 08:11:09.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.406849 Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      333 2023-04-26 10:32:02.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2878 2023-05-03 02:21:51.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3399 2023-05-03 02:25:01.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4130 2023-04-26 08:40:01.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.421929 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-04-30 08:16:08.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/aku.py
--rw-rw-rw-   0        0        0      516 2023-04-26 09:33:48.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      869 2023-04-26 09:29:09.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      650 2023-04-26 10:31:23.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6389 2023-04-26 09:30:45.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     2062 2023-04-26 09:29:36.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1056 2023-04-26 09:28:52.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1481 2023-04-30 09:04:42.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     1100 2023-05-02 09:06:11.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/lengthsa.py
--rw-rw-rw-   0        0        0     4451 2023-04-27 03:25:53.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2361 2023-04-26 09:35:46.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3106 2023-04-27 03:25:08.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1227 2023-04-26 09:29:23.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8576 2023-04-27 03:28:15.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1082 2023-04-26 09:16:16.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      802 2023-04-30 08:25:27.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.433044 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/
--rw-rw-rw-   0        0        0      276 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3913 2023-04-26 10:25:28.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1124 2023-04-26 10:23:52.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2236 2023-04-26 09:44:49.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      698 2023-04-26 09:46:24.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3510 2023-04-26 10:22:39.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7140 2023-04-26 10:03:11.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4384 2023-04-26 10:17:15.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/missions.py
--rw-rw-rw-   0        0        0     1016 2023-04-26 10:13:14.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1657 2023-04-26 10:18:48.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1426 2023-04-26 10:16:14.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      356 2023-04-26 10:30:56.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.438959 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-04-26 11:02:30.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2795 2023-04-26 11:01:45.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/load.py
--rw-rw-rw-   0        0        0      661 2023-04-26 10:58:58.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1906 2023-04-30 08:09:14.000000 Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    13855 2023-04-30 09:03:37.000000 Shark sac Korean editor-0.0.1/src/modkr2/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-04-26 08:26:01.000000 Shark sac Korean editor-0.0.1/src/modkr2/game_data_getter.py
--rw-rw-rw-   0        0        0    23001 2023-04-30 08:04:44.000000 Shark sac Korean editor-0.0.1/src/modkr2/helper.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/item.py
--rw-rw-rw-   0        0        0     3505 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/managed_item.py
--rw-rw-rw-   0        0        0    66980 2023-05-03 02:19:48.000000 Shark sac Korean editor-0.0.1/src/modkr2/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-04-30 07:47:55.000000 Shark sac Korean editor-0.0.1/src/modkr2/patcher.py
--rw-rw-rw-   0        0        0     2450 2023-04-26 10:55:23.000000 Shark sac Korean editor-0.0.1/src/modkr2/root_handler.py
--rw-rw-rw-   0        0        0    53823 2023-04-26 08:24:37.000000 Shark sac Korean editor-0.0.1/src/modkr2/serialise_save.py
--rw-rw-rw-   0        0        0    25211 2023-04-26 10:54:03.000000 Shark sac Korean editor-0.0.1/src/modkr2/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/tracker.py
--rw-rw-rw-   0        0        0     3544 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/updater.py
--rw-rw-rw-   0        0        0     4474 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/src/modkr2/user_info.py
--rw-rw-rw-   0        0        0     8297 2023-04-25 08:36:00.000000 Shark sac Korean editor-0.0.1/src/modkr2/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-03 02:38:27.440954 Shark sac Korean editor-0.0.1/tests/
--rw-rw-rw-   0        0        0      648 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/tests/test_helper.py
--rw-rw-rw-   0        0        0     6784 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/tests/test_item.py
--rw-rw-rw-   0        0        0     1103 2023-04-19 18:25:16.000000 Shark sac Korean editor-0.0.1/tests/test_parse.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.242415 Shark sac Korean editor-2.0.5/
+-rw-rw-rw-   0        0        0      731 2023-05-01 09:13:43.242415 Shark sac Korean editor-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.178087 Shark sac Korean editor-2.0.5/Shark_sac_Korean_editor.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-05-01 09:13:43.000000 Shark sac Korean editor-2.0.5/Shark_sac_Korean_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-05-01 09:13:43.000000 Shark sac Korean editor-2.0.5/Shark_sac_Korean_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:13:43.000000 Shark sac Korean editor-2.0.5/Shark_sac_Korean_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 09:13:43.000000 Shark sac Korean editor-2.0.5/Shark_sac_Korean_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.193045 Shark sac Korean editor-2.0.5/modkr/
+-rw-rw-rw-   0        0        0      281 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/__init__.py
+-rw-rw-rw-   0        0        0     9605 2023-05-01 09:12:19.000000 Shark sac Korean editor-2.0.5/modkr/__main__.py
+-rw-rw-rw-   0        0        0    10240 2023-04-26 10:58:08.000000 Shark sac Korean editor-2.0.5/modkr/adb_handler.py
+-rw-rw-rw-   0        0        0    13764 2023-04-26 10:44:46.000000 Shark sac Korean editor-2.0.5/modkr/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-04-26 08:21:08.000000 Shark sac Korean editor-2.0.5/modkr/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.194042 Shark sac Korean editor-2.0.5/modkr/edits/
+-rw-rw-rw-   0        0        0       67 2023-04-26 08:19:36.000000 Shark sac Korean editor-2.0.5/modkr/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.199499 Shark sac Korean editor-2.0.5/modkr/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8976 2023-04-27 12:50:49.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-04-26 08:20:39.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     4041 2023-04-27 11:46:25.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16755 2023-04-27 11:45:13.000000 Shark sac Korean editor-2.0.5/modkr/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.207974 Shark sac Korean editor-2.0.5/modkr/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8994 2023-04-27 02:57:22.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11449 2023-04-30 07:58:40.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3262 2023-04-26 08:44:31.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1083 2023-04-27 03:03:55.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2883 2023-04-27 03:19:09.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1277 2023-04-27 03:06:18.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     8065 2023-04-27 02:58:27.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4634 2023-04-30 08:11:09.000000 Shark sac Korean editor-2.0.5/modkr/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.212563 Shark sac Korean editor-2.0.5/modkr/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-04-26 10:32:02.000000 Shark sac Korean editor-2.0.5/modkr/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2835 2023-04-26 08:38:24.000000 Shark sac Korean editor-2.0.5/modkr/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3399 2023-04-26 08:41:50.000000 Shark sac Korean editor-2.0.5/modkr/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4130 2023-04-26 08:40:01.000000 Shark sac Korean editor-2.0.5/modkr/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.225522 Shark sac Korean editor-2.0.5/modkr/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-04-30 08:16:08.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      516 2023-04-26 09:33:48.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      869 2023-04-26 09:29:09.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      650 2023-04-26 10:31:23.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6389 2023-04-26 09:30:45.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     2062 2023-04-26 09:29:36.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1056 2023-04-26 09:28:52.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1481 2023-04-30 09:04:42.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4451 2023-04-27 03:25:53.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2361 2023-04-26 09:35:46.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3106 2023-04-27 03:25:08.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1227 2023-04-26 09:29:23.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8576 2023-04-27 03:28:15.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1082 2023-04-26 09:16:16.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      802 2023-04-30 08:25:27.000000 Shark sac Korean editor-2.0.5/modkr/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.236134 Shark sac Korean editor-2.0.5/modkr/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3913 2023-04-26 10:25:28.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1124 2023-04-26 10:23:52.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2236 2023-04-26 09:44:49.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      698 2023-04-26 09:46:24.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3510 2023-04-26 10:22:39.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7140 2023-04-26 10:03:11.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4384 2023-04-26 10:17:15.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/missions.py
+-rw-rw-rw-   0        0        0     1016 2023-04-26 10:13:14.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1657 2023-04-26 10:18:48.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1426 2023-04-26 10:16:14.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      356 2023-04-26 10:30:56.000000 Shark sac Korean editor-2.0.5/modkr/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:13:43.241418 Shark sac Korean editor-2.0.5/modkr/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-26 11:02:30.000000 Shark sac Korean editor-2.0.5/modkr/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2795 2023-04-26 11:01:45.000000 Shark sac Korean editor-2.0.5/modkr/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      661 2023-04-26 10:58:58.000000 Shark sac Korean editor-2.0.5/modkr/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1906 2023-04-30 08:09:14.000000 Shark sac Korean editor-2.0.5/modkr/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    13855 2023-04-30 09:03:37.000000 Shark sac Korean editor-2.0.5/modkr/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-04-26 08:26:01.000000 Shark sac Korean editor-2.0.5/modkr/game_data_getter.py
+-rw-rw-rw-   0        0        0    23001 2023-04-30 08:04:44.000000 Shark sac Korean editor-2.0.5/modkr/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/item.py
+-rw-rw-rw-   0        0        0     3505 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/managed_item.py
+-rw-rw-rw-   0        0        0    66980 2023-04-25 17:12:37.000000 Shark sac Korean editor-2.0.5/modkr/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-04-30 07:47:55.000000 Shark sac Korean editor-2.0.5/modkr/patcher.py
+-rw-rw-rw-   0        0        0     2450 2023-04-26 10:55:23.000000 Shark sac Korean editor-2.0.5/modkr/root_handler.py
+-rw-rw-rw-   0        0        0    53823 2023-04-26 08:24:37.000000 Shark sac Korean editor-2.0.5/modkr/serialise_save.py
+-rw-rw-rw-   0        0        0    25211 2023-04-26 10:54:03.000000 Shark sac Korean editor-2.0.5/modkr/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/tracker.py
+-rw-rw-rw-   0        0        0     3544 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-04-25 08:36:00.000000 Shark sac Korean editor-2.0.5/modkr/user_input_handler.py
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:13:43.242415 Shark sac Korean editor-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-05-01 09:12:41.000000 Shark sac Korean editor-2.0.5/setup.py
```

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/__main__.py` & `Shark sac Korean editor-2.0.5/modkr/__main__.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/adb_handler.py` & `Shark sac Korean editor-2.0.5/modkr/adb_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/config_manager.py` & `Shark sac Korean editor-2.0.5/modkr/config_manager.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/csv_handler.py` & `Shark sac Korean editor-2.0.5/modkr/csv_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/basic_items.py` & `Shark sac Korean editor-2.0.5/modkr/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/catfruit.py` & `Shark sac Korean editor-2.0.5/modkr/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/catseyes.py` & `Shark sac Korean editor-2.0.5/modkr/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/ototo_base_mats.py` & `Shark sac Korean editor-2.0.5/modkr/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/talent_orbs.py` & `Shark sac Korean editor-2.0.5/modkr/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/basic/talent_orbs_new.py` & `Shark sac Korean editor-2.0.5/modkr/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/cat_helper.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/cat_id_selector.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/chara_drop.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/clear_cat_guide.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/evolve_cats.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/get_remove_cats.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/talents.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/upgrade_blue.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/cats/upgrade_cats.py` & `Shark sac Korean editor-2.0.5/modkr/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/gamatoto_xp.py` & `Shark sac Korean editor-2.0.5/modkr/edits/gamototo/gamatoto_xp.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_boundaries(is_jp: bool) -> Optional[list[int]]:
     """Get the xp requirements for each level"""
 
     file_data = game_data_getter.get_file_latest(
         "DataLocal", "GamatotoExpedition.csv", is_jp
     )
     if file_data is None:
-        helper.error_text("가마토토 경험치 요구 사항을 가져오지 못했습니다.")
+        helper.error_text("Failed to get gamatoto xp requirements")
         return None
     boundaries = file_data.decode("utf-8").splitlines()
     previous = 0
     xp_requirements: list[int] = []
     previous = 0
     for line in boundaries:
         requirement = int(line.split(",")[0])
@@ -48,29 +48,29 @@
 
     xp_requirements = get_boundaries(is_jp)
     if xp_requirements is None:
         return None
     if level <= 1:
         gamatoto_xp = 0
     else:
-        gamatoto_xp = xp_requirements[level - 1]
+        gamatoto_xp = xp_requirements[level - 2]
     return gamatoto_xp
 
 
 def edit_gamatoto_xp(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for gamatoto xp"""
 
     gamatoto_xp = save_stats["gamatoto_xp"]
 
     data = get_level_from_xp(gamatoto_xp["Value"], helper.check_data_is_jp(save_stats))
     if data is None:
         return save_stats
     level = data["level"]
 
-    helper.colored_text(f"가마토토 경험치: &{gamatoto_xp['Value']}&\n레벨: &{level}&")
+    helper.colored_text(f"Gamatoto xp: &{gamatoto_xp['Value']}&\nLevel: &{level}&")
     raw = (
         user_input_handler.colored_input(
             "가마토토 경험치를 편집하시겠습니까?(&1&)또는 레벨(&2&)?:"
         )
         == "1"
     )
```

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/helpers.py` & `Shark sac Korean editor-2.0.5/modkr/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/gamototo/ototo_cat_cannon.py` & `Shark sac Korean editor-2.0.5/modkr/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/aku.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/allow_filibuster_clearing.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/behemoth_culling.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/clear_tutorial.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/enigma_stages.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/event_stages.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/gauntlet.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/itf_timed_scores.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/legend_quest.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/lengthsa.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/uncanny.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""Handler for editting lengthsa legends"""
+"""Handler for editting uncanny legends"""
 from typing import Any
 
 from . import event_stages
 from ... import user_input_handler
 
-def edit_lengthsa(save_stats: dict[str, Any]) -> dict[str, Any]:
-    """Handler for editting lengthsa legends"""
-    stage_data = save_stats["lengthsa"]
+def edit_uncanny(save_stats: dict[str, Any]) -> dict[str, Any]:
+    """Handler for editting uncanny legends"""
+    stage_data = save_stats["uncanny"]
     lengths = stage_data["Lengths"]
 
     ids = []
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "단계 ID 입력(예: &1& = 제로 필드, &2& = 시공간의 가장자리)(모든 범위를 가져오려면 &all&을 입력할 수 있습니다. 예: &1&-&49& 또는 공백으로 구분된 ID(예: &5 4 7&)):"
+            "단계 ID 입력(예: &1& = 새 범례, &2& = 여기 드래곤)(모든 범위를 가져오려면 &all&을 입력할 수 있습니다. 예: &1&-&49& 또는 공백으로 구분된 ID(예: &5 4 7&)):"
         ),
         lengths["total"],
     )
-    save_stats["lengthsa"] = event_stages.stage_handler(stage_data, ids, -1)
+    save_stats["uncanny"] = event_stages.stage_handler(stage_data, ids, -1)
 
     return save_stats
 
 def is_ancient_curse_clear(save_stats: dict[str, Any]) -> bool:
     """
     Check if the ancient curse is cleared
 
     Args:
         save_stats (dict[str, Any]): The save stats
 
     Returns:
         bool: If the ancient curse is cleared
     """
-    return save_stats["lengthsa"]["Value"]["clear_progress"][0][0] >= 1
+    return save_stats["uncanny"]["Value"]["clear_progress"][0][0] >= 1
```

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/main_story.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/outbreaks.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/story_level_id_selector.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/towers.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/treasures.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/levels/unlock_aku_realm.py` & `Shark sac Korean editor-2.0.5/modkr/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/cat_shrine.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/claim_user_rank_rewards.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/create_new_account.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/fix_elsewhere.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/fix_time_issues.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/get_gold_pass.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/meow_medals.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/missions.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/play_time.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/scheme_item.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/trade_progress.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/other/unlock_enemy_guide.py` & `Shark sac Korean editor-2.0.5/modkr/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/convert.py` & `Shark sac Korean editor-2.0.5/modkr/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/load.py` & `Shark sac Korean editor-2.0.5/modkr/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/other.py` & `Shark sac Korean editor-2.0.5/modkr/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/save.py` & `Shark sac Korean editor-2.0.5/modkr/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/edits/save_management/server_upload.py` & `Shark sac Korean editor-2.0.5/modkr/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/feature_handler.py` & `Shark sac Korean editor-2.0.5/modkr/feature_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/game_data_getter.py` & `Shark sac Korean editor-2.0.5/modkr/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/helper.py` & `Shark sac Korean editor-2.0.5/modkr/helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/item.py` & `Shark sac Korean editor-2.0.5/modkr/item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/locale_handler.py` & `Shark sac Korean editor-2.0.5/modkr/locale_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/managed_item.py` & `Shark sac Korean editor-2.0.5/modkr/managed_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/parse_save.py` & `Shark sac Korean editor-2.0.5/modkr/parse_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/patcher.py` & `Shark sac Korean editor-2.0.5/modkr/patcher.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/root_handler.py` & `Shark sac Korean editor-2.0.5/modkr/root_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/serialise_save.py` & `Shark sac Korean editor-2.0.5/modkr/serialise_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/server_handler.py` & `Shark sac Korean editor-2.0.5/modkr/server_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/tracker.py` & `Shark sac Korean editor-2.0.5/modkr/tracker.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/updater.py` & `Shark sac Korean editor-2.0.5/modkr/updater.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-0.0.1/src/modkr2/user_input_handler.py` & `Shark sac Korean editor-2.0.5/modkr/user_input_handler.py`

 * *Files identical despite different names*

